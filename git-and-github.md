![GeneralAssemb.ly](http://fewd.in/img/icons/FEWD_Logo.png)

#FEWD - Git and GitHub

###Jesse Shawl

<jesse@jshawl.com> &bull; [@jshawl](https://twitter.com/jshawl)

---

## Agenda

1. Create a local repo and start tracking changes
2. Make some commits
3. Publish your project to http://username.github.io/
4. Understand branching and project pages.

---

## Git

![](http://git-scm.com/images/logos/downloads/Git-Icon-1788C.png)

### What is Git?

Git is a distributed version control system.

-v-

### A little Configuration


    $ git config --global user.name "Your Name Here"
    # Sets the default name for git to use when you commit
    
    $ git config --global user.email "your_email@example.com"
    # Sets the default email for git to use when you commit

-v-

### Navigate to Project

![](https://s3.amazonaws.com/quickcast/1272/13651/quickcast.gif)

`git init`

`git status`

-v-

### Initial Commit

Add files to the staging area:

`git add`

Check out the status:

`git status` 

Make a commit:

`git commit -m "Your commit message"`

-v-

### What Just Happened?

![](http://git-scm.com/figures/18333fig0201-tn.png)

-v-

### Making More Commits

Go on, make some changes. When you're ready to commit,
Add them to the staging area: 

`git add .`

And make the commit 

`git commit -m 'your message'`

-v-

### When to Commit

Git is like a time machine. I make a commit for any point in time I want to be able to revert back to.

-v-

### Viewing the commit history

To see your commits:

`git log`

or my favorite

`git log --all --decorate --graph --pretty --oneline`

More info - http://git-scm.com/book/en/Git-Basics-Viewing-the-Commit-History

-v-

### Staging deleted files

`git add --all :/`

-v-

### Questions?

---

## GitHub

![](https://dl.dropboxusercontent.com/u/216146956/Octocat.png)

GitHub is not Git. Git came before GitHub. It's a social coding network.
But really, it's a place where you can host your repositories.

-v-

### Your First Remote Repo

Head over to github.com and create a new repo, called yourgithubusername.github.io

Copy the clone URl. should be https://...

-v-

### Link the local repo with the remote

    git remote add origin https://clone_url_here/

-v-
    
### Push your code to GitHub

After you've made some commits, push your code to GitHub:

    git push origin master
    
`origin` is the name of the remote repository. We chose that name in the previous step.

`master` is the name of the branch you were working on. More on this soon.

-v-

### Creating a Project Page

You might want to have a separate repo for other projects on your GitHub account, that are accessible at either your own domain or http://username.github.io/project-name/

Create _another_ new repo on github.com

-v-

### Clone the url

    git clone https://github.com/username/project-name.git
    
and move into that directory

    cd project-name

-v-
    
### Create a new branch

In order for github pages to display your content in a project page, you must push your code to the gh-pages branch.

Create the gh-pages branch locally:

    $ git checkout -b gh-pages

-v-
    
### Make some more commits:

    $ git add .
    $ git commit -m 'My awesome commit message'
    
-v-

### Push your code to github

    $ git push origin gh-pages

-v-
    
### View your project in the browser

visit http://username.github.io/project-name/

-v-

### Using your own domain

You can use GitHub pages with your own domain, too! 

To do this, you'll need to create a file called CNAME, with its contents being your domain name.

Also, you'll need to configure the DNS to point to GitHub.

More info here - https://help.github.com/articles/setting-up-a-custom-domain-with-pages

-v-

### Questions? 

-v-

## Further Resources

- http://git-scm.com/book
- http://try.github.io/
- http://gitready.com/




