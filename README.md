# OWASP-juice-shop
Let's play it!

I open http://localhost:3000, it is a web site about juice so that it's called juice shop. I have no idea how to play it LOL.

It looks like I have to login, but not sure it play online or offline?

I tried to login with 'or'1'='1 but not work...but! when I used ' in username box, it's show errors!

Got it! I tried username ' or 'a' = 'a' -- and it work -- is comment is sql.

It say "You successfully solved a challenge: Error Handling (Provoke an error that is not very gracefully handled.)" I think
it's about trying ' in username box and "You successfully solved a challenge: Login Admin (Log in with the administrator's user account.)" for bypass login.

I haven't found the instruction yet. I thought I need to find all URLs.

Luckly, I found a comment about link to scoreboard in the source code.

As I thought, a scoreboard page contains all problem that I have to solve.

### 1.Score Board
  * found a link that is commented in page source
---
### 2.Error Handling
  * login raised an error when entering ' in input box
---
### 3.XSS Tier 1
  * search box is vulnerable to reflect XSS
---
### 4.Five-Star Feedback
  * I thought it was persistent XSS, but it's not. I found admin page at #/administration
---
### 5.Redirects Tier 1
 * SKIP
 ---
 ### 6.Confidential Document
  * When I try to checkout things in basket, it's show path that file is stored. http://localhost:3000/ftp/
 ---
### 7.Admin Section
 * Already found at #/administration
### 8.Zero Stars
 * Just reclick the stars
