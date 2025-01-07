Open redirects happen when the web application takes an untrusted input and redirects a user from the web application to untrusted site or resources that will be used further for malicious purpose.

The impact for Open Redirect is usually low, unless you are using it to escalate other vulnerabilities.

Sometimes the application may have some security measures in place where the developers define a list of either trusted or untrusted resources. In some cases, you may be able to bypass it, if you fully understand how it works.



#### Open Redirect {filtering and Bypasses}

- `https://example.com/login/?nextPage=https://google.com` {allow}
- `https://example.com/login/?nextPage=https://evilsite.com` {not allow}
- `https://example.com/login/?nextPage=https://evilsite.com/?google.com` {allow}

bypass: https://www.google.com@youtube.com@yahoo.com
another method: https://www.google.com/?redirect=https://<malicious-site.com>
