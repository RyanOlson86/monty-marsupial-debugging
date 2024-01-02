# Bug Report!

## Describe

**What is happening? What do you see?**
express deprecated res.send(status): Use res.sendStatus(status) instead server/routes/koala.router.js:77:17
in the server terminal

**What _should_ be happening? What do you want to see?**
Should be sending a status instead of res.send()


## Isolate

**Is this problem client side? Server side? Elsewhere? How do you know?**
server side because error is in the server terminal

**What line of code is the error happening on?**

Paste the relevant code here:
```js
express deprecated res.send(status): Use res.sendStatus(status) instead server/routes/koala.router.js:77:17
```

And describe what it's doing wrong:

**What tools did you use to isolate the error?**

- [x] `console.log()`
- [ ] Chrome debugger (_Sources_ panel)
- [ ] VSCode debugger
- [ ] Chrome Network Panel
- [ ] Postman
- [ ] Postico

<!-- Briefly describe how the tool helped you, and how you used it -->


## Fix

❗ Don't try to fix before first **describing** and **isolating!**

Briefly describe your fix:
changed res.send(200) to res.sendStatus(200) on line 77 of koala.router.js

**What tools did you use?**

- [x] Fix one line of code. Then test using the debugger or `console.log()`s.
- [ ] Google search
- [ ] Ask a pod mate for help
- [ ] Escalate

**Results**

<!-- Go back to your original description. Is the app behaving how you want it to, now? Describe the bug, technically: what was your code doing wrong, and how did you fix it. -->