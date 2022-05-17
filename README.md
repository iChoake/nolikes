Ever wanted to delete all your likes/favorites from Twitter but only found broken/expensive tools? You are in the right place.

1. Go to: https://twitter.com/{username}/likes
** Add Info on How to Open Chrome Developer Safely **
3. Open the console and run the following JavaScript code:

```javascript
setInterval(() => {
  for (const d of document.querySelectorAll('div[data-testid="unlike"]')) {
    d.click()
  }
  window.scrollTo(0, document.body.scrollHeight)
}, 1000)
```
