# Bug Report!

## Describe

**What is happening? What do you see?**
When adding koalas into SQL database, getting an error
ERROR:  invalid input syntax for type integer: "Red"
LINE 4:  ('Scotty', 'Red', 4, TRUE, 'Born in Guatemala'), 
                    ^

**What _should_ be happening? What do you want to see?**
Should be adding new info into table

## Isolate

**Is this problem client side? Server side? Elsewhere? How do you know?**
In the database setup

**What line of code is the error happening on?**
n/a

Paste the relevant code here:
```
ERROR:  invalid input syntax for type integer: "Red"
LINE 4:  ('Scotty', 'Red', 4, TRUE, 'Born in Guatemala'), 
                    ^
```

And describe what it's doing wrong:
The table is expecting integer for "name" but getting a VARCHAR

**What tools did you use to isolate the error?**

- [ ] `console.log()`
- [ ] Chrome debugger (_Sources_ panel)
- [ ] VSCode debugger
- [ ] Chrome Network Panel
- [ ] Postman
- [x] Postico

<!-- Briefly describe how the tool helped you, and how you used it -->
Postico showed the error was a syntax error


## Fix

❗ Don't try to fix before first **describing** and **isolating!**

Briefly describe your fix:
changed "name" input type to VARCHAR(20) NOT NULL

**What tools did you use?**

- [X] Fix one line of code. Then test using the debugger or `console.log()`s.
- [ ] Google search
- [ ] Ask a pod mate for help
- [ ] Escalate

**Results**

<!-- Go back to your original description. Is the app behaving how you want it to, now? Describe the bug, technically: what was your code doing wrong, and how did you fix it. -->
The database would not add values to table because value type was wrong. Now values are added to table but in wrong column