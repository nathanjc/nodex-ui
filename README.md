# 1. You want to start editing some code

Open your terminal:

    $ cd Development/Catalysm/nodex-ui

What branch are you on? "master", "develop", or "one-of-your-own"

Always run:

    $ git status

This keeps you aware of what's happening.

### If you're in the "develop" branch:

    $ git checkout -b new-feature

Start editing.

### Else, if you are in "one-of-your-own" branches:

Start editing.

===

# 2. You've edited some code and want to save your changes

Run:

    $ git status

See what's changed.

### If you've added or deleted files you'll want to run:

    $ git add -A

(This will add/delete any new/deleted files)

Then:

    $ git commit -m "I made some awesome updates to my code!"

### Or if you've only "modified" files:

You can shortcut the above command to:

    $ git commit -am "I made some awesome updates to my code!"

===

# 3. You're done working on a feature and want to merge your edits back to the develop branch

**You must complete Step 2. before this step!**

Run:

    $ git status

### If this returns:

    Your branch is up-to-date with 'origin/develop'.
    nothing to commit, working directory clean

Run:

    $ git checkout develop
    $ git status
    $ git merge new-feature

If you followed the above instructions there should be no problems, hurrah!

### Else if it returns a problem:

Fix the problem and run through the steps again until there are no problems!

===

# You've committed your code and want to push the updates to Github

**Make sure you're in the "develop" branch!**

Run:

    $ git status

### If this returns:

    nothing to commit, working directory clean

Run:

    $ git push origin develop

### Else if it returns a problem:

Fix the problem and run through the steps again until there are no problems!
