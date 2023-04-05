Repository to code review in Jeelab

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
! When you commit the status, please note what you did (e.g. add some function, change variable name, optimize the code ,...)

- check log
```
>>> git log // you can track the commit history
```

- check branch  
<img title="concept of the branch" alt="concept of the branch" src="https://github.com/github/https://github.com/jyKim-97/neuroscience_code_review/github_branch_flowchart.png">

<img src= width="128"/>

```
>>> git branch
```

- You need to pull repository first


# References
- Mike Cohen book
- 