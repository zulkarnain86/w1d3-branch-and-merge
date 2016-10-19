![](https://makersinstitute.id/img/logo-makersinstitute.png)

# Branch and Merge Conflicts

## Objectives

In this project you'll going to do a fast-forward merge and solve a merge conflict with your partner.

## Fast-Forward Merge

### Step 1:

- In this repo exist a file called homework.js. 
- Your task is to change the content of this file on a branch and then merge it to master branch. 
- You can see the instruction in **javascript-homework** folder. 
- Instead of making just 1 commit, make another commit by making another change.

### Step 2:

- You can see your log in prettier way with `git log --all --graph --decorate --oneline --simplify-by-decoration`.
- As you can see that your branch is two commit ahead from your master.
- Now we are going to add all the change you make in the new branch to master branch.
- Go to master branch, and then use `git merge your-branch-name`.
- From here again use `git log --all --graph --decorate --oneline --simplify-by-decoration` to see the pretty git log.
- You can see that master and your branch are in the same line. And there is just one line. This is what is called fast-forward merge.

## Keep Calm and Solve the Conflicts

Now you're going to collaborate with your friend to make a change to howework.js file.

### Step 1:

- First, go to this forked repo, and go to **settings**. 
- In settings click **Collaborators & teams** below options. 
- Now input your password so you can go in. 
- Decide with your friend who's going to invite and accept the invitation. 
- In collaborators tab, write your friends username to add collaborator. 
- After that copy the invitation link to your friend so your friend can be a collaborator to your repo.
- Your friend must accept the invitation.
- Now your friend can push to your repo.

### Step 2:

- Your friend has to clone your repo. 
- Now you and your friend are going to collaborate. 
- In local, both of you, in `master` branch, make a change to the **homework.js** file. 
- Make sure you and your friend make a different change, but in the same line.
- Now let your friend push (after add and commit first of course) his change to server first.
- Then you push your change the server.
- You'll going to see that this is won't work because you're friend already push a change first. There is a conflict.

### Step 3:

- Don't panic. We are going to solve this conflict.
- Use `git fetch` to get your friend change. 
- Your friend's change is stored in `origin/master` branch.
- You can use `git checkout origin/master` to see your friend's work. The text in text editor is changing as you change the branch.
- Go back to master branch with `git checkout master`. We are going to solve this conflict once for all.
- Use `git merge origin/master` to merge your friend's work with yours, from `origin/master` to `master`.
- Now you see in your text editor there are some symbols like this that added by Git:
```
<<<<<<<<
Your work
=====
Your friend's work
>>>>>>>>
```
- Decide with your friend what change that you are two going to make.
- Then write the change and remove all the symbol that added by Git.
- Finally, add, commit, and push. Congratz! You have solve the conflict. You and your friend are happy. :smile:
- You and your friend can swap role and let your friend solve the conflict.

## Contributions
If you see a problem or a typo, please fork, make the necessary changes, and create a pull request so we can review your changes and merge them into the master repo and branch.
