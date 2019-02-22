# CSP Violation Demo

Firefox does not like the solution to CSP violations (using `try…catch` + `eval`/`Function`) existing in `web3@1.0.0-beta.46`. This little repo shows a fix proposal, pretty much.

`NOTE`: It seems to be a Firefox-specific issue.

You can diff `web3.js` files: 
```
diff broken/web3.js fixed/web3.js
```

---

Run it with `npx static . -p 5000` and navigate to http://localhost:5000, open the console and click through the links. "Broken" page should display the following error message (twice):
> _Content Security Policy: The page’s settings blocked the loading of a resource at eval (“script-src”)._

Screenshot:
https://www.dropbox.com/s/m8z4mlc1yr7no6r/Screenshot%202019-02-22%2012.56.09.png?dl=0
