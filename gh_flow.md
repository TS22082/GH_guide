# You're on master

The first thing to do is to create a new branch and then move to that branch

**In your terminal**

```
git checkout -b <branchname>
```

Add you changes to the code then go through the push process

```
git add *
git commit -m "added changes"
git push origin <branchname>
```

**In your browser**

Navigate to your profile on github

Click "create pull request"

Click "Accept changes" (This will pull the changes in you branch to master)

**In your terminal**

Change to the master branch

```
git checkout master
```

Then pull changes

```
git pull
```

List branches

```
git branch -l
```

Delete the old branch (this keeps the tree clean)

```
git branch -d <branchname>
```

At this point you are on master, the code has been update, and you are ready to create a new branch to start working on a new feature.

will this work????
