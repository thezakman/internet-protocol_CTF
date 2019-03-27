                                                              
```
  ___ _  _ _____ ___ ___ _  _ ___ _____   ___ ___  ___ _____ ___   ___ ___  _    
 |_ _| \| |_   _| __| _ \ \| | __|_   _| | _ \ _ \/ _ \_   _/ _ \ / __/ _ \| |   
  | || .` | | | | _||   / .` | _|  | |   |  _/   / (_) || || (_) | (_| (_) | |__ 
 |___|_|\_| |_| |___|_|_\_|\_|___| |_|   |_| |_|_\\___/ |_| \___/ \___\___/|____|
                                                                
                                                                 DATE: 26-03-2019
                                                                 @TheZakMan

 [ URL: http://80.211.167.123/ ]
```


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
23/tcp   open  telnet
| banner: \xFF\xFB\x01\xFF\xFB\x03\xFF\xFD\x18\xFF\xFD\x00\x1B[?1000h\x0C
|_Mystic BBS v1.12 A43 for Windows Node 1\x0D\x0ACopyright (C) 1997-20...
| fingerprint-strings: 
|   GenericLines, GetRequest, Help, NULL, RPCCheck, tn3270: 
|     [?1000h
|     Mystic BBS v1.12 A43 for Windows Node 1
|     Copyright (C) 1997-2019 By James Coyle
|     Detecting terminal emulation: 
|     [6nASCII detected.
|     Ascii (No Color)
|     Ansi (Color)
|_    Graphics Mode ->
70/tcp   open  gopher
| fingerprint-strings: 
|   GenericLines: 
|     Iimage.png /image.png 80.211.167.123 70
|     0welcome.txt /welcome.txt 80.211.167.123 70
|   GetRequest: 
|     HTTP/1.1 400 Bad request
|     Content-Type: text/html; charset=UTF-8
|     Server: Motsognir/0.99
|     Connection: close
|     <!DOCTYPE HTML PUBLIC "-//W3C//DTD HTML 4.01//EN" "http://www.w3.org/TR/html4/strict.dtd">
|     <html>
|     <head>
|     <title>400 - Bad request</title>
|     <meta name="generator" content="Motsognir v0.99">
|     </head>
|     <body>
|     style="font-size: 1.3em; margin: 1em 1em 1em 1em; text-align: left; font-weight: bold;">400 - BAD REQUEST</p>
|     style="font-size: 1.1em; margin: 1em 1em 1em 1em; text-align: left;">Your request is not admissible. Sorry. This is a gopher server, which means that you have to use the gopher protocol to access it. Right now, you used the HTTP protocol instead.</p>
|     style="text-align: center;"><a href="gopher://80.211.167.123/" style="font-size: 1.15em;">Click here to access this server using the gopher protocol.</a></p>
|     </body>
|_    </html>
80/tcp   open  http    Microsoft IIS httpd 10.0
|_http-server-header: Microsoft-IIS/10.0
110/tcp  open  pop3    hMailServer pop3d
| banner: +OK 01010111 01100101 01101100 01100011 01101111 01101101 01100
|_101 00100000 01110100 01101111 00100000 01110100 01101000 01100101 0...
6667/tcp open  irc     ircu ircd
2 services unrecognized despite returning data. If you know the service/version, please submit the following fingerprints at https://nmap.org/cgi-bin/submit.cgi?new-service :
==============NEXT SERVICE FINGERPRINT (SUBMIT INDIVIDUALLY)==============
SF-Port23-TCP:V=7.70%I=7%D=3/26%Time=5C9AB947%P=x86_64-pc-linux-gnu%r(NULL
SF:,D9,"\xff\xfb\x01\xff\xfb\x03\xff\xfd\x18\xff\xfd\0\x1b\[\?1000h\x0cMys
SF:tic\x20BBS\x20v1\.12\x20A43\x20for\x20Windows\x20Node\x201\r\nCopyright
SF:\x20\(C\)\x201997-2019\x20By\x20James\x20Coyle\r\n\r\nDetecting\x20term
SF:inal\x20emulation:\x20\x1b\[6nASCII\x20detected\.\r\n\r\n\(0\)\x20Ascii
SF:\x20\(No\x20Color\)\r\n\(1\)\x20Ansi\x20\x20\(Color\)\r\n\r\nGraphics\x
SF:20Mode\x20->\x20")%r(GenericLines,D9,"\xff\xfb\x01\xff\xfb\x03\xff\xfd\
SF:x18\xff\xfd\0\x1b\[\?1000h\x0cMystic\x20BBS\x20v1\.12\x20A43\x20for\x20
SF:Windows\x20Node\x201\r\nCopyright\x20\(C\)\x201997-2019\x20By\x20James\
SF:x20Coyle\r\n\r\nDetecting\x20terminal\x20emulation:\x20\x1b\[6nASCII\x2
SF:0detected\.\r\n\r\n\(0\)\x20Ascii\x20\(No\x20Color\)\r\n\(1\)\x20Ansi\x
SF:20\x20\(Color\)\r\n\r\nGraphics\x20Mode\x20->\x20")%r(tn3270,E5,"\xff\x
SF:fb\x01\xff\xfb\x03\xff\xfd\x18\xff\xfd\0\x1b\[\?1000h\xff\xfa\x18\x01\x
SF:ff\xf0\xff\xfe\x19\xff\xfc\x19\x0cMystic\x20BBS\x20v1\.12\x20A43\x20for
SF:\x20Windows\x20Node\x201\r\nCopyright\x20\(C\)\x201997-2019\x20By\x20Ja
SF:mes\x20Coyle\r\n\r\nDetecting\x20terminal\x20emulation:\x20\x1b\[6nASCI
SF:I\x20detected\.\r\n\r\n\(0\)\x20Ascii\x20\(No\x20Color\)\r\n\(1\)\x20An
SF:si\x20\x20\(Color\)\r\n\r\nGraphics\x20Mode\x20->\x20")%r(GetRequest,D9
SF:,"\xff\xfb\x01\xff\xfb\x03\xff\xfd\x18\xff\xfd\0\x1b\[\?1000h\x0cMystic
SF:\x20BBS\x20v1\.12\x20A43\x20for\x20Windows\x20Node\x201\r\nCopyright\x2
SF:0\(C\)\x201997-2019\x20By\x20James\x20Coyle\r\n\r\nDetecting\x20termina
SF:l\x20emulation:\x20\x1b\[6nASCII\x20detected\.\r\n\r\n\(0\)\x20Ascii\x2
SF:0\(No\x20Color\)\r\n\(1\)\x20Ansi\x20\x20\(Color\)\r\n\r\nGraphics\x20M
SF:ode\x20->\x20")%r(RPCCheck,D9,"\xff\xfb\x01\xff\xfb\x03\xff\xfd\x18\xff
SF:\xfd\0\x1b\[\?1000h\x0cMystic\x20BBS\x20v1\.12\x20A43\x20for\x20Windows
SF:\x20Node\x201\r\nCopyright\x20\(C\)\x201997-2019\x20By\x20James\x20Coyl
SF:e\r\n\r\nDetecting\x20terminal\x20emulation:\x20\x1b\[6nASCII\x20detect
SF:ed\.\r\n\r\n\(0\)\x20Ascii\x20\(No\x20Color\)\r\n\(1\)\x20Ansi\x20\x20\
SF:(Color\)\r\n\r\nGraphics\x20Mode\x20->\x20")%r(Help,D9,"\xff\xfb\x01\xf
SF:f\xfb\x03\xff\xfd\x18\xff\xfd\0\x1b\[\?1000h\x0cMystic\x20BBS\x20v1\.12
SF:\x20A43\x20for\x20Windows\x20Node\x201\r\nCopyright\x20\(C\)\x201997-20
SF:19\x20By\x20James\x20Coyle\r\n\r\nDetecting\x20terminal\x20emulation:\x
SF:20\x1b\[6nASCII\x20detected\.\r\n\r\n\(0\)\x20Ascii\x20\(No\x20Color\)\
SF:r\n\(1\)\x20Ansi\x20\x20\(Color\)\r\n\r\nGraphics\x20Mode\x20->\x20");
==============NEXT SERVICE FINGERPRINT (SUBMIT INDIVIDUALLY)==============
SF-Port70-TCP:V=7.70%I=7%D=3/26%Time=5C9AB948%P=x86_64-pc-linux-gnu%r(GetR
SF:equest,382,"HTTP/1\.1\x20400\x20Bad\x20request\r\nContent-Type:\x20text
SF:/html;\x20charset=UTF-8\r\nServer:\x20Motsognir/0\.99\r\nConnection:\x2
SF:0close\r\n\r\n<!DOCTYPE\x20HTML\x20PUBLIC\x20\"-//W3C//DTD\x20HTML\x204
SF:\.01//EN\"\x20\"http://www\.w3\.org/TR/html4/strict\.dtd\">\r\n<html>\r
SF:\n\x20\x20<head>\r\n\x20\x20\x20\x20<title>400\x20-\x20Bad\x20request</
SF:title>\r\n\x20\x20\x20\x20<meta\x20name=\"generator\"\x20content=\"Mots
SF:ognir\x20v0\.99\">\r\n\x20\x20</head>\r\n\x20\x20<body>\r\n\x20\x20\x20
SF:\x20<p\x20style=\"font-size:\x201\.3em;\x20margin:\x201em\x201em\x201em
SF:\x201em;\x20text-align:\x20left;\x20font-weight:\x20bold;\">400\x20-\x2
SF:0BAD\x20REQUEST</p>\r\n\x20\x20\x20\x20<p\x20style=\"font-size:\x201\.1
SF:em;\x20margin:\x201em\x201em\x201em\x201em;\x20text-align:\x20left;\">Y
SF:our\x20request\x20is\x20not\x20admissible\.\x20Sorry\.\x20This\x20is\x2
SF:0a\x20gopher\x20server,\x20which\x20means\x20that\x20you\x20have\x20to\
SF:x20use\x20the\x20gopher\x20protocol\x20to\x20access\x20it\.\x20Right\x2
SF:0now,\x20you\x20used\x20the\x20HTTP\x20protocol\x20instead\.</p>\r\n\x2
SF:0\x20\x20\x20<p\x20style=\"text-align:\x20center;\"><a\x20href=\"gopher
SF:://80\.211\.167\.123/\"\x20style=\"font-size:\x201\.15em;\">Click\x20he
SF:re\x20to\x20access\x20this\x20server\x20using\x20the\x20gopher\x20proto
SF:col\.</a></p>\r\n\x20\x20</body>\r\n</html>\r\n")%r(GenericLines,59,"Ii
SF:mage\.png\t/image\.png\t80\.211\.167\.123\t70\r\n0welcome\.txt\t/welcom
SF:e\.txt\t80\.211\.167\.123\t70\r\n\.\r\n");
Service Info: Host: irc.mbr.local; OS: Windows; CPE: cpe:/o:microsoft:windows





https://en.wikipedia.org/wiki/Gopher_(protocol)

Because of the simplicity of the Gopher protocol, tools such as netcat make it possible to download Gopher content easily from the command line:
echo jacks/jack.exe | nc gopher.example.org 70 > jack.exe


echo /welcome.txt | nc 80.211.167.123 70 > welcome.txt
echo /image.png | nc 80.211.167.123 70 > image.png



[POP3]
nc 80.211.167.123 110
+OK 
01010111 01100101 01101100 01100011 01101111 01101101 01100101 00100000 01110100 01101111 00100000 01110100 01101000 01100101 00100000 01110000 01101111 01110000 00110011 00100000 01110011 01100101 01110010 01110110 01100101 01110010 00101110 00100000 01011001 01101111 01110101 00100000 01100011 01100001 01101110 00100000 01100011 01101000 01100101 01100011 01101011 00100000 01111001 01101111 01110101 01110010 00100000 01101001 01101110 01100010 01101111 01111000 00100000 01100001 01110100 00100000 01110101 01110011 01100101 01110010 01000000 01101101 01100001 01101001 01101100 00101110 01101100 01101111 01100011 01100001 01101100

Welcome to the pop3 server.  You can check your inbox at user@mail.local
