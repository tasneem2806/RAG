# Opensource github contribution
## TOC
- [Setting up](#setting-up)

## Setting up
### **Step 1**:
`Fork` the repository that you are about to work on.

### **Step 2**:
After the `Fork` the repo should appear on your own repo. Then you should clone the repo in your machine.
```bash
mkdir RAG
cd RAG
git clone https://github.com/tawsif-r/RAG.git .
```


### **Step 3**
Then get into a new branch using the following command:
```bash
git checkout -b feature/contribution
```

### **Step 4**
work on your branch, then commit, then push onto the remote branch.
```bash
git add .
git commit -m "I have changed some files"
git push origin feature/contribution
```

### **Step 5**
When you go back to your own repo at github web, you will see that there is compare option hovering, which will lead to a review panel.
Thats where the contributor lifecycle ends.

### **Step 6**
You need to make sure you are in the right branch before you start working, preferably the release branch, or the default branch, in most cases it is the main branch. Now after each successful merge it is better to sync the changes with the **FORKED**
repo of your own.

Then in your own machine run these commands which should sync things up with your working repo.
```bash
git checkout main # default branch switch
git fetch --all
git pull origin main # grabbing whatever changes made to this git branch
```


### Issues that you might face when the steps are not properly followed:
- **Merge conflict**: Whenever there is a mismatch between the working branch and the default branch or the branch that you want to merge into then you would get something like a merge conflict. You can resolve these merge conflicts in the github or
on the vscode source control panel.


