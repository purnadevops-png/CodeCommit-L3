# Three way merge

Let us continue from the fast-forward merge

1) Checkout to the branch1

```
git checkout branch1
```

2) Add another file 'branchfile2.html' and commit with a different message .

```
git commit -m "branchfile2"
```

5) Now let us get back to master 
```
git checkout master
```

6) Add one file and commit 

7) Let us circle back to branch1 , add and commit again 

So, by now we made a bunch of commits with both master and branch 

8) Checkout to master and merge the branch . You shold be seeing recursive strategy 

```
Merge made by the 'recursive' strategy.
 test3.html               | 0
 testbranchagainagain.txt | 0
 2 files changed, 0 insertions(+), 0 deletions(-)
 create mode 100644 test3.html
 create mode 100644 testbranchagainagain.txt
 ```

Instead of just moving the branch pointer forward, Git creates a new snapshot that results from this three-way merge and automatically creates a new commit that points to it. This is referred to as a merge commit,