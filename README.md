# You're on master

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

# Pull changes

**In your terminal**

Change to the master branch

```
git checkout master
```

Then pull changes

```
git pull
```

# Clean Tree

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

# Finishing Up

At this point you are on master, the code has been update, and you are ready to create a new branch to start working on a new feature.

changes that will be deleted



