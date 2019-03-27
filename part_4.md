                                                              
```
# Part - 4 (FTP + BBS + IRC)
  ___ _  _ _____ ___ ___ _  _ ___ _____   ___ ___  ___ _____ ___   ___ ___  _    
 |_ _| \| |_   _| __| _ \ \| | __|_   _| | _ \ _ \/ _ \_   _/ _ \ / __/ _ \| |   
  | || .` | | | | _||   / .` | _|  | |   |  _/   / (_) || || (_) | (_| (_) | |__ 
 |___|_|\_| |_| |___|_|_\_|\_|___| |_|   |_| |_|_\\___/ |_| \___/ \___\___/|____|
                                                                
                                                                 DATE: 26-03-2019
                                                                 @TheZakMan

 [ URL: http://80.211.167.123/ ]


root@kali:~# nmap -sV --script=banner 80.211.167.123
Starting Nmap 7.70 ( https://nmap.org ) at 2019-03-26 19:43 EDT
Nmap scan report for host123-167-211-80.serverdedicati.aruba.it (80.211.167.123)
Host is up (0.059s latency).
Not shown: 994 filtered ports
PORT     STATE SERVICE VERSION
21/tcp   open  ftp     IIS ftpd 7
|_banner: 220
```

```
┌─╔═╗╔╦╗╔═╗─┐
│ ╠╣  ║ ╠═╝ │
└─╚   ╩ ╩  ─┘

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

```
```
 __ ____  ____  ___ __ 
|  (  _ \(  _ \/ __)  |
|   ) _ < ) _ <\__ \  |
|__(____/(____/(___/__|

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
```

```
https://xiao-steganography.softonic.com.br/
https://download.cnet.com/g00/Xiao-Steganography/


Extracted 2 files:
modem.wav.txt & www.bmp.txt

cat www.bmp.txt == nothingiseverything


cat modem.wav.txt

HEX TO DEC
303834203038332030353420313037203131352031313320313034203132322031313620303535203039302031313820313134203038352031313320313039

DEC TO ASCII
084083054107115113104122116055090118114085113109

RESULT:
TS6ksqhzt7ZvrUqm
```



```
Connecting to IRC on the /motd we got:

* - irc.mbr.local Message of the Day - 
* - 27/3/2019 16:40
* - Welcome to the Internet Relay Chat Server!!
* - This is the last part of the string: KLBioykc7vK8rEso
```


```
STRING: 
(1/4) GOPHER Server
(2/4) modem.wav Xio Stego
(3/4) Email
(4/4) IRC


TS6ksqhzt7ZvrUqm Sgbt+inVGiMo4418 KLBioykc7vK8rEso
```
