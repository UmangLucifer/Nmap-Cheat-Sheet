<H1># Nmap-Cheat-Sheet</H1>

<h2>Nmap Target</h2>
<b>Scan a single IP</b>	- nmap 192.168.1.1<br>
<b>Scan a hostname</b>	- 	nmap www.domain.com<br>
<b>Scan an IP range</b>	- 	nmap 192.168.1.1-100<br>
<b>Scan a subnet</b>	- 	nmap 192.168.1.0/24<br>
<b>Scan from a predefined list</b>	- 	nmap -iL list.txt<br>

<h2>Nmap Ports</h2>
<b>Scan a single port</b>	- 	nmap -p 22 192.168.1.1<br>
<b>Scan a range of ports</b>	- 	nmap -p 1-20 192.168.1.1<br>
<b>Scan multiple ports</b>	- 	nmap -p 22,80,443 192.168.1.1<br>
<b>Scan Mixed TCP/UDP ports</b>	- 	nmap -p U:53,T:22 192.168.1.1<br>
<b>Scan 100 common ports</b>	- 	nmap -F 192.168.1.1<br>
<b>Scan top # ports</b>	- 	nmap –top-ports <No> 192.168.1.1<br>
<b>Scan ports linearly</b>	- 	nmap -r -p 1-1000 192.168.1.1<br>
<b>Scan all ports</b>	- 	nmap -p- 192.168.1.1<br>

<h2>Nmap Scan</h2>
<b>TCP Connect Scan</b>	- 	nmap -sT 192.168.1.1<br>
<b>TCP SYN scan (Silent scan)</b>	- 	nmap -sS 192.168.1.1<br>
<b>UDP scan</b>	- 	nmap -sU -p 137,139 192.168.1.1<br>
<b>No ping scan</b>	- 	nmap -Pn 192.168.1.1<br>
<b>Host Discovery (no ports)</b>	- 	nmap -sn 192.168.1.1<br>
<b>Version Scan</b>	- 	nmap -sV 192.168.1.1<br>
<b>OS Detection</b>	- 	nmap -o 192.168.1.1<br>
<b>Aggressive service discovery</b>	- 	nmap -sV –version-intensity 5 192.168.1.1<br>
<b>Light banner grabbing</b>	- 	nmap -sV –version-intensity 0 192.168.1.1<br>

<h2>Nmap Scan Time</h2>
<b>Paranoid: Very slow</b>	- 	nmap -t0 192.168.1.1<br>
<b>Sneaky: Quite slow</b>	- 	nmap -t1 192.168.1.1<br>
<b>Polite: Slows down</b>	- 	nmap -t2 192.168.1.1<br>
<b>Normal: Default</b>	- 	nmap -t3 192.168.1.1<br>
<b>Aggressive: Fast and reliable</b>	- 	nmap -t4 192.168.1.1<br>
<b>Insane: Very aggressive</b>	- 	nmap -t5 192.168.1.1<br>

<h2>Nmap Scan Output Format</h2>
<b>Standard Nmap output</b>	- 	nmap -oN output.txt 192.168.1.1<br>
<b>XML format</b>	- 	nmap -oX output.txt 192.168.1.1<br>
<b>All formats output</b>	- 	nmap -oA output.txt 192.168.1.1<br>

<h2>Nmap Scan Script</h2>
<b>Default scripts</b>	- 	nmap -sV -sC 192.168.1.1<br>
<b>Script help</b>	- 	nmap –script-help=ssl-heartbleed<br>
<b>custom</b>	- 	nmap –script-help=scriptname<br>

<h2>Nmap Scan Triest</h2>
<b>retransmissions</b>	- 	–max-retries <tries><br>
<b>Give up on target after time</b>	- 	–host-timeout <time><br>
<b>Adjust delay between probes</b>	- 	–scan-delay/–max-scan-delay <time><br>
<b>Send packets no slower</b>	- 	–min-rate <number><br>
<b>Custom</b>	- 	–max-rate <number><br>


