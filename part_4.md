                                                              
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




```
