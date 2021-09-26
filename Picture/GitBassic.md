# Learning Github





***Code:***

***Only people who use new install git version control not ever git version***

|                                                              |                                                          |
| ------------------------------------------------------------ | -------------------------------------------------------- |
| Check Version of GitHub:                                     | git version                                              |
| Connection between local repo in your computer and remote repository | git config --global user.name "NguyenNgoc Due"           |
| Link your github account                                     | git config --global user.email "duengocnguyen@gmail.com" |
| Check config is okay?                                        | git config --list                                        |
|                                                              |                                                          |

***Create Repo***

1. ***Git Init***:

   Create a local Repo in your own PC

   > git init 
   >
   > (Initialized empty Git repository in your computer (local))

   Link the local repository to an empty GitHub repository

   > git remove add origin [GitHub_Repo_URL]
   >
   > (open Github.com/new --> Create a new repository--> get quick link of your repository)
   >
   > git remove add origin https://github.com/....

2. ***Git Clone***

   Clone a Remote Repo on GitHub to Local PC

   >git clone [GitHub_Repo_URL]

---

***Example:***

Step 1: Create a index.html

```html
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>GitHub and GitHub Tutorial</title>
</head>
<body>
    <h1> 10 basic commands any developer have to know </h1>
</body>
</html>
```

**Git Workflow**

![](C:\Users\NGUYEN NGOC DUE\OneDrive\01_Learming Programing Developer\Learning GitHub\git_workflow.png)

3. ***Git Add***

   Add changes to Staging area

   > git add file

   ```Cmd
   git add index.html
   ```

4. ***Git Commit***

   Snapshots the file in preparation for versioning

   > git commit -m "descriptive message"
   >
   > *(if you want to change your descriptive message)*
   >
   > git commit --amend -m "amend descriptive message"

   ```Cmd
   git commit -m "Create a new index.html"
   ```

5. ***Git Push***

   Uploads all local branch commits to GitHub

   > git push origin [branch-name]

   ```Cmd
   git push origin master
   ```

   