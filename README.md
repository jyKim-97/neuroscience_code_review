Repository to code review in Jeelab

# Use commandline in Matlab
- add ! before your command  
Example
```MATLAB
!git status
!echo Hello World
```

# Github short start
- sync repository to your local machine  
**! Before modification, you must run this command**
```
git pull // Apply changes in repository to local machine
```

- check status of the file
```
>>> git status // check file sync status in local machine
```
You can also track the file in the matlab (right side on the "Current Folder" tab shows git status)

- add changes and message
If you modified existing code or added new, add to git track and add message
```
>>> git add // apply modification to git staging area (you can run this command multiple times before commit)
>>> git commit -m "some message" // capture the snapshot of current staging area (that you added before) with some message
```
**! When you commit the status, please note what you did (e.g. add some function, change variable name, optimize the code ,...)**

- upload source code
After commit your code, apply the changes to github repository
```
>>> git push
```

- check log
```
>>> git log // you can track the commit history
```

- branch  
<img title="concept of the branch" alt="concept of the branch" src="https://github.com/jyKim-97/neuroscience_code_review/blob/main/github_branch_flowchart.png">

```
>>> git branch // check the current git branch, * means you are in that branch
>>> git checkout "branch name" // switch to "branch name" branch
```

- You need to pull repository first

# How to upload your source code
## Start
- clone repository & make branch
```
>>> git clone https://github.com/jyKim-97/neuroscience_code_review
>>> git branch <TEST> // set your own branch name
```

## Code writing & uploading
- Before write your code, always pull repository & check branch (do not use main branch)
```
>>> git pull // sync
>>> git branch
  main
* <TEST> // -> You need check you are in this branch
>>> git checkout <TEST> // If you are not in <TEST>, switch the branch
```
- After writing your code, or if you want to leave message in the middle
```
>>> git add <source codes> // move the file to staging area
>>> git commit -m "message" // take snapshot of staging area
```
- Upload your source code
```
>>> git push --set-upstream origin <TEST>
```
- After upload your code, go to the github page and make "pull request"  
> When you go to the repository and move to pull requests, you can check **"compare & pull request"** button on the top
<img title="pull request" alt="pull request" src="https://github.com/jyKim-97/neuroscience_code_review/blob/main/github_pull.png">

> After press the button, you can open pull request. Write title of the request and leave the comment if you have.
>  > If you scroll down the page, you can see the file changed  

<img title="open request1" alt="open request1" src="https://github.com/jyKim-97/neuroscience_code_review/blob/main/pull_req1.png">
<img title="scrolling" alt="open request2" src="https://github.com/jyKim-97/neuroscience_code_review/blob/main/pull_req2.png">


# References
- Mike Cohen book
- 