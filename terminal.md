dci-student@thinkpad:~/Desktop/DCI Tutoring Sessions/Movie Card$ `git init`
Initialised empty Git repository in /home/dci-student/Desktop/DCI Tutoring Sessions/Movie Card/.git/

dci-student@thinkpad:~/Desktop/DCI Tutoring Sessions/Movie Card$ `git add .`

dci-student@thinkpad:~/Desktop/DCI Tutoring Sessions/Movie Card$ `git commit -m "first commit"`
[main (root-commit) 36ae6db] first commit
 2 files changed, 144 insertions(+)
 create mode 100644 index.html
 create mode 100644 style.css

dci-student@thinkpad:~/Desktop/DCI Tutoring Sessions/Movie Card (main)$ `git branch`
* main

dci-student@thinkpad:~/Desktop/DCI Tutoring Sessions/Movie Card (main)$ `git switch -c experiment`
Switched to a new branch 'experiment'

dci-student@thinkpad:~/Desktop/DCI Tutoring Sessions/Movie Card (experiment)$ `git branch`
* experiment
  main

dci-student@thinkpad:~/Desktop/DCI Tutoring Sessions/Movie Card (experiment)$ `git add .`

dci-student@thinkpad:~/Desktop/DCI Tutoring Sessions/Movie Card (experiment)$ `git commit -m "experiment background color"`
[experiment 6a1da3d] experiment background color
 1 file changed, 1 insertion(+), 1 deletion(-)

dci-student@thinkpad:~/Desktop/DCI Tutoring Sessions/Movie Card (experiment)$ `git status`
On branch experiment
nothing to commit, working tree clean

dci-student@thinkpad:~/Desktop/DCI Tutoring Sessions/Movie Card (experiment)$ `git log` 
commit 6a1da3dba42845e62dda8ccd165e050013b2e1ef (HEAD -> experiment)
Author: Worlanyo Kwabla Kporfeame <kworlanyo@gmail.com>
Date:   Mon Nov 6 19:21:02 2023 +0100

    experiment background color

commit 36ae6dbbd3ad116b87971b4cdb0034c89ffd214a (main)
Author: Worlanyo Kwabla Kporfeame <kworlanyo@gmail.com>
Date:   Mon Nov 6 19:15:31 2023 +0100

    first commit

dci-student@thinkpad:~/Desktop/DCI Tutoring Sessions/Movie Card (experiment)$ `git checkout main`
Switched to branch 'main'

dci-student@thinkpad:~/Desktop/DCI Tutoring Sessions/Movie Card (main)$ `git merge experiment`
Updating 36ae6db..6a1da3d
Fast-forward
 style.css | 2 +-
 1 file changed, 1 insertion(+), 1 deletion(-)

dci-student@thinkpad:~/Desktop/DCI Tutoring Sessions/Movie Card (main)$ `git add . && git commit -m "change background color"`
[main 514e65f] change background color
 1 file changed, 1 insertion(+), 1 deletion(-)

dci-student@thinkpad:~/Desktop/DCI Tutoring Sessions/Movie Card (main)$ `git remote add origin git@github.com:kworlanyo/movie-card-3.git`

dci-student@thinkpad:~/Desktop/DCI Tutoring Sessions/Movie Card (main)$ `git remote`
origin

dci-student@thinkpad:~/Desktop/DCI Tutoring Sessions/Movie Card (main)$ `git push -u origin main`
Enumerating objects: 10, done.
Counting objects: 100% (10/10), done.
Delta compression using up to 8 threads
Compressing objects: 100% (10/10), done.
Writing objects: 100% (10/10), 1.99 KiB | 1.99 MiB/s, done.
Total 10 (delta 2), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (2/2), done.
To github.com:kworlanyo/movie-card-3.git
 * [new branch]      main -> main
branch 'main' set up to track 'origin/main'.
dci-student@thinkpad:~/Desktop/DCI Tutoring Sessions/Movie Card (main)$ 