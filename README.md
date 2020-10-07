# Git Challenge
There are two branches, `add-echo` and `add-reverse`. The goal of this challenge is to use `git rebase` to bring both commits onto master. When finished there should be no merge commits or branching. For example, `git log` on the `master` branch should look similar to this:
```
/challenge-git master
⚡ git log
61a2c67 feat: add reverse route (David Guttman, 7 minutes ago)
2c2c5d6 feat: add echo route (David Guttman, 10 minutes ago)
dcc4c0b docs: add more instructions (David Guttman, 11 minutes ago)
...
```
## Instructions
How to attempt this challenge:
1) Create a new repo in your account and note the git url
2) Clone this repo
3) Solve the challenge
4) Set your new repo as the origin: `git remote set-url origin ${your repo url}`
5) Push your solution to your repo
You must follow these steps for your solution to be accepted -- forks or other methods will not be considered.

## How to solve it
1) Create a new repo in your account and note the git url
- don't create README, just create empty project
- don't clone it to your computer
- `git url` is what you get for cloning, for example `git@github.com:alepekhin/MyWestHollywoodChallenge.git`
1) Clone this repo
- it obvious, but you can clone it to any other folder as `git clone url folder`
2) Solve the challenge
- go to the folder where an repo was cloned
- execute `npm i`, `npm test`
- switch to the first branch `git checkout add-reverse`
- rebase it `git rebase master`
- switch to master `git checkout master`
- merge branch `git merge add-reverese`
- switch to the second branch `git checkout add-echo`
- rebase it `git rebase master`
- resolve conflicts, execute `npm test` after resolving
- switch to master `git checkout master`
- merge branch `git merge add-echo`
- ??? probably there are some other steps, I forgot 
3) Set your new repo as the origin: `git remote set-url origin ${your repo url}`
- `your repo url` is `git url` from the first step
4) Push your solution to your repo
- git push





