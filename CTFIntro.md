# Introduction - Beginner’s Guide

**CTF for Newbs**

*by @thvl3*

*Apr 30, 2025*

---

## Overview

This corny little guide will help you succeed in your very first CTF, brought to you by PicoCTF and the BYU-I Society of Cybersecurity. We'll cover everything from getting registered on the PicoCTF platform to understanding common challenge types and finding the right tools.


## **NOTICE**

**Before you ask for help on a challenge, please either consult this guide or google. The goal is to teach you how to teach yourself using the materials you are provided.** 

---

## Objectives

By the end of this document, you should understand how to:
* Interact with PicoCTF as a platform.
* Register for PicoCTF and join specific events or classrooms.
* Approach and interact with different types of challenges.
* Access the tools and resources you need to thrive in CTFs.

---

## Target audience

This manual is for CTF first-timers. No prior cybersecurity experience is assumed!

---

## Prerequisites

The ability to read, a willingness to learn, and a laptop with an internet connection and a web browser.

---

# Getting started

## Overview

This guide provides a structured introduction to Capture The Flag competitions, specifically using the PicoCTF platform. We will cover platform navigation, fundamental cybersecurity concepts encountered in CTFs, essential tools, and resources for further learning. The goal is to equip you with the basic knowledge and confidence to participate in your first CTF event.

## Structure

The training follows this guide. It combines:
1.  **Theoretical Learning:** Reading through this guide to understand concepts, terminology, and platform usage.
2.  **Practical Application:** Hands-on practice within the PicoCTF platform, solving introductory challenges. We encourage you to follow along and try things out as you read.

## Duration

* **Reading this Guide:** Approximately 10 minutes.
* **PicoCTF Registration & Familiarization:** 10 minutes.
* **Initial Challenge Practice:** 1-3 hours (variable, depending on your pace).
* **Total Estimated Time:** 2-3 hours to get comfortable with the basics.

## Delivery method

* **Written Materials:** This guide serves as your primary reference.
* **Experiential Learning:** Direct interaction with the PicoCTF website and challenges.
* **Self-Paced:** You can work through the material and practice at your own speed.

## Importance & relevance

CTFs are a fun and engaging way to learn practical cybersecurity skills. They simulate real-world scenarios and challenge you to think critically and creatively. Participating in CTFs like PicoCTF helps build foundational knowledge in areas like web security, cryptography, forensics, and more, which are valuable for anyone interested in technology or cybersecurity careers. Plus, they're a great way to test your problem-solving abilities!

## Basic concepts & terminology

Understanding these terms will help you navigate the CTF landscape:

| Term or concept         | Definition or explanation                                                                                                |
| :---------------------- | :----------------------------------------------------------------------------------------------------------------------- |
| **CTF** | Capture The Flag. A cybersecurity competition where participants solve challenges to find hidden "flags."                  |
| **Flag** | A secret string of text hidden within a challenge. Submitting the correct flag earns points. Flags often look like `picoCTF{s0m3_t3xt_h3r3}`. |
| **Challenge (Chal)** | A specific problem or task to solve in order to find a flag.                                                             |
| **Category** | Challenges are usually grouped by type, such as Web Exploitation, Cryptography, Forensics, Reverse Engineering, Binary Exploitation (Pwn). |
| **PicoCTF** | A popular, free online CTF platform designed for beginners, especially middle and high school students, but great for all ages. |
| **Shell / Terminal** | A command-line interface used to interact with operating systems (like Linux). Essential for many challenges.              |
| **Web Developer Tools** | Tools built into web browsers (like Chrome DevTools) used to inspect website code (HTML, CSS, JavaScript) and network traffic. Often crucial for Web Exploitation challenges. |
| **Encoding/Decoding** | Converting data between different formats (e.g., Base64, Hexadecimal, ASCII). Not encryption, but often used to obscure data. |
| **Encryption/Decryption** | Transforming data using a key to make it unreadable without the key (e.g., Caesar cipher, AES). Key concept in Cryptography. |
| **Steganography** | Hiding data within other data, like concealing a message inside an image file. Common in Forensics.                     |
| **Reverse Engineering** | Analyzing compiled software (an executable file) to understand how it works without having the source code.             |
| **Binary Exploitation (Pwn)** | Finding vulnerabilities in compiled programs (binaries) and exploiting them to gain control or access hidden information. |
| **Write-up** | A detailed explanation of how a CTF challenge was solved, often published after a competition ends. Great for learning. |

---

# Issue resolution

## Common problems & solutions

Beginners often encounter similar hurdles. Here’s how to approach them:

| Common problem                                     | Suggested Approach                                                                                                                                                                                             |
| :------------------------------------------------- | :------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **"I don't know where to start on a challenge."** | 1. **Read the prompt carefully:** Look for keywords, hints, and the challenge category. <br> 2. **Examine provided files/links:** Download any files, visit any websites. Use basic tools (like `file` command, browser DevTools). <br> 3. **Check the hints:** PicoCTF challenges often have hints available (sometimes costing points). <br> 4. **Google is your friend:** Search for terms, techniques, or tools related to the category or prompt. <br> 5. **Try simple things first:** Is it basic encoding? Is the flag hidden in the web page source? |
| **"My command/tool isn't working."** | 1. **Check syntax:** Did you type the command correctly? Are the arguments right? <br> 2. **Check installation:** Is the tool installed? (e.g., `python --version`, `nc -h`). <br> 3. **Read documentation/help:** Use `man <command>` or `<tool> --help` to understand usage. <br> 4. **Permissions?** Do you need `sudo`? Are file permissions correct (`chmod`)? <br> 5. **Network issues?** If connecting to a remote service, is the host/port correct? Is your network connection stable? |
| **"I found something, but it's not the flag."** | 1. **Check flag format:** Does it look like `picoCTF{...}`? Flags usually have a specific prefix and curly braces. <br> 2. **Keep digging:** What you found might be an intermediate step or a piece of the puzzle, not the final flag. <br> 3. **Re-read the prompt:** Did you miss a constraint or detail about what the flag represents?                                                                                                  |
| **"The website/service for the challenge is down."** | 1. **Wait a bit:** Sometimes services are temporarily overloaded or reset. <br> 2. **Check official channels:** Look at the PicoCTF platform announcements or Discord (if available) for status updates. <br> 3. **Try later:** If it persists, move to another challenge and come back.                                                                                                           |

## Error messages

While PicoCTF itself doesn't show many "error codes," the tools you use will. Instead of a list, here’s a strategy:
1.  **Read the error message carefully:** It often tells you exactly what's wrong (e.g., "File not found," "Connection refused," "Syntax error").
2.  **Copy and paste the error message into a search engine:** Chances are someone else has encountered the same error. Look for explanations on sites like Stack Overflow or forums related to the tool.
3.  **Isolate the problem:** Simplify your command or code. Does a simpler version work? Gradually add complexity back until the error reappears.

---

# Basic & Advanced Operations (Challenge Categories)

## Basic Operations: Interacting with PicoCTF

| Common Task                                | Steps                                                                                                                                                                                                                                                           |
| :----------------------------------------- | :-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **Registering & Logging In** | 1. Go to the PicoCTF website (e.g., `picoctf.org`). <br> 2. Click "Register" and create an account. <br> 3. Log in with your credentials. <br> 4. If joining a specific event/classroom, find the "Join" or "Enroll" section and enter the provided code.             |
| **Accessing Challenges** | 1. Navigate to the "Game" or "Challenges" section. <br> 2. Challenges are usually listed by category. <br> 3. Click on a challenge title to view the description, any provided files/links, point value, and hints.                                                    |
| **Downloading Challenge Files** | 1. Click the link for the file provided in the challenge description. <br> 2. Save the file to your computer, preferably in an organized folder for the specific challenge.                                                                                       |
| **Connecting to Remote Services (Netcat)** | 1. Many challenges provide a host and port (e.g., `saturn.picoctf.net 12345`). <br> 2. Open your terminal/shell. <br> 3. Use the `nc` (netcat) command: `nc saturn.picoctf.net 12345`. <br> 4. Interact with the service as required by the challenge.                 |
| **Using the PicoShell (Web Shell)** | 1. PicoCTF often provides a web-based Linux shell. Find the "Shell" or "PicoShell" link. <br> 2. Use this terminal to run basic Linux commands (`ls`, `cd`, `cat`, `grep`), download files (`wget`), run scripts (`python`), etc., without needing a local Linux setup. |
| **Submitting Flags** | 1. Once you find the flag (e.g., `picoCTF{y0u_f0und_m3}`), copy it. <br> 2. Go back to the challenge page on the PicoCTF website. <br> 3. Paste the flag into the submission box. <br> 4. Click "Submit". You'll get immediate feedback if it's correct.             |

## Tips & Shortcuts

1.  **Learn Basic Linux Commands:** `ls`, `cd`, `cat`, `grep`, `wget`, `chmod`, `file`, `strings` are invaluable. Use the PicoShell or install WSL/use a Linux VM.
2.  **Master Browser DevTools:** Right-click -> Inspect Element. Explore the HTML source, CSS styles, JavaScript console, and Network tabs. Essential for web challenges.
3.  **Use CyberChef:** An incredibly useful web app for encoding/decoding, encryption/decryption, and data manipulation. Drag and drop "recipes" to transform data.
4.  **Take Notes:** Keep track of what you've tried for each challenge, useful commands, and potential leads.
5.  **Read Write-ups (After Trying!):** If you get stuck, look for write-ups *after* the competition ends or *after* you've genuinely tried. They are excellent learning tools.

---

## Common Challenge Categories (Formerly "Advanced Operations")

Understanding the types of challenges helps you know which tools and techniques to apply.

| Category                 | Description & Common Techniques                                                                                                                                                                                                                            | Common Tools                                                                                                                                                              |
| :----------------------- | :--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | :------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| **Web Exploitation** | Finding vulnerabilities in websites. Look for issues in HTML, CSS, JavaScript. Check cookies, headers, forms. Common vulns: SQL Injection (SQLi), Cross-Site Scripting (XSS), Directory Traversal, Inspecting Source Code, Robots.txt.                         | Browser DevTools (Inspect Element, Console, Network), `curl`, `wget`, Burp Suite (Proxy), SQLMap, CyberChef                                                              |
| **Cryptography (Crypto)**| Breaking or manipulating encryption/ciphers. Identify the cipher type (Caesar, Vigenere, Substitution, XOR, RSA, AES). Look for weak keys, implementation flaws, or frequency analysis clues. Often involves encoding (Base64, Hex, Binary).                | Pen-and-paper, Python scripting, CyberChef, Online cipher identifiers (e.g., Boxentriq, dCode), `openssl` command-line tool, RsaCtfTool                                     |
| **Forensics** | Analyzing files or data dumps to find hidden information. Examine file metadata (EXIF), hidden data in images/audio (steganography), network traffic captures (.pcap files), memory dumps, disk images.                                                    | `file`, `strings`, `exiftool`, `binwalk`, `steghide`, `zsteg`, Audacity (for audio), Wireshark (for .pcap), Volatility (memory forensics), Autopsy/FTK Imager (disk forensics) |
| **Reverse Engineering (RE)** | Understanding how a program works without source code, usually by analyzing its compiled form (executable). Disassemble or decompile the binary. Analyze assembly code or pseudo-code to find logic flaws or hidden flags.                             | `file`, `strings`, `ltrace`, `strace`, Ghidra, IDA Pro (paid), radare2, Binary Ninja (paid), GDB (debugger)                                                              |
| **Binary Exploitation (Pwn)** | Finding memory corruption vulnerabilities (e.g., buffer overflows, format string bugs) in programs and exploiting them to gain control of the program's execution, often to get a shell or leak the flag. Usually involves C programs on Linux. | Python (especially `pwntools` library), GDB (debugger), Ghidra/IDA Pro, `checksec`, `nc` (netcat)                                                                        |
| **General Skills** | Miscellaneous challenges that might involve scripting, logic puzzles, trivia, or using various command-line tools.                                                                                                                                       | Linux command line tools (`grep`, `sed`, `awk`, `find`), Python/Bash scripting, Google Search                                                                           |

## Best practices

1.  **Stay Ethical:** Only target the systems and services explicitly provided for the CTF. Do not attack the CTF platform itself or other players.
2.  **Read Carefully:** Pay close attention to challenge descriptions, hints, and any provided materials. Details matter.
3.  **Be Systematic:** Don't just randomly try things. Form hypotheses based on the category and evidence, then test them.
4.  **Learn Your Tools:** Spend time understanding how basic tools work (Linux commands, DevTools, CyberChef).
5.  **Don't Give Up Easily:** CTFs require persistence. If one approach doesn't work, try another. Take breaks when frustrated.
6.  **Collaborate (If Allowed):** Some CTFs are team events. Learn to communicate and share findings effectively. For PicoCTF, check the specific event rules.
7.  **Have Fun and Learn:** The primary goal is to learn new skills and enjoy the process of problem-solving.

*(The "Customization options" section from the template is not directly applicable to CTFs and has been removed.)*

---

# Conclusion

## Summary of key points

1.  **CTFs are learning games:** They challenge you to solve cybersecurity puzzles to find hidden "flags."
2.  **PicoCTF is beginner-friendly:** It provides a platform with diverse challenges suited for newcomers.
3.  **Master the basics:** Learn fundamental Linux commands, browser DevTools, and concepts like encoding/encryption.
4.  **Understand categories:** Knowing the common challenge types (Web, Crypto, Forensics, RE, Pwn) helps guide your approach.
5.  **Persistence and resources are key:** Use hints, search engines, tools like CyberChef, and don't be afraid to struggle – it's part of learning!

## Closing remarks

Welcome to the exciting world of CTFs! This guide has hopefully given you the foundation and confidence to dive into PicoCTF. Remember that everyone starts somewhere, and the cybersecurity field is vast. Be patient with yourself, celebrate small victories, learn from challenges you can't solve, and most importantly, have fun exploring and learning! Good luck!

## Contact information

If you have questions or need help specifically related to the BYU-I Society of Cybersecurity activities or this guide:

| Role or department               | Person / Contact                                  |
| :------------------------------- | :------------------------------------------------ |
| Society President/Red Team Guy | [Ethan Hulse @thule]          |
| Blue Team and Forensics        | [Edidiong Ekpe @dark3v3]      |
| Network and AD Red Team Guy    | [Connor Dedic @enigma3nma]    |


---


---

# Resources

## Additional reading materials

* **CTF Field Guide:** [https://trailofbits.github.io/ctf/](https://trailofbits.github.io/ctf/) (Comprehensive guide by Trail of Bits)
* **OWASP Top 10:** [https://owasp.org/www-project-top-ten/](https://owasp.org/www-project-top-ten/) (Understand common web vulnerabilities)

## Online tutorials & Tools

* **PicoCTF Resources:** Check their website for past problems and learning resources.
* **CyberChef:** [https://gchq.github.io/CyberChef/](https://gchq.github.io/CyberChef/) (Essential for data manipulation)
* **OverTheWire Wargames:** [https://overthewire.org/wargames/](https://overthewire.org/wargames/) (Practice Linux command line and security concepts)
* **TryHackMe:** [https://tryhackme.com/](https://tryhackme.com/) (Hands-on cybersecurity training rooms)
* **Hack The Box:** [https://www.hackthebox.com/](https://www.hackthebox.com/) (More advanced penetration testing labs)

## Community forums

* **BYU-I Society of Cybersecurity:** [https://discord.gg/KBjkfHKqnm]
* **Reddit:** r/cybersecurity, r/netsecstudents, r/securityCTF
