Payload is injected from the victim's request. Victim's request. Victim must click a malicious link or navigate to an attacker-controlled property.


| Request                          | Response            | Explanation    |
| -------------------------------- | ------------------- | -------------- |
| site.com/page?name=John          | Hello, John         | Normal request |
| site.com/page?name=`<u>John</u>` | Hello,`<u>John</u>` | No XSS         |
| site.com/page?name=`<u>John</u>` | Hello, John         | Possible XSS   |

In this example, the payload is injected into the victim's request using the "name" parameter. In order for this to work, the victim must click this malicious link or navigate to an attacker-controlled property. `https://example.com/page?param=<payload>`

- Example: `http://www.facebook.com/translations/?aloc=ro_RO&search=&app=1&q='"><script>alert(document.cookie)</script>`

payload inserted through the "q" parameter.
Payload reflects unfiltered here. {"'">}


---
### Q1: <script>alert('1')</script> Which XSS it is ?

##### ANS: Reflected XSS



