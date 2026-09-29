# Intro-to-Cyber-Security
TryHackMe: Pre Security - Introduction to Cyber Security  

*So, i can tell which is offensive and defensive security, n also learn about careers available in cyber.
Through this THM, I able to learn basic offensive security concepts, where I able hack a vulnerable online-banking application. Get exposure to defensive security and protect a system by blocking an ongoing cyber attack and in module, i learn about the different careers within cyber security.*

##

Task1: Think Like Hacker!

*Offensive Security is about thinking like an attacker to find weaknesses before real hackers do.*

In this room, i hack the website in a safe and legal environment to see how ethical hackers operate.
Which term describes simulating a hacker's actions to find weaknesses?

    Offensive Security
    Defensive Security
    
Answer: Offensive Security

##

Task2: Start the lab

This room uses a virtual desktop to simulate a real system. A browser will automatically open, display FakeBank, a fake banking application which will be i targeting.
What is the bank account number in the FakeBank application?

<img width="868" height="196" alt="image" src="https://github.com/user-attachments/assets/f8f7e212-512a-4c0e-b435-703ccb208659" />

Answer: 8881

##

Task3: Find Hidden Pages

*Goal - Find a weakness in the FakeBank application. One common mistake is leaving hidden pages accessible.
Open the Terminal on the machine. Use this to run hacking tool, **dirbuster**.*

Finding Hidden Pages: To find hidden pages using Dirbuster, use **dirb** and the URL that wish to search:

    dirb http://fakebank.thm

Any lines from the output that start with + are pages that have been found. Dirb will find two URLs.

Dirb found one URL, http://fakebank.thm/images.
What is the other hidden URL?

<img width="522" height="350" alt="image" src="https://github.com/user-attachments/assets/3291b8e3-636d-437b-9462-ceacded538e5" />

Answer: http://fakebank.thm/bank-transfer

##

Task4: Attack the Admin Page

I found a hidden admin panel that lets me add money to account.

To open this URL in the browser of the simulated desktop:
Add the following below, to the URL in the browser.

    /bank-transfer

Use acc number **8881** and deposit **$2000**. After depositing, return to account page and confirm the balance is now positive.

<img width="667" height="522" alt="image" src="https://github.com/user-attachments/assets/31aac82c-bf3e-4924-b03a-761749f70c42" />

When your balance turns positive, a pop-up with green text appears. So, enter the green words as the answer (ALL CAPS).

Answer: BANK-HACKED.

*Thats it. Thank u.*
