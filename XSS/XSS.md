#### Cross - Site Scripting

- What is XSS?
	XSS allows an attacker to execute arbitrary client-side code on a victim's browser. XSS can be used for phishing, exfiltrating data, account takeovers and more.

---
#### How does XSS work ?

- An attacker inserts a malicious script ( or a payload ) into the victim's browser
- When the victim encounters the script it executes in the victim's browser.
- A malicious payload is able to perform any action that the victim is able to perform.
- If the victim has special privileges it can be a serious vulnerability.

---
#### Impact

- Read / Modify / Delete content of any page
- Steal a users cookies or session and gain access to their account 
- Server malicious content like phishing

---
#### Reflected XSS

Payload is injected from the victim's request. Victim's request. Victim must click a malicious link or navigate to an attacker-controlled property.


#### Stored XSS

Payload is stored server-side and can be triggered by a victim with no interaction outside of the application


#### DOM XSS

The vulnerability is in the client-side code versus the server-side. Injection is still typically from the victim's request.


#### Blind XSS

--- 

xss example: `<script>alert(document.cookie)</alert>`

---
#### Polyglots:

An XSS polyglot is a string of text which can escape attribute, tags and bypass filters all in one. You could have used the below polyglot on all six level's you've just complete, and it would have executed the code successfully 

```Javascript
jaVasCript:/*-/*`/*\`/*'/*"/**/(/* */onerror=alert('THM') )//%0D%0A%0d%0a//</style/<title/</teXtarEa/</scRipt/-
-!>/x3csVg/<sVg/<sVg/oNloAd=alert('THM')//>\x3e
```

---
Choose an XSS payload 
Insert that payload everywhere possible.
Read the source page
try to execute the payload or try to bypass the filters or mitigations.

some payload:
```javascript
<Script>alert('hello')</Script>
```

```Javascript
<Script>alert(document.Cookie)</Script>
```

```Javascript
<Script>alert(document.Domain)</Script>
```

```Javascript
<Script>
```


---
#### How to know is XSS alive or not 

- check first run normal script / try encode & decode
- check parameter
- check CSP: Content Security Policy / is alive then bypass it
- 
- 