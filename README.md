# codepathwk8
# Project 8 - Pentesting Live Targets

Time spent: **16** hours spent in total

> Objective: Identify vulnerabilities in three different versions of the Globitek website: blue, green, and red.

The six possible exploits are:
* Username Enumeration
* Insecure Direct Object Reference (IDOR)
* SQL Injection (SQLi)
* Cross-Site Scripting (XSS)
* Cross-Site Request Forgery (CSRF)
* Session Hijacking/Fixation

Each version of the site has been given two of the six vulnerabilities. (In other words, all six of the exploits should be assignable to one of the sites.)

## Blue

Vulnerability #1: SQL Injection

<img src='https://raw.githubusercontent.com/lihaojin/codepathwk8/master/SQLi.gif'/>

Details: Set the id equal to %27%20OR%20SLEEP(5)=0--%27. Then reload the page. The server will wait for 5 seconds before loading.

Vulnerability #2: Session Hijacking/Fixation
<img src='https://raw.githubusercontent.com/lihaojin/codepathwk8/master/blue1.gif'/>
When logged in, use the session id from the logged in page and use it on a different one. The second one will now be logged in as well.

## Green

Vulnerability #1: XSS
<img src='https://raw.githubusercontent.com/lihaojin/codepathwk8/master/green1.gif'/>
Details: First go to the contact page as a visitor and type in a random name and email in the designated fields. Then paste the following into the feedback.
<script>alert('Haojin Li');</script>
Afterwards log in and click on the feedback.

Vulnerability #2: User Enumeration
<img src='https://raw.githubusercontent.com/lihaojin/codepathwk8/master/green2.gif'/>
Details: Registered users produce bolded error message when entering an incorrect password and unregistered users with incorrect passwords produce an unbolded error message.


## Red

Vulnerability #1: CSRF
<img src='https://raw.githubusercontent.com/lihaojin/codepathwk8/master/red1.gif'/>
Details: This attack opens an html file that changes the content of the page.

Vulnerability #2: IDOR
<img src='https://raw.githubusercontent.com/lihaojin/codepathwk8/master/red2.gif'/>
Details: Two salesperson accounts are not supposed to be seen by normal users. However, we find out from the admin account that indexes 10 and 11 are salespersons that aren't supposed to be seen by regular users. When setting the id to 10 in the url, we see that salespersons information.


## Notes

Describe any challenges encountered while doing the work
