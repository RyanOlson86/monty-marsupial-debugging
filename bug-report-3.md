# Bug Report!

## Describe

**What is happening? What do you see?**
Name and color are rendering in the wrong columns on the DOM


**What _should_ be happening? What do you want to see?**
Color and name should be in the right columns

## Isolate

**Is this problem client side? Server side? Elsewhere? How do you know?**
Problem is in the database. Existing koalas have name and color properties switched. Adding new koalas with the form populates the DOM correctly

**What line of code is the error happening on?**

Paste the relevant code here:
```
n/a
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
console.log of incoming data from GET functions is showing name and color keys reversed for starting data of the database

## Fix

❗ Don't try to fix before first **describing** and **isolating!**

Briefly describe your fix:
swapped name and color values in INSERT function in postico

**What tools did you use?**

- [x] Fix one line of code. Then test using the debugger or `console.log()`s.
- [ ] Google search
- [ ] Ask a pod mate for help
- [ ] Escalate

**Results**

<!-- Go back to your original description. Is the app behaving how you want it to, now? Describe the bug, technically: what was your code doing wrong, and how did you fix it. -->
fixed starting database and now everything works well