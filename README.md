# NCL Tools and Tips
This repository exists to collect techniques and tools for competing in the [National Cyber League](https://nationalcyberleague.org/) competition.

To that end, there are a few rules:
1. We don't share specific problems and solutions here - even from the Gym. This is a public forum, and the NCL is a private competition.
1. Don't push commits or PRs to this repository _during_ the competition time periods. That would be [against the rules](https://nationalcyberleague.org/ncl-rules?rq=rules) of non-collaboration.
1. We don't worry too much about organization at first - we can curate it as we go!
<!--- Yes, I know those all say item "1". Markdown will "do the right thing" here and turn it into a numbered list. --->

# General Commands
ls -a
    - This will show all files (including hidden files) in the given directory

tar xvf <file_name>
    - This will extract a tar file

# General Tools
binwalk
    - This tool can be used to walk a binary and extract files

johnTheRipper
    - This tool is used for password cracking

hashcat
    - This tool is used for password cracking

# Section-specific tools

<!--- NOTE: You can make relative references in hyperlinks and Github will point them locally! --->
* Open Source Intelligence
* [Cryptography](section-cryptography.md)
* [Password Cracking](section-password-cracking.md)
* [Log Analysis](section-log-analysis.md)
* [Network Traffic Analysis](section-network-analysis.md)
* [Wireless Access Exploitation](section-wireless.md)
* [Forensics](section-forensics.md)
* [Scanning](section-scanning.md)
* [Web Application Exploitation](section-web-apps.md)
* [Enumeration & Exploitation](section-enum-and-exploit.md)

# Extra Information
- The shellshock vulnerablility uses command injection. Try looking for "bash" in a file if you are trying to see if someone tried to use it.

- In Hexidecimal, 1 byte is represented as two characters

- When cracking passwords, if a key is given it has a good chance of being a Vigenère cipher.

# Random Links
    ---Image Metadata Viewer---
    http://exif.regex.info/exif.cgi

    ---Beginners CTF Guide: Finding Hidden Data in Images---
    https://infosecwriteups.com/beginners-ctf-guide-finding-hidden-data-in-images-e3be9e34ae0d

    ---Cipher Identifier    NOTE:Struggles to identify Rail Fence Ciphers---
    https://www.boxentriq.com/code-breaking/cipher-identifier

    ---Caeser Cipher Decoder---
    https://cryptii.com/pipes/caesar-cipher-decoder

    ---Atbash Cipher Decoder---
    http://rumkin.com/tools/cipher/atbash.php

    ---Morse Code Translator---
    https://morsedecoder.com/

    ---Rail Fense Cipher Decoder---
    https://planetcalc.com/6947/

    ---MD5 File Checksum---
    https://emn178.github.io/online-tools/md5_checksum.html

    ---Egyptian Hieroglyphic Typewriter---
    https://discoveringegypt.com/egyptian-hieroglyphic-writing/hieroglyphic-typewriter/

    ---MD5 Decrypt---
    https://md5decrypt.net/en/#answer

    ---Futurama Alien Language Decoder---
    http://www.gotfuturama.com/Interactive/AlienCodec/

    ---Intro to SQL---
    https://www.khanacademy.org/computing/computer-programming/sql

    ---Online Python Debugger---
    https://www.onlinegdb.com/online_python_debugger

    ---DNS Cyber Skyline 2021---
    https://www.youtube.com/watch?v=FFFLW7nBzpk&t=89s

    ---Networking Cyber Skyline---
    https://trove.cyberskyline.com/computer-fundamentals-for-cybersecurity/networking

    ---Log Analysis NCL 2021---
    https://www.youtube.com/watch?v=m4s3HJkIR1w&t=80s

    ---Unix Timestamp Converter---
    https://www.epochconverter.com/

    ---Basics of HTTP---
    https://developer.mozilla.org/en-US/docs/Web/HTTP/Basics_of_HTTP

    ---Reverse Engineering NCL---
    https://www.youtube.com/watch?v=70grYjg3fuE&t=50s

    ---Hexadecimal to Decimal---
    https://www.rapidtables.com/convert/number/hex-to-decimal.html

    ---Base 64 Decoder---
    https://www.base64decode.org/

    ---Wired Equivalent Privacy---
    https://en.wikipedia.org/wiki/Wired_Equivalent_Privacy#Encryption_details

    ---HTTP headers---
    https://developer.mozilla.org/en-US/docs/Web/HTTP/Headers

    ---2018 NCL Gym – Enumeration And Exploitation---
    https://palomarinfosec.github.io/Presentations/ExploitationGuide.pdf

    ---Ultimate SQL Injection Cheatsheet---
    https://www.hackingloops.com/sql-injection-cheat-sheet/

    ---Cyber Sky Line: Analyzing FTP Traffic---
    https://www.youtube.com/watch?v=qgM-HLy8BJk&t=5s

    ---Cyber Skyline SQL Basics---
    https://www.youtube.com/watch?v=qrnLPhVHNBc&t=102s