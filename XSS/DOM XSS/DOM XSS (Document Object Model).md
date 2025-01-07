The vulnerability is in the client-side code versus the server-side. Injection is still typically from the victim's request.

DOM XSS happens when JavaScript reflects data from an attacker controlled resource (for example the within the URL) and passes it to a function later on.

Consider the following piece of code that could be exploited by linking the victim to the following URL:

`https://example.com/#send-transaction<div/class="header_wrap"><a/href=javascript:alert(0)><h1>pwn3d</h1></a><img/src=//unskid.me/dist/black.gif></div>`

---
##### DOM Based XSS is where the javascript execution happens directly in the browser.

ex: The website's javascript gets the contents from the  `window.location.hash`

---
##### DOM Hacking 

```javascript
"><img src=xss onerror=alert('hello')>//
```
