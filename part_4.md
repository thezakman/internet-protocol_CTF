                                                              
```
  ___ _  _ _____ ___ ___ _  _ ___ _____   ___ ___  ___ _____ ___   ___ ___  _    
 |_ _| \| |_   _| __| _ \ \| | __|_   _| | _ \ _ \/ _ \_   _/ _ \ / __/ _ \| |   
  | || .` | | | | _||   / .` | _|  | |   |  _/   / (_) || || (_) | (_| (_) | |__ 
 |___|_|\_| |_| |___|_|_\_|\_|___| |_|   |_| |_|_\\___/ |_| \___/ \___\___/|____|
                                                                
                                                                 DATE: 26-03-2019
                                                                 @TheZakMan

 [ URL: http://80.211.167.123/ ]



MBR SERVER STATUS

21/tcp	FTP	ONLINE
23/tcp	TELNET/BBS	ONLINE
25/tcp	SMTP	ONLINE
70/tcp	GOPHER	ONLINE
80/tcp	HTTP	ONLINE
110/tcp	POP3	ONLINE
6667/tcp	IRC	ONLINE


TIME TO HACK :)

,---,---,---,---,---,---,---,---,---,---,---,---,---,-------,
| ~ | 1 | 2 | 3 | 4 | 5 | 6 | 7 | 8 | 9 | 0 | [ | ] | <-    |
|---'-,-'-,-'-,-'-,-'-,-'-,-'-,-'-,-'-,-'-,-'-,-'-,-'-,-----|
| ->| | " | , | . | P | Y | F | G | C | R | L | / | = |  \  |
|-----',--',--',--',--',--',--',--',--',--',--',--',--'-----|
| Caps | A | O | E | U | I | D | H | T | N | S | - |  Enter |
|------'-,-'-,-'-,-'-,-'-,-'-,-'-,-'-,-'-,-'-,-'-,-'--------|
|        | ; | Q | J | K | X | B | M | W | V | Z |          |
|------,-',--'--,'---'---'---'---'---'---'-,-'---',--,------|
| ctrl |  | alt |                          | alt  |  | ctrl |
'------'  '-----'--------------------------'------'  '------'

root@kali:~# nmap -sV --script=banner 80.211.167.123
Starting Nmap 7.70 ( https://nmap.org ) at 2019-03-26 19:43 EDT
Nmap scan report for host123-167-211-80.serverdedicati.aruba.it (80.211.167.123)
Host is up (0.059s latency).
Not shown: 994 filtered ports
PORT     STATE SERVICE VERSION
21/tcp   open  ftp     IIS ftpd 7
|_banner: 220



ftp> open 80.211.167.123
Connected to 80.211.167.123.
220 
Name (80.211.167.123:root): anonymous
331 Anonymous access allowed, send identity (e-mail name) as password.
Password:
230-Welcome to the FTP server of MBR. Be kind and say hi to all other servers!
230 User logged in.
Remote system type is Windows_NT.
ftp> dir
200 PORT command successful.
125 Data connection already open; Transfer starting.
03-19-19  09:39PM              4993069 modem.wav
03-19-19  07:29PM               786489 www.bmp
226 Transfer complete.




$ zsteg -E b1,rgb,msb,XY www.bmp | strings | rev 
pass.txt  nothingiseverything
TAG:Int21




<killernat> pay attention to the tip about monalisa (BBS) it will lead you to the tool you need to find the last part
<killernat> and with that i need to sleep
<killernat> by the way the tool borks on both files


[BBS]

1#
Send me an email to masterbootrecord@protonmail.com once you have found the code word and i'll give you the prize.

The first part of the string is on the Gopher server.
Good luck!

MASTER BOOT RECORD
Heavy Metal is not dead. It was just not evenly synthesized.


23#
Hello dear Keygen,
Can you send me the code please?
Thank you
Best Regards,
CodeError0

#24
Wrong server.
The Keygen

27#
Saving you some brain damage
http://80.211.167.123/mbr.png.txt

#31
Some Hints for FTP Files.
Hint1) Beware the cats. They can contain malware.
Hint2) Mona Lisa knows the solution.
Hint3) Don't Call that phone number LOL
Hint4) Beware of red herrings!

#33

Don't forget to check the Voting boot on V and cast your vote or add some new questions. ;)

STRING: 
(1/4) GOPHER Server


```
