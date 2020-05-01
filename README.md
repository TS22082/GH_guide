
# Jump to sections
- [Branching](#branching)<br>
- [Versioning](#versioning)<br>
- [Fork](#fork)

# Branching

**Example:**

![Starting Point](./assets/git_master.png)

The first thing to do is to create a new branch and then move to that branch

**In your terminal**

```
git checkout -b <branchname>
```

**Example:**

![Alt Text](./assets/new_branch.gif)
&nbsp;

# Add changes

Add you changes to the code then go through the push process

```
git add *
git commit -m "added changes"
git push origin <branchname>
```

**In your browser**

Navigate to the code repo on your github

Click Branches (next to code)

Find your branch then click "create pull request"

Click "Accept changes" (This will update the changes you made to the repos master)

![Alt Text](./assets/GUI_new_example.gif)

## Pull changes

**In your terminal**

Change to the master branch

```
git checkout master
```

Then pull changes

```
git pull
```

## Clean Tree

List branches

```
git branch -l
```

Delete the old branch (this keeps the tree clean)

```
git branch -d <branchname>
```

**Example:**

![Alt Text](./assets/check_and_delete.gif)

At this point you are on master, the code has been update, and you are ready to create a new branch to start working on a new feature.

# Versioning

There are many ways to go back to an old version using git and github. I prefer to copy the version I want to a seperate branch and make a pull request because that method isnt destructive like "revert" is.

![Alt Text](./assets/commit.png)

![Alt Text](./assets/commitHash.png)

```
git checkout -b <branch name> <commit hash>
```

This will create a new branch with the old version of the code. 

Add a comment or make some minor change so you can add.

```
git commit -m "go back to old version of code"
git add *
git push origin <branch name>
```

Navigate repo, you will see a new pull request. Accept the change and merge to master.

# Fork

Anytime you want to add to someone elses code on gh you will fork the original code so you have a copy you can make changes to, then make a pull request to let the original creator you made a contribution they can accept or decline.

A friends repo that I will fork:

![Alt Text](./assets/fork.png)

After I fork the repository I will have a copy on my github account that I can clone and update.

![Alt Text](./assets/clone.png)

![Alt Text](./assets/update.gif)

Navigate back to the repo on github (your account). You will see your version has been updated. If this is a change we want the original creator to include in ther code, make a pull request.

![Alt Text](./assets/pull_request.gif)

The original code owner will be notified there is a new pull request. After they accept it the code will e updated. 

![Alt Text](./assets/added_change.gif)

