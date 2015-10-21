#Git Cheatsheet

### Start a new project

```shell
$ mkdir project_name
$ git init
$ touch readme.md
$ git add readme.md
git commit -m "Initial Commit"
```

### Do some work and then save it

First do some work! 
Make some changes, put them in the box, label the box.
```shell
$ git status
$ git add <whatever file>
$ git status
$ git commit -m "I made a bunch of changes, there are so many details, wee."
```
### Share my work with the world!

First, create a github repo.


```shell
$ git remote add origin git@github.com:<github username>/<name of repository>.git
$ git push -u origin master
```

### Help someone else with their code

First find the code on github that you want to contribute to.

Then fork it!

```shell
$ git clone git@github.com:<your username>/<repo name>.git
```
Then, make some changes you think are important.

```shell
$ git add <your files>
$ git commit -m "A really thorough explanation of what we did since this is someoe else's work."
$ git push origin master
```
Finish what you started working on, then push up any additional commits.

File a pull request with the commits in it that you want to share. Make sure you have a good explanation in the pull request of what this is, what it's intended to do and some nice languara, rather than making fun of the original author.

### How to work on two different things(changes) at the same time

Branching is for when you want to work on something that might span over multiple commits, that's, significant enough to warrant some kind of really specific deliniation.

### Typical Collaboration Patterns

A typical collaboration pattern is actually to fork then branch off of master, then push to your fork, the file a pull request.

The reason for this is that master, as a branch, should always represent code or whatever that "works" and is suitable for deployment or sharing or whatever "going public" is for you.

### How To Make Git Alias Command Line Shortcuts

It's handy to have keyboard shortcuts in the command line for commands used frequently. Fortunately, there are ways to make aliases for common commands in Git.

```shell
$ git config --global alias.<short cut> <command>
```
Using the above line, we'll create a global alias, or keyboard shortcut for the command line, for a specific command.

```shell
$ git config --global alias.co checkout
```
For above, we used the config command for git to configure git to your preferences and create a global alias "co" (keyboard shortcut for the command line) for the git command "checkout"











