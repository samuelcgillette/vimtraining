# Challenges

Three timed challenges, about 5 minutes each, that use the skills from `vim-practice.txt`. Finish the practice file first.

| # | File | Mission |
|---|------|---------|
| 1 | `01-lectitio-divinitatus.txt` | Restore pages of the Lectitio Divinitatus sabotaged by Chaos cultists |
| 2 | `02-guardsmen-primer.txt` | Fix the typos and false doctrine in a misprinted Guardsman's primer |
| 3 | `03-weakness-of-my-windows.txt` | Rescue a Tech-Priest's sermon from a failing Windows machine |

## How to play

```bash
vim challenges/01-lectitio-divinitatus.txt
```

Read the orders at the top of the file, then fix the record below them. Unlike the lessons, the orders tell you *what* is wrong but not *which keys* to press.

When you're done, save and check your work from inside Vim:

```
:w
:!diff % %:h/keys/01-lectitio-divinitatus-solved.txt
```

No output means you got it exactly right. Each challenge file lists its own check command.

## Keys

The `keys/` folder has two files for each challenge:

- `*-key.txt` is a step-by-step solution that lists the lesson each step uses.
- `*-solved.txt` is the finished file that the diff check compares against.

## Start over

```bash
git checkout challenges/
```
