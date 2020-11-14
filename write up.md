EZ CTF


[Task 1] Nmap

command : nmap IP-Address

Starting Nmap 7.80 ( https://nmap.org ) at 2020-11-14 22:36 WIB
Nmap scan report for 10.10.255.253
Host is up (0.20s latency).
Not shown: 998 closed ports
PORT   STATE SERVICE
22/tcp open  ssh
80/tcp open  http

Nmap done: 1 IP address (1 host up) scanned in 41.02 seconds


1. How many ports are open ?
	2

2. What is the title of the running web server ?
	Violet Evergarden!!!!

3. What is ssh port ?
	22


[Task 2] GoBuster

command : gobuster -u 10.10.255.253 -w /home/rafito/Documents/wordlist/directory-list-2.3-medium.txt -x txt -t 100

/robots.txt (Status: 200)
Progress: 2147 / 220561 (0.97%)^C


1. Run gobuster

2. How to find a txt format ?
	-x txt

3. What is the secret directory ?
	/robots.txt

4. Lets check out the secret directory


[Task 3] SSH

1. What is the SSH username ?
	violet

2. What is the SSH password ?
	00110011011101100110010101110010011001110100000001110010011001000011001101101110 
	(this is binary code, so you should decode it)
	this is the answer : 3verg@rd3n

3.What is the user.txt flag ?
	THM{daosdnc4123o41o32k234n5v234}
	

[Task 4] Steganography

1. What is the full path to .jpg file ?
	/home/violet/Document

2. Download .jpg file to your computer

3. Extract the .jpg file

4. What is the root password ? 
	vybirlbh
	(this is a rot13 code, decode it)
	real answer : iloveyou


[Task 5] Finale

1. What is the root.txt ?
	THM{asdf9sf80dg9asdf8ae0fa8f}


[Task 6] Bonus

1. Who is the author of message.txt ?
	r4f
	(It's located in .cred on root directory)
