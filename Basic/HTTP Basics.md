```http
GET /HTTP/1.1
Host: nahamsec.com
User-Agent: Mozila/5.0(Macintosh;Intel Mac OS X 10.9; rv:50.0) Gecko/20100101Firefox/50.5
Accept:text/html,application/xhtml+xml,application/xml;q=0.9,*/*;q=0.8
Authorization: BearerSOMETHING_HERE
Referrer: https://www.google.com
```

#### HTTP Basics Continued

- What page (or endpoint) to fetch

```http
GET /HTTP/1.1
```

---

- What website (or host) to fetch from

```http
HOST: nahamsec.com
```

---

- Browser information including name, version or etc

```HTTP
User-Agent: Mozila/5.0(Macintosh;Intel Mac OS X 10.9; rv:50.0)
```

---

- What type of data to send / receive

```HTTP
Content-type:
```

---

- Authorization header allowing you to fetch data

```HTTP
Authorization: Bearer 
SOMETHING_HERE
```

---

- What site / page sent you to this new page

```HTTP
Referrer: https://www.google.com
```

---

#### Commonly Used HTTP Methods

- **GET** : to fetch data
- **HEAD** : Does the same things as get but doesn't show the full response
- **POST** : to create or change data
- **PUT** : to replace to modify data
- **DELETE** : to delete data
- **OPTIONS** : to see communication options (GET, HEAD, POST, PUT, DELETE, ETC)

---

#### Most Common Response Status Codes

| Range | Status                                                                |
| ----- | --------------------------------------------------------------------- |
| 200   | Successful response                                                   |
| 300   | Redirects                                                             |
| 401   | Unauthorized or unauthenticated                                       |
| 403   | Forbidden or no access to resources                                   |
| 404   | Not Found or file doesn't exist                                       |
| 405   | HTTP Method not allowed                                               |
| 500   | Internal error when the server doesn't know how to handle the request |
and tons more. you can check them out on Mozilla's website (https://developer.mozilla.org/en-US/docs/web/HTTP/Status)

