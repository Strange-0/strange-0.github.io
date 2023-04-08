## Table of Contents

* [Introduction](#introduction)
* [Before Enrollment Preparation](#before-enrollment-preparation)
* [Post Enrollment Preparation](#post-enrollment-preparation)
* [Exam Day](#exam-day)
* [My Overall Methodology and Recommendation](#my-overall-methodology-and-recommendation)
* [Resources for Learning](#resources-for-learning)

# My OSCP Exam Adventure

![](https://miro.medium.com/v2/resize:fit:400/1*6bqjHNQUoFQ17mUv6G7iLw.png)

## Introduction:

As a second-year college student with no prior hacking experience, I was unsure of what I wanted to do in the future. I was searching for different fields to pursue when I came across the Offensive Security Certified Professional (OSCP) certification. Intrigued by the reputation and the exam structure, I was thinking how cool are those guys who had passed it and another thing that attracted me was the certificate and wallet card that offsec gave to the holders at that time (I know its immature but I felt bit sad when i got to know that that i won’t be getting those but still having skill was more important from a career point of view.) So after researching about the field i found different courses and platforms to prepare for oscp. But i wasn’t consistent as i had my college studies too and also i had a habbit of procrastination so time went and after a year my graduation was completed and i had job offer but didn’t want to go for that. So i decided to start preparing for oscp. So oscp is the reason I’m in this field. In this blog post, I will share my journey towards obtaining the OSCP certification, including the challenges I faced, the skills I acquired, and the lessons I learned along the way and i will share every resource that i used to learn and just oscp but in general.

## Before Enrollment Preparation:

Before Enrolling, I completed Practical Ethical Hacking course by TCMsecurity and it was enough to get hang of the things and i was also reading blogs by people on their oscp experience. After that i started with tryhackme to get hands on experience, it is the best platform for beginners. So after some time, i did only around 15 labs on tryhackme. Then i started with TJNull HTB machines for oscp. I was not able to do any machine without looking at walkthrough and kind of demotivated and didn’t have enough confidence and was able to do only around 20 machines including both windows and linux. Then i enrolled on HTB academy for Peneteration Tester path which covered almost every topic oscp had. After doing some important modules i was little confident that now i have what it takes to pass oscp. So after 2.5 months from the day i started preparing for oscp i enrolled for oscp on 2 dec 2022 with learn one subscription as it was on discount during that time.

**My recommendations for pre-enrollment phase :**

-   Practical Ethical Hacking course by TCMsecurity
-   HTB academy Active Directory Enumration Module (all the modules are good but if you only want something to prepare for Active Directory then it is more than enough)
-   Tryhackme for beginner hands on experience
-   TJNull list of oscp like machines HTB (even if you are not able to do them yourself, don’t feel demotivated just learn whatever you can from each and every machine).
-   Read blogs and watch videos by people who has passed the exam.

## Post Enrollment Preparation:

So after enrolling, my plan was to go through videos and look for any new topic and get bonus points in a month by completing 80 % exercises and doing 1 machine a day. But as a wise man once said

> “Nothing ever goes as planned in this accursed world”

As i started study material i didn’t find them useful to me then i moved on to doing exercises which was very tedious task so i skipped that for later and moved to PWK labs directly and i was doing fine for first 20 days even though i was not able to any machine without looking at hints and asking for help on discord but i was learning a lot but then i thought of taking a break (biggest mistake). Taking a break is not bad but it’s important to get back on track but i kind lost touch of that and wasted almost a month doing absolutely nothing (not exaggerating). I just wasn’t able to do anything and left everything to do for later and started thinking that i won’t be able to pass it and had lost of faith in myself that i had at the time of enrollment. Even though i was thinking about doing everyday but i couldn’t get myself to start the system and start doing practice actually and this made me more stressed. On 20 jan 2023 i scheduled my exam for 27 feb 2023 thinking that i might start doing things if i have some kind of pressure of exam being scheduled, it did had a little effect but i still wasn’t giving my best and after a week my system stopped working which gave me a reason to stop and i was back to my lazy schedule. I still remember on feb 18 2023 i started again with strong will of doing but when i started i felt totally blank like i was a beginner, i couldn’t process what i can i do in these 10 days. I was so stressed but still tried doing anything i could, I had already given up on getting bonus points as it was so irritating to start and stop VMs for every topic, i just couldn’t do it. So on 25 feb 2023 before 3 hours of loosing the chance to reschedule the exam, i rescheduled my exam for 6 march 2023 because i was not mentally ready. So in the last week i completed retired machines in labs, wasn’t able to do them without help and cleared my AD and pivoting concepts and i was literally feeling like a looser already.

![](https://miro.medium.com/v2/resize:fit:640/1*SJE_0wS4K3ghKBZtpFtZNQ.gif)

Overview of 3 months:

-   PWK labs — 40
-   Topic exercises — 50 %
-   Clearing Active Directory and pivoting concepts in last week

**My recommendations for Post Enrollment phase :**

-   Get those bonus points if you want to be less stressed during exam.
-   Make sure you are taking notes of everything you are doing in labs or whatever.
-   Join discord and offsec forums to get help and hints.
-   Labs were good but exam machines were bit different and difficult than labs (not that much difficult but a bit).
-   Try a simulation of exam using retired machines in labs, there are total of 5 machines.
-   Make sure you have clear understanding of Active Directory (you only need to have basic knowledge of AD)
-   Rabbit holes is one of the main reason the machines are difficult, beware of them. I didn’t really fell for them so all i can say is just enumerate everything and setup timer for different phases. You need to have that instinct to detect them which will come from practice labs.

I just did one hard machine from pg practice 2 days before the exam day but it was quite straightforward and easy. So i don’t know much about it but many people recommend that too, so you can try it if you want.

## Exam Day:

On exam day i had already thought that i’m going to fail so my plan was to get most of the day and get experience from the machines so that my preparation for second attempt is better. Exam started:

![](https://miro.medium.com/v2/resize:fit:480/1*aG4OgyTBJRFTfLfFWj8lyg.gif)

-   10 AM to 4PM — I started with AD set and got initial foothold in 2 hours and i didn’t take a break and went for privesc and i was able to find privesc easily manually without any tool. Exploited and got system. For the next machine it took a bit of time to get system but i was able to find weakness using a tool [PrivescCheck](https://github.com/itm4n/PrivescCheck). After exploitaing that i got system and then moved to DC and got domain access. It took total of 6 hours to complete AD set (my plan was to complete it in 4 hours). I was not confident in doing the things i did during exam but surprisingly enough i was calm even though i was confused during the AD set of the exam.
-   4:30 PM to 8 PM — After completing AD set i took a break of 30 min and then started doing independent machines. I was able to get initial shell in 1 hour and then privesc took 2 hours including breaks. At this point i was regretting not getting those bonus points because if i had i would already have passing scores.
-   9 PM to 10 PM — Then after having 60 points i need to score only 10 to get passing scores but i wanted to complete every machine. So thinking that way i started doing another machine and was able to get initial foothold in about 1 hour, it was filled with rabbit holes but i was able to go in direction (hacker instinct). At this point i was so happy that i had scored passing points, controlling my emotions i started looking for privesc but i couldn’t so i took a break and ate my dinner and came back at 12 AM after an hour break.
-   12 AM to 3 AM — At this point i was tired but still wanted to complete every machine but before that i started taking screenshots and requirements for report as i don’t want to fail because of incomplete report. So it took me about 3 hours to get screenshots and completely exploiting every machine again while check report requirements.

![](https://miro.medium.com/v2/resize:fit:220/1*GbhFwXjA6ra8ZnmqNT7qfg.gif)

-   3 AM to 8 AM — After that i took a break to sleep but i couldn’t so after an hour i decided to just go on and look for any privesc or initial foothold on last independent machine. As a the time passes by i was getting tired and frustated even though i was able to find vulnerability in last machine for foothold i couldn’t get a shell on that and wasn’t able to privesc on other machine. So after getting tired due to no sleep in 24 hours, i lost the interest to do anymore so i decided to end my exam at 8 AM after checking my reporting and flag submission on panel. Overall i enjoyed the exam.

## Exam Reporting:

After ending my exam i slept whole day and woke up at 7 PM and i had fever and headache that i had during exam too but after waking up it was much more than normal headache so i took medicine (even though i hate medicines). After that i took some rest and started writing my report at 9 PM. When i started it was a shock for me because that was the first time i am writing a report and template that offsec provided had some issue with formatting or i don’t know. It just didn’t work for me. So after checking editing it with different software, i changed the template and used another improved version of it [here](https://github.com/whoisflynn/OSCP-Exam-Report-Template/blob/master/OSCP-OS-XXXXX-Exam-Report_Template.docx).

It was better than official and i could edit it, still not the way i wanted to but it was fine. In my report i explained everything from start to finish how i scanned and exploited anything and what my thought process was during any exploitation and pasted every command i found important to be written. I even included links to configure burp suite with firefox (i don’t know if i overdid it but i didn’t want of fail because of report).

**Reporting Recommendations:**

-   Prepare your report template before the exam so you don’t have to worry about that i like did at the last moment.
-   Explain everything how found the vulnerability and how you exploited it, what exploit you used, link to the exploit , highlight any changes if done, i just mean everything.
-   Include screenshots of flags with ip and other important screenshots that might need to be included.
-   Take screenshots and notes while doing the exam it will be helpful later.

## After i got My Results:

I submitted my report at 5:30 AM on 8 march and was relaxed but still feeling nervous about result as i knew i had scored passing points but still it all depends on my report whether it is good enough according to offsec. On 10 march around 5:50 PM i got my results at first i didn’t want to look at it but i mistakenly clicked it and saw what i wanted to.

![](https://miro.medium.com/v2/resize:fit:700/1*ktkvyXhQ1EbvUZ7PAY5LKQ.png)

![](https://miro.medium.com/v2/resize:fit:496/1*teR37yLxeYCaarenPXPz7g.gif)

## My Overall Methodology and Recommendation:

-   I prefer to do things manually rather then doing any enum with tools.
-   I always start with rustscan to look for open ports and nmap script scan on found ports.
-   If there any port like 80,8080 are open then i will look at them in my browser manually while my script scan is running.
-   If any common ports like 21,135,139,111,25 are open then also i will enumerate manually and will do basic enumeration and when i get stuck i will look for it in my notes or google it.
-   for fuzzing web directories i use ffuf, gobuster most of the time but i can use dirb also and if nothing works i just skip this for some time.
-   Most of the time i just google if any unknown service is running or port is open.
-   If i find an exploit for a service i will look at it and check if i can just do it manually, my coding skills are not good but sometimes i can understand a little what a particular exploit is doing.
-   I prefer not to use any kernel exploits but if i do i make sure that my system matches the exploit version and right now i’m learning about docker so that i can compile exploits easily specially for this purpose.
-   I use python server to serve file and transfer them.
-   For file transfer in windows if powershell is running i mostly just look at my notes accordingly if i want to invoke them directly or store them and then run and other method i use is impacket smbserver. And there is certutil too and nothing else works i will look for more on internet.
-   For file transfer in linux running python server and wget is enough but sometimes wget is not installed so nc can be useful in those times.
-   To find exploits i just google the name and version if available of the service, most of the time i was able to find exploit on first result page.
-   For Pivoting i used chisel which worked really well for me. But in labs i also tried sshuttle which is good too but for exam i would recommend chisel.
-   For windows privesc, i first enumerate manually and look for user privileges, unquoted service path, running servcies, alwayinstalleelevated and if i find nothing then i would use [PrivescCheck](https://github.com/itm4n/PrivescCheck) to look for weakness and winpeas after that. If i don’t find anything then just ask for help.
-   For linux privesc, same i first enumerate manually and look for permissions on password files, cronjobs, sudo privileges, suid binaries, services running as root and if i don’t find anything then i would use LinEnum and linpeas and ask for help at the end.
-   For dumping creds i use mimikatz but crackmapexec can also be used to do the same. sometimes i just copy the sam file on my attack box and use impacket secretsdump to dump creds from files.
-   About reverse shell i use php reverse shell by pentestmonkey mostly but for windows nishang powershellreversetcp is my go to thing. After getting a shell i just run another reverse shell to have a backup shell ready.
-   For upgrading shell in linux you can check my [Notes](https://strange-1.gitbook.io/notes/shells/spawning-a-tty-shell).

At the end i would say the best way to become better is to take notes of whatever you are doing and practice everyday. I was not disciplined enough to do what my initial plan was but i still manage to pass the exam on first attempt, so you can too. I kind of gave too much importance to the exam rather than health but i knew i have the knowledge and skill required to pass the exam and i would say that its good to have passed the exam in first attempt but even if you don’t, it doesn’t mean that you don’t have enough skills or whatever. After submitting the report i felt that i deserve to pass the exam not because i scored required points but because i knew i was able to penetrate systems and find weakness in them. So What matters the most is how good your understanding is about a particular topic. I am still learning daily and will continue to do so as much i want.

And How i feel after passing, i know its just entry level cert but this is my first ever achievement in life so it feels so special. I used to think about those who passed oscp as “Cool guys” and now i am one of them, so yeah i can see the difference and it feels so good:

![](https://miro.medium.com/v2/resize:fit:498/1*OEv05rGAyiKuZvVPyJFreg.gif)

You can check my Notes and use it but i still encourage you to make your own cheatsheet.

My Notes — [https://strange-1.gitbook.io/notes/](https://strange-1.gitbook.io/notes/)

### Connect with me

[![Twitter](https://img.shields.io/badge/Twitter-%231DA1F2.svg?style=for-the-badge&logo=Twitter&logoColor=white)](https://twitter.com/Strange_017)
[![Medium](https://img.shields.io/badge/Medium-%2312100E.svg?style=for-the-badge&logo=Medium&logoColor=white)](https://medium.com/@aryandhiman767)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-%230077B5.svg?style=for-the-badge&logo=LinkedIn&logoColor=white)](https://www.linkedin.com/in/saatvik-dhiman-10923420a)
[![HackTheBox](https://img.shields.io/badge/HackTheBox-6cbf5a.svg?style=for-the-badge&logo=HackTheBox&logoColor=white)](https://app.hackthebox.com/profile/951050)
[![TryHackMe](https://img.shields.io/badge/TryHackMe-212121.svg?style=for-the-badge&logo=TryHackMe&logoColor=white)](https://tryhackme.com/p/Strange000)
[![GitBook](https://img.shields.io/badge/GitBook-3884FF.svg?style=for-the-badge&logo=GitBook&logoColor=white)](https://strange-1.gitbook.io/)


# Resources for Learning:

Basic Pentesting Courses:

-   [https://academy.tcm-sec.com/p/practical-ethical-hacking-the-complete-course](https://academy.tcm-sec.com/p/practical-ethical-hacking-the-complete-course)
-   [https://www.udemy.com/course/learn-ethical-hacking-from-scratch/](https://www.udemy.com/course/learn-ethical-hacking-from-scratch/)
-   [https://academy.hackthebox.com/path/preview/penetration-tester](https://academy.hackthebox.com/path/preview/penetration-tester)
-   Pivoting -[https://academy.hackthebox.com/course/preview/pivoting-tunneling-and-port-forwarding](https://academy.hackthebox.com/course/preview/pivoting-tunneling-and-port-forwarding)
-   File Transfers -[https://academy.hackthebox.com/course/preview/file-transfers](https://academy.hackthebox.com/course/preview/file-transfers)

Windows Privilege Escalation:

-   [https://www.udemy.com/course/windows-privilege-escalation/](https://www.udemy.com/course/windows-privilege-escalation/)
-   [https://academy.tcm-sec.com/p/windows-privilege-escalation-for-beginners](https://academy.tcm-sec.com/p/windows-privilege-escalation-for-beginners)
-   [https://academy.hackthebox.com/course/preview/windows-privilege-escalation](https://academy.hackthebox.com/course/preview/windows-privilege-escalation)

Linux Privilege Escalation:

-   [https://www.udemy.com/course/linux-privilege-escalation/](https://www.udemy.com/course/linux-privilege-escalation/)
-   [https://academy.tcm-sec.com/p/linux-privilege-escalation](https://academy.tcm-sec.com/p/linux-privilege-escalation)
-   [https://academy.hackthebox.com/course/preview/linux-privilege-escalation](https://academy.hackthebox.com/course/preview/linux-privilege-escalation)

Active Directory:

-   [https://academy.hackthebox.com/course/preview/introduction-to-active-directory](https://academy.hackthebox.com/course/preview/introduction-to-active-directory)
-   [https://academy.hackthebox.com/course/preview/active-directory-enumeration--attacks](https://academy.hackthebox.com/course/preview/active-directory-enumeration--attacks)
-   [https://www.netwrix.com/attack.html](https://www.netwrix.com/attack.html)

Buffer Overflow:

-   Heath Adams -[https://www.youtube.com/watch?v=ncBblM920jw&themeRefresh=1](https://www.youtube.com/watch?v=ncBblM920jw&themeRefresh=1)
-   [https://tryhackme.com/room/bufferoverflowprep](https://tryhackme.com/room/bufferoverflowprep)
-   Linux Buffer Overflow -[https://academy.hackthebox.com/course/preview/stack-based-buffer-overflows-on-linux-x86](https://academy.hackthebox.com/course/preview/stack-based-buffer-overflows-on-linux-x86)
-   Windows Buffer Overflow -[https://academy.hackthebox.com/course/preview/stack-based-buffer-overflows-on-windows-x86](https://academy.hackthebox.com/course/preview/stack-based-buffer-overflows-on-windows-x86)

Platforms to practice:

-   [https://tryhackme.com/](https://tryhackme.com/)
-   [https://www.hackthebox.com/](https://www.hackthebox.com/)
-   [https://portal.offsec.com/sign-in](https://portal.offsec.com/sign-in)
-   [https://portswigger.net/web-security](https://portswigger.net/web-security)

Useful sites:

-   Reverse shells -[https://www.revshells.com/](https://www.revshells.com/)
-   Cracking hashes -[https://crackstation.net/](https://crackstation.net/)
-   Checking hashes -[https://hashcat.net/wiki/doku.php?id=example_hashes](https://hashcat.net/wiki/doku.php?id=example_hashes)

Other Useful Resources:

-   [https://book.hacktricks.xyz/welcome/readme](https://book.hacktricks.xyz/welcome/readme)
-   [https://github.com/Kitsun3Sec/Pentest-Cheat-Sheets](https://github.com/Kitsun3Sec/Pentest-Cheat-Sheets)
-   [https://github.com/swisskyrepo/PayloadsAllTheThings](https://github.com/swisskyrepo/PayloadsAllTheThings)
-   [https://liodeus.github.io/2020/09/18/OSCP-personal-cheatsheet.html](https://liodeus.github.io/2020/09/18/OSCP-personal-cheatsheet.html)
-   [https://github.com/tagnullde/OSCP/blob/master/oscp-cheatsheet.md](https://github.com/tagnullde/OSCP/blob/master/oscp-cheatsheet.md)
-   [https://reconshell.com/oscp-preparation-cheat-sheets/](https://reconshell.com/oscp-preparation-cheat-sheets/)

Thank you for Reading…
