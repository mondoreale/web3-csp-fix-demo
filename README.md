# CSP Violation Demo

Firefox does not like the solition to CSP violations (using `eval`) existing in `web3@1.0.0-beta.46`. This little repo shows a fix proposal, pretty much.

`NOTE`: It seems to be a Firefox-specific issue.

You can diff `web3.js` files: 
```
diff broken/web3.js fixed/web3.js
```

---

Run it with `npx static . -p 5000` and go to http://localhost:5000
