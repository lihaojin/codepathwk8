# codepathwk8
# Project 8 - Pentesting Live Targets

Time spent: **X** hours spent in total

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

Vulnerability #2: __________________


## Green

Vulnerability #1: XSS
<img src='https://raw.githubusercontent.com/lihaojin/codepathwk8/master/green1.gif'/>
Details: First go to the contact page as a visitor and type in a random name and email in the designated fields. Then paste the following into the feedback.
<script>alert('Haojin Li');</script>
Afterwards log in and click on the feedback.

Vulnerability #2: __________________


## Red

Vulnerability #1: __________________

Vulnerability #2: __________________


## Notes

Describe any challenges encountered while doing the work
