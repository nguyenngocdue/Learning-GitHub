# Learning Github

![](C:\Users\NGUYEN NGOC DUE\OneDrive\01_Learming Programing Developer\Learning GitHub\Picture\TXvLy.png)



***Code:***

***Only people who use new install git version control not ever git version***

|                                                              |                                                          |
| ------------------------------------------------------------ | -------------------------------------------------------- |
| Check Version of GitHub:                                     | git version                                              |
| Connection between local repo in your computer and remote repository | git config --global user.name "NguyenNgoc Due"           |
| Link your github account                                     | git config --global user.email "duengocnguyen@gmail.com" |
| Check config is okay?                                        | git config --list                                        |
|                                                              |                                                          |

> git config
>
> ![](C:\Users\NGUYEN NGOC DUE\OneDrive\01_Learming Programing Developer\Learning GitHub\Picture\gitconfig.PNG)

***Create Repository***

1. ***Git Init***:

   Create a local Repo in your own PC

   > > git init 
   >
   > (Initialized empty Git repository in your computer (local))

   Link the local repository to an empty GitHub repository

   > *(add remote repo in local repo)*
   >
   > > git remove add origin [GitHub_Repo_URL]
   >
   > (open Github.com/new --> Create a new repository--> get quick link of your repository)
   >
   > ![](C:\Users\NGUYEN NGOC DUE\OneDrive\01_Learming Programing Developer\Learning GitHub\Picture\CreateRepository.PNG)
   >
   > *My quick repository link: https://github.com/nguyenngocdue/Learning-GitHub.git *
   >
   > > git remote add origin https://github.com/....

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

![](C:\Users\NGUYEN NGOC DUE\OneDrive\01_Learming Programing Developer\Learning GitHub\Picture\git_workflow.png)

3. ***Git Add***

   Add changes to Staging area

   > > git add file
   >
   > ```Cmd
   > git add index.html
   > ```
   >
   > ![](C:\Users\NGUYEN NGOC DUE\OneDrive\01_Learming Programing Developer\Learning GitHub\Picture\git_add_index.png)

   

4. ***Git Commit***

   Snapshots the file in preparation for versioning

   > > git commit -m "descriptive message"
   >
   > *(if you want to change your descriptive message)*
   >
   > ```Cmd
   > git commit -m "Create a new index.html"
   > ```
   >
   > ![](C:\Users\NGUYEN NGOC DUE\OneDrive\01_Learming Programing Developer\Learning GitHub\Picture\git_commit_.m.png)
   >
   > > git commit --amend -m "amend descriptive message"
   >
   > ```html
   > // add <h2> </h2>
   > <html lang="en">
   > <head>
   >     <meta charset="UTF-8">
   >     <meta http-equiv="X-UA-Compatible" content="IE=edge">
   >     <meta name="viewport" content="width=device-width, initial-scale=1.0">
   >     <title>GitHub and GitHub Tutorial</title>
   > </head>
   > <body>
   >     <h1> 10 basic commands any developer have to know </h1>
   >     <h2>You can do anything if you know Github</h2>
   > </body>
   > </html>
   > ```
   >
   > ```cmd
   > git commit --amend -m "Add <h2>Text</h2> "
   > ```
   >
   > ![](C:\Users\NGUYEN NGOC DUE\OneDrive\01_Learming Programing Developer\Learning GitHub\Picture\git_commit_amend_01.png)
   >
   > ![](C:\Users\NGUYEN NGOC DUE\OneDrive\01_Learming Programing Developer\Learning GitHub\Picture\git_commit_amend_02.png)

   

5. ***Git Push***

   Uploads all local branch commits to GitHub

   ![](C:\Users\NGUYEN NGOC DUE\OneDrive\01_Learming Programing Developer\Learning GitHub\Picture\gitPush.png)

   > > git push origin [branch-name]
   >
   > ```cmd
   > git push origin master
   > ```
   >
   > ![](C:\Users\NGUYEN NGOC DUE\OneDrive\01_Learming Programing Developer\Learning GitHub\Picture\git_push_origin_master.png)
   >
   > ![](C:\Users\NGUYEN NGOC DUE\OneDrive\01_Learming Programing Developer\Learning GitHub\Picture\check_git_push.PNG)

   

   change contents in index.hmtl

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
       <p> Detail Guide how to use the basic commands on GitHub  </p>
   </body>
   </html>	
   ```

   >git add.
   >
   >*(changes will be added in Staging Area)*

   > git commit  -m "I just upadte some chages in index.html file"
   >
   > git commit --amend -m "Change H1 to H2, add <p>"

