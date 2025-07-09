LENOVO@DESKTOP-5S3K7S4 MINGW64 ~/OneDrive/Desktop/confilt
$ git init
Initialized empty Git repository in C:/Users/LENOVO/OneDrive/Desktop/confilt/.git/

LENOVO@DESKTOP-5S3K7S4 MINGW64 ~/OneDrive/Desktop/confilt (master)
$ ls

LENOVO@DESKTOP-5S3K7S4 MINGW64 ~/OneDrive/Desktop/confilt (master)
$ pwd
/c/Users/LENOVO/OneDrive/Desktop/confilt

LENOVO@DESKTOP-5S3K7S4 MINGW64 ~/OneDrive/Desktop/confilt (master)
$ echo "first html file">shaku.html

LENOVO@DESKTOP-5S3K7S4 MINGW64 ~/OneDrive/Desktop/confilt (master)
$ git add shaku.html
warning: in the working copy of 'shaku.html', LF will be replaced by CRLF the next time Git touches it

LENOVO@DESKTOP-5S3K7S4 MINGW64 ~/OneDrive/Desktop/confilt (master)
$ git add .

LENOVO@DESKTOP-5S3K7S4 MINGW64 ~/OneDrive/Desktop/confilt (master)
$ git commit -m "first commit"
[master (root-commit) 0492829] first commit
 1 file changed, 1 insertion(+)
 create mode 100644 shaku.html

LENOVO@DESKTOP-5S3K7S4 MINGW64 ~/OneDrive/Desktop/confilt (master)
$ git status
On branch master
nothing to commit, working tree clean

LENOVO@DESKTOP-5S3K7S4 MINGW64 ~/OneDrive/Desktop/confilt (master)
$ git branch
* master

LENOVO@DESKTOP-5S3K7S4 MINGW64 ~/OneDrive/Desktop/confilt (master)
$ git branch feature_a

LENOVO@DESKTOP-5S3K7S4 MINGW64 ~/OneDrive/Desktop/confilt (master)
$ git checkout feature_a
Switched to branch 'feature_a'

LENOVO@DESKTOP-5S3K7S4 MINGW64 ~/OneDrive/Desktop/confilt (feature_a)
$ echo "css file"> style.css

LENOVO@DESKTOP-5S3K7S4 MINGW64 ~/OneDrive/Desktop/confilt (feature_a)
$ git add .
warning: in the working copy of 'style.css', LF will be replaced by CRLF the next time Git touches it

LENOVO@DESKTOP-5S3K7S4 MINGW64 ~/OneDrive/Desktop/confilt (feature_a)
$ git commit -m "second commit"
[feature_a 8b1e14f] second commit
 1 file changed, 1 insertion(+)
 create mode 100644 style.css

LENOVO@DESKTOP-5S3K7S4 MINGW64 ~/OneDrive/Desktop/confilt (feature_a)
$ git status
On branch feature_a
nothing to commit, working tree clean

LENOVO@DESKTOP-5S3K7S4 MINGW64 ~/OneDrive/Desktop/confilt (feature_a)
$ git checkout master
Switched to branch 'master'

LENOVO@DESKTOP-5S3K7S4 MINGW64 ~/OneDrive/Desktop/confilt (master)
$ git branch feature_b

LENOVO@DESKTOP-5S3K7S4 MINGW64 ~/OneDrive/Desktop/confilt (master)
$ git checkout feature_b
Switched to branch 'feature_b'

LENOVO@DESKTOP-5S3K7S4 MINGW64 ~/OneDrive/Desktop/confilt (feature_b)
$ echo "this is css file"> style.css

LENOVO@DESKTOP-5S3K7S4 MINGW64 ~/OneDrive/Desktop/confilt (feature_b)
$ git add style.css
warning: in the working copy of 'style.css', LF will be replaced by CRLF the next time Git touches it

LENOVO@DESKTOP-5S3K7S4 MINGW64 ~/OneDrive/Desktop/confilt (feature_b)
$ git commit -m "third commit"
[feature_b 4ca6d2e] third commit
 1 file changed, 1 insertion(+)
 create mode 100644 style.css

LENOVO@DESKTOP-5S3K7S4 MINGW64 ~/OneDrive/Desktop/confilt (feature_b)
$ git branch
  feature_a
* feature_b
  master

LENOVO@DESKTOP-5S3K7S4 MINGW64 ~/OneDrive/Desktop/confilt (feature_b)
$ git checkout feature_a
Switched to branch 'feature_a'

LENOVO@DESKTOP-5S3K7S4 MINGW64 ~/OneDrive/Desktop/confilt (feature_a)
$ git merge feature_b
Auto-merging style.css
CONFLICT (add/add): Merge conflict in style.css
Automatic merge failed; fix conflicts and then commit the result.

LENOVO@DESKTOP-5S3K7S4 MINGW64 ~/OneDrive/Desktop/confilt (feature_a|MERGING)
$ nano style.css

LENOVO@DESKTOP-5S3K7S4 MINGW64 ~/OneDrive/Desktop/confilt (feature_a|MERGING)
$ git add style.css

LENOVO@DESKTOP-5S3K7S4 MINGW64 ~/OneDrive/Desktop/confilt (feature_a|MERGING)
$ git commit -m "fourth commit"
[feature_a a8cf675] fourth commit

LENOVO@DESKTOP-5S3K7S4 MINGW64 ~/OneDrive/Desktop/confilt (feature_a)
$ git merge feature_b
Already up to date.

LENOVO@DESKTOP-5S3K7S4 MINGW64 ~/OneDrive/Desktop/confilt (feature_a)
$ git branch -M main

LENOVO@DESKTOP-5S3K7S4 MINGW64 ~/OneDrive/Desktop/confilt (main)
$ git remote add origin https://github.com/shakunthala1611/confilt.git

LENOVO@DESKTOP-5S3K7S4 MINGW64 ~/OneDrive/Desktop/confilt (main)
$ git push -u origin main
Enumerating objects: 12, done.
Counting objects: 100% (12/12), done.
Delta compression using up to 12 threads
Compressing objects: 100% (7/7), done.
Writing objects: 100% (12/12), 993 bytes | 331.00 KiB/s, done.
Total 12 (delta 1), reused 0 (delta 0), pack-reused 0 (from 0)
remote: Resolving deltas: 100% (1/1), done.
To https://github.com/shakunthala1611/confilt.git
 * [new branch]      main -> main
branch 'main' set up to track 'origin/main'.

LENOVO@DESKTOP-5S3K7S4 MINGW64 ~/OneDrive/Desktop/confilt (main)
$
