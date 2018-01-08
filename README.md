# OWASP-juice-shop
Let's play it!

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
### 9.Deprecated Interface
 * SKIP
### 10.Login Admin
 * Enter 'or'a'='a' and like %admin% --
### 11.Password Strength
 * I thought it was SQLi and crack password, but pass word is in response in administration page. password crackable.
 ### 12.Basket Access
  * Modify Request URL: http://localhost:3000/rest/basket/1 -> 2
