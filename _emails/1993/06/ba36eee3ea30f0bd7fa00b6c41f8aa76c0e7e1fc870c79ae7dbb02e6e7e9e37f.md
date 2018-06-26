---
layout: default
---

# 1993-06-05 - Re: Software infrastructure

## Header Data

From: J. Michael Diehl \<mdiehl<span>@</span>triton.unm.edu\><br>
To: nobody@soda.berkeley.edu<br>
Message Hash: ba36eee3ea30f0bd7fa00b6c41f8aa76c0e7e1fc870c79ae7dbb02e6e7e9e37f<br>
Message ID: \<9306050100.AA12806@triton.unm.edu\><br>
Reply To: \<9306040600.AA20309@soda.berkeley.edu\><br>
UTC Datetime: 1993-06-05 01:01:06 UTC<br>
Raw Date: Fri, 4 Jun 93 18:01:06 PDT<br>

## Raw message

```
{% raw  %}From: J. Michael Diehl <mdiehl@triton.unm.edu>
Date: Fri, 4 Jun 93 18:01:06 PDT
To: nobody@soda.berkeley.edu
Subject: Re: Software infrastructure
In-Reply-To: <9306040600.AA20309@soda.berkeley.edu>
Message-ID: <9306050100.AA12806@triton.unm.edu>
MIME-Version: 1.0
Content-Type: text/plain


According to nobody@soda.berkeley.edu:
> 
> From: Hal Finney, <74076.1041@compuserve.com>
>  
> Mike Diehl's system sounds pretty good to me.  You can create messages, 
> encrypt them, upload and send them, as well as downloading, decrypting, and 
> reading messages, all with a nice menu-based interface.  That's what we 
> want, right?
>  
> It sounds like the system would be easily adaptable to other types of hosts, 
> too.  BBS operators could customize the scripts for their particular systems 
> and offer the package.  We could create versions for users of other mail 
> packages than elm on Unix systems, as well as for some of the commercial 
> systems.  You could cover a lot of people this way.

Making it adaptable is what I mean by "cleaning it up a bit." ;^)

> > Well, if you have followed my this far, you either crazy or interested.;^)  
> > It puzzles me why we are contemplating writing our own comm package when so 
> > many good ones are out there that can be made to serve our purposes.  I'm 
> > open to comments.....  Fire away!
>  
> The only real problem I see is the use of Telix.  How much does this program 
> cost?  We can't give away a disk with Telix on it.

Telix is "user supported software."  Registering it costs $39.

>  
> What about Kermit?  It's free and it has a scripting language, but it 
> doesn't sound nearly as advanced as Telix's.  Would it be good enough?  Or 
> are their other free programs which we could use?

I remember kermit's script language as being kinda messy...  At the end of this
message, I will include a portion of my, uncommented, script to compare.  Also,
kermit is (I think) restricted to one xfer protocol, which may not be a good
idea.

> If we could adapt Kermit or some other free program to do what Mike is 
> describing, we could give away floppies with secure and easy-to-use 
> encrypted email handling capabilities, as well as making them available on 
> the net.  People could just get the version they need for their particular 
> mail access.method.  The package would include the communication program, 
> the scripts, and the encryption software.  The user interface would be as 
> Mike described, all menu driven and easy to use.

Well, either way, I will contribute my user-interface if you'all want it.  I'm
not married to telix, but I do think it is very good.  We could write comparable
scripts in every major comm program script language.... I'd have to document
my interface.  But if I decide to port my interface to C, I'd like to change 
a few things, so maybe this is a bit premature.....

> I think this would be a good way to go if we could get past the hurdle of 
> finding a free comm program that would be adequate.
> Note added in proof :)

I don't understand this last comment.  Maybe it's obvious and I'm just tired...
Part of my script system is after my signature.  Note that I hacked in a C
preprocesser, and this is the output from it, just before the script is compiled
Yes, Telix scripts are compiled! ;^)

 
+-----------------------+-----------------------------+---------+
| J. Michael Diehl ;-)  | I thought I was wrong once. | PGP KEY |
| mdiehl@triton.unm.edu |   But, I was mistaken.      |available|
| mike.diehl@fido.org   |                             | Ask Me! |
| (505) 299-2282        +-----------------------------+---------+
|                                                               |
+------"I'm just looking for the opportunity to be -------------+
|            Politically Incorrect!"   <Me>                     |
+-----If codes are outlawed, only criminals wil have codes.-----+
+----Is Big Brother in your phone?  If you don't know, ask me---+


str	PROMPT[] = "%";
str	PASSWRD[15];
 
command( str cmd ) 
{
	enter( cmd );
	while ( ! waitfor(PROMPT, 90));
}
 
enter( str cmd )
{
	cputs( cmd );
	cputs( "^M" );
}
 
match( str rec, str snd )
{
	while ( ! waitfor(rec, 90));
	enter( snd );
}
 
 
 
str	name[40] = "",
	file[40] = "",
	subject[40] = "",
	buff[80];
 
int	f,
	i;
 
main()
{ 
	if ( ! carrier()) 
		if ( dial("1", 10, 0) < 1) {
			prints("Could not dial in.");
			exittelix();
		}
 
	cputs("^M");
	command("biff n");
	
	if ( ! waitfor("%", 90)) {
		prints("No prompt after login");
		return;
	}
	
/*/ routing format is:  filename\n address\n subject\n /*/ 

	if ((f = fopen("c:\uload\mail\routing", "r")) ==0) return;
	while (feof(f) == 0) {
 
		fgets(file, 40, f);
		if (feof(f) != 0) continue;
		fgets(name, 40, f);
		if (feof(f) != 0) continue;
		fgets(subject, 40, f);
		if (feof(f) != 0) continue;
 
		buff = "";
		strcat(buff, "elm ");
		strcat(buff, name);
		enter(buff);
 
		match("Subject:", subject);
		delay_scr(10);
		cputs("i");
		_asc_scrtrans=1;
		_asc_slftrans=0;
		send('A', file);
		command("^[:wq^Ms^M");  
 
		fdelete(file);
 
	} 
	fdelete("c:\uload\mail\routing");
	
 
	f = fclose(f);
}
	
  



{% endraw %}
```

## Thread

+ Return to [June 1993](/archive/1993/06)

+ Return to "[bhoward<span>@</span>is.morgan.com (Bruce Howard)](/author/bhoward_at_is_morgan_com_bruce_howard_)"
+ Return to "[J. Michael Diehl <mdiehl<span>@</span>triton.unm.edu>](/author/j_michael_diehl_mdiehl_at_triton_unm_edu_)"
+ Return to "[nobody<span>@</span>soda.berkeley.edu](/author/nobody_at_soda_berkeley_edu)"
+ Return to "[Stanton McCandlish <anton<span>@</span>hydra.unm.edu>](/author/stanton_mccandlish_anton_at_hydra_unm_edu_)"

+ 1993-06-04 (Thu, 3 Jun 93 23:04:13 PDT) - [Software infrastructure](/archive/1993/06/ab5d0d052b5431422a98d598de18a4044e94c978f87eb2399098dc22380c5161) - _nobody@soda.berkeley.edu_
  + 1993-06-04 (Fri, 4 Jun 93 03:32:25 PDT) - [Re: Software infrastructure](/archive/1993/06/d5b8fbb5a8e485f8d055407cb7a1de80f8fac30baeeb9270c76bd53e4622eb14) - _Stanton McCandlish \<anton@hydra.unm.edu\>_
    + 1993-06-04 (Fri, 4 Jun 93 10:07:22 PDT) - [Re: Software infrastructure](/archive/1993/06/f810be4d19ce78319a844d115c757320c3e780ca13faea22e10482438c271beb) - _bhoward@is.morgan.com (Bruce Howard)_
    + 1993-06-05 (Fri, 4 Jun 93 18:09:16 PDT) - [Re: Software infrastructure](/archive/1993/06/8b42f377921a6c5466b792384578828e17df9c1a56706d5a7bfaab1372957d77) - _J. Michael Diehl \<mdiehl@triton.unm.edu\>_
  + 1993-06-05 (Fri, 4 Jun 93 18:01:06 PDT) - Re: Software infrastructure - _J. Michael Diehl \<mdiehl@triton.unm.edu\>_

