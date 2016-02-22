---
published: true
---


#Linux Mint Compromised by Unknown Hackers
![linux mint logo]({{site.baseurl}}/http://www.case-badges.com/images/linux_mint_label_1.jpg)
> **What happened?**

> Hackers made a modified Linux Mint ISO, with a backdoor in it, and managed to hack our website to point to it.
Does this affect you?

> As far as we know, the only compromised edition was Linux Mint 17.3 Cinnamon edition.

> If you downloaded another release or another edition, this does not affect you. If you downloaded via torrents or via a direct HTTP link, this doesn’t affect you either.

> Finally, the situation happened today, so it should only impact people who downloaded this edition on February 20th.

> **How to check if your ISO is compromised?**

> If you still have the ISO file, check its MD5 signature with the command “md5sum yourfile.iso” (where yourfile.iso is the name of the ISO).

> Once in the live session, **if there is a file in /var/lib/man.cy, then this is an infected ISO.**

##Malware in GNU/Linux what? What malware it is?
A some security researcher detected this malware is just a modification of Kaiten,this malware is commonly used on DDoS attacks and nothing much more really. Unixfreaxjp wrote about this malware [here](http://blog.malwaremustdie.org/2013/05/story-of-unix-trojan-tsunami-ircbot-w.html "here").
Aaaand a decompile of this sample is [here.](https://gist.github.com/Oweoqi/31239851e5b84dbba894 "here.")

##Give me some more info...
The code below is what researchers find:
				CHAN "#mint" //The channel where bots connect
				char *servers[] = updates.absentvodka.com //The IRC where the bad actors manipulate his zombies to launch attacks	
Well, doing a simple whois on the domain looks the bad actors delete everything about that domain and doesn't show any DNS Records but the infected ISOs we're hosted on Bulgaria according to Clem.

##How works this malware?
Made your computer a zombie and connect into IRC with a lot of others zombies computers and launch DDoS (Distributed Denial of Service) to other computers basically saturating the computer with millions of requests.

##Well i'm infected how i can remove this shit?
The best solution is reinstall the ISO and check the hash of the ISO file, anyway if you have backups that's not a big problem for deal with it. **The malware itself can't infect other files** since malware is not like Windows and can self-replicate because Linux is a very great isolated enviroment. 

###That's my first post, i hope you enjoy it.
