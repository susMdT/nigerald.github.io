---
title: Hack The Box: Love
permalink: /HTB/Love
---
# Love Writeup 
Love is an easy level box on HackTheBox and took quite some time for me to solve as it was the second box that I have tried to solve. It was pretty interesting to solve and I learned some new exploit methods that I could try to use later.

# Walkthrough
First I performed an nmap scan using `nmap -p- <box ip>`. This first identifies the ports in use. You can follow this up with `nmap -sV -sC -A --script=vuln <box ip> -p x,y,z > file.txt` to get a more indepth scan of those running ports and the system itself, but I was too lazy to do that. This second command will also write the results of the scan to a `file.txt` in your current directory so you could reference the scan again later, if necessary. The result of my initial nmap scan showed me that http was running:
![Image](https://github.com/susMdT/nigerald.github.io/blob/gh-pages/images/love%20(1).png)
