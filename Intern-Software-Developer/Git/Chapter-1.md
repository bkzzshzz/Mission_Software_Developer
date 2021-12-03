# About Git

## 1. To view the git version: `git --version`

## 2. To view the contents of a git repository including the contents of hidden .git folder:
```
bikesh@bkes:~$ cd Desktop/ && find Mission_Software_Developer
```
### The contents will be shown as:
```
Mission_Software_Developer
Mission_Software_Developer/Intern-Software-Developer
Mission_Software_Developer/Intern-Software-Developer/Git
Mission_Software_Developer/Intern-Software-Developer/Git/about-git.md
Mission_Software_Developer/.git
Mission_Software_Developer/.git/refs
Mission_Software_Developer/.git/refs/tags
Mission_Software_Developer/.git/refs/heads
Mission_Software_Developer/.git/HEAD
Mission_Software_Developer/.git/branches
Mission_Software_Developer/.git/hooks
Mission_Software_Developer/.git/hooks/pre-push.sample
Mission_Software_Developer/.git/hooks/prepare-commit-msg.sample
Mission_Software_Developer/.git/hooks/post-update.sample
Mission_Software_Developer/.git/hooks/fsmonitor-watchman.sample
Mission_Software_Developer/.git/hooks/pre-merge-commit.sample
Mission_Software_Developer/.git/hooks/pre-rebase.sample
Mission_Software_Developer/.git/hooks/applypatch-msg.sample
Mission_Software_Developer/.git/hooks/update.sample
Mission_Software_Developer/.git/hooks/pre-receive.sample
Mission_Software_Developer/.git/hooks/pre-applypatch.sample
Mission_Software_Developer/.git/hooks/pre-commit.sample
Mission_Software_Developer/.git/hooks/commit-msg.sample
Mission_Software_Developer/.git/description
Mission_Software_Developer/.git/config
Mission_Software_Developer/.git/info
Mission_Software_Developer/.git/info/exclude
Mission_Software_Developer/.git/objects
Mission_Software_Developer/.git/objects/info
Mission_Software_Developer/.git/objects/pack
```

## 3. `git add <filename>` to add to the repo

## 4. `git diff` to enlist the insertions and deletions or simply updates on a file.

## 5. `git diff master~1 master` shows the difference between the previous commit and the latest commit.
```
bikesh@bkes:~/Desktop/hacker_rank$ git diff --word-diff master~1 master
diff --git a/matrix_manipulation.py b/matrix_manipulation.py
index 9178a47..6796b07 100644
--- a/matrix_manipulation.py
+++ b/matrix_manipulation.py
@@ -34,4 +34,5 @@ print(f"The row wise summation of \n {y} \n is \n {numpy.sum(y, axis=1)} ")
#The transpose is given by .T
print(f"The transpose of matrix \n {x} is \n {x.T}")

{+# Added a remark+}
```

## 6. `git diff --stat master~1 master` shows the only the changes like:
```
bikesh@bkes:~/Desktop/hacker_rank$ git diff --stat master~1 master
 matrix_manipulation.py | 37 +++++++++++++++++++++++++++++++++++++
 1 file changed, 37 insertions(+)
```

