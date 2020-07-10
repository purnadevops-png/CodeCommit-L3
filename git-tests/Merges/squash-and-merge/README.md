# Squash and Merge 

1) Let us create a new .git directory for this test 
2) Create a file in master branch and add 3 to 4 lines in it .

```
This is 1
This is 2
This is 3
```
3) Add and commit
3) Create a new branch and checkout to it 
4) Keep editing the file and perform add and commits.
5) Check the commit history by running git log

Now, lets remove the commits not needed 

```
git rebase -i HEAD~3
```
6) Squash the commits not needed 
7) Remove the commits messages not needed 
8) Check git log 

You now see that , the previous commits are no longer present.
