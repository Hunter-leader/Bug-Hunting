Payload is stored server-side and can be triggered by a victim with no interaction outside of the application

Also Known as persistent XSS

- It stores the payload in the database
- The payload is reflected back to the user when visiting a particular page
- One of the most famous stored XSS is in TweetDeck.

The payload is stored **server-side** and can be triggered by a victim without any interaction outside of using the application


example:
```XSS
<script>
class="xss">$('.xss').parents().eq(1).find('a').
eq(1).click();$('[data-action=retweet]').click();alert('XSS in Tweetdeck')</script>
```
