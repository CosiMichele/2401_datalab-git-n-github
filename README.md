# Github and Git

![git_def](https://swcarpentry.github.io/git-novice/fig/phd101212s.png) 

We have all been here, taken by the [Software Carpentry Version Control lesson](https://swcarpentry.github.io/git-novice/01-basics.html).

This lesson of the Data Science Tapas Series we are going to explore Git and GitHub, essential tools for the modern scientist. Likely, if you have to work with code or have to use the computer, you may have found yourself in a GitHub repository looking at someone else's code (or on [Stack Overflow](https://stackoverflow.com/)) addressing the issue you are encountering. The initial concept of Git was to give coders a way to save and [branch](https://www.atlassian.com/git/tutorials/using-branches) their code, and later on GitHub gave some of the fundamentals functionalities that allow code to easily be shared with collaborators as well as a myriad of other functionalities.

Here, we are going to go cover some of these basic functionalities, in an effort to help you understand how Git and GitHub can be essential to your work.

## Agenda

- [Git vs GitHub overview](#git-vs-github-overview)
	- [The GitHub Interface](#the-github-interface)
- [Key GitHub Features](#key-github-features)
	- [Repositories](#repositories)
	- [Adding Code to GitHub](#adding-and-modifying-code-in-github)
	- [History](#history)
	- [Forks, Pull Requests and Issues](#forks-pull-requests-and-issues)
- [Version Control]()
	- [Branches]()
- [Connecting Git to GitHub]()
- [The Git Life Cycle]()
- [Definitions]()

## Git vs GitHub Overview

- **Git**: 
    - First developed in 2005, git is a version control software that allows users to make changes and add versions to their code.
	- Changes and versions are saved locally.
	- Accessible through the Shell.

- **GitHub**:
	- First launched in 2008, its main focus is hosting and sharing code.
    - Uses Git version control software. 
	- Changes and versions are saved online (requires an account).
	- Mainly administered through the web (it also has a [desktop app](https://desktop.github.com/)).
    - Acquired by Microsoft in 2018.

![git v hub simplified](https://devmountain.com/wp-content/uploads/2022/01/Gitvs_Github-1a-1.jpg) 
([Source](https://devmountain.com/blog/git-vs-github-whats-the-difference/))

### The GitHub Interface

Since we are talking about making science accessible, we invite you to use GitHub to save and share your code. Please start by creating a GitHub account at https://github.com/. 

Upon creation of your account, you should be able to access your Dashboard. A number of social media like features are presented to you -- these have been added recently and it is up to you to use them or not. These are not the strength of GitHub, but these allow you to keep up to date with some profiles/accounts or repository that you **Star** (follow).

On your personal page, you will be able to add a picture, a description of yourself, and a link to your website. You can also add your location, your organization, and your pronouns. You can have a list of your most important repositories and show off your daily contributions. You are able to customize your profile to your liking.

![img1](https://foss.cyverse.org/assets/github_shot1.png)

Check out [this profile](https://github.com/Gchism94) for a fancier example. 

Outside of its more social media-like dashboard, GitHub has a number of useful features for working with and sharing code. 

## Key GitHub Features 

GitHub gives you the ability to create and manage your **Repositories**, a space were you can add and share your code. A suggestion is to have *one* repository for *one* project. Let's explore the features that come with each Repository.

### Repositories

To create your repository, you can either click the **+** sign on the top right and select New Repository, or within your Repositories page, click the green **New** button.

![img2](https://foss.cyverse.org/assets/git_1.png)

Here, you can choose the name of your own repository, choose to make it private or public, adding a README and a licence. It is **strongly** reccomended that you choose to add an empty README file.

![img3](https://foss.cyverse.org/assets/git_2.png)


**So, why a README?** 

There are two main reasons why you would like a README file:
	
1. It adds structure to your repository *automatically* - otherwise you would need to create said structure by yourself (not recommended for beginners).
2. It is the "default" file that GitHub reads upon opening the repository. It can be treated as the go-to file that explains what the repository is for, what each file does, how to cite your reasearch, amongst other things.


**Adding a Licence**
The addition of a licence can heavily contribute to the shareability of your code. Make sure that whichever licence you choose is in line with your principals as well as your project's. GitHub comes with a list of licences which you can review. It is also common to choose a licence later on!


Ultimately, your new repository should look like the following screenshot. Notice the **LICENCE** document and the **README.md**

![img4](https://foss.cyverse.org/assets/git_3.png)

**Editing the README.md**

The Github repository file has a .md extension which stands for Markdown. Markdown is a lightweight markup language for creating formatted text using a plain-text editor common throughout text files on the web. It uses symbols (*~-#`) for syntaxing text, and it is what GitHub (and this website!) use to format text. Markdown is easier to use than HTML. You can read more on Markdown on the [Markdown Guide](https://www.markdownguide.org/).

### Adding and Modifying Code in Github

GitHub allows you to add and modify code in two ways: 

1. through the online portal (the webpage you're seeing)
2. On your local computer using either the [Desktop Application](https://desktop.github.com/) or the Command Line Interface (CLI).

Adding code to your repository through the web page is suggested if what you want to add is simple (Like a README file!).

- Click the **Add File** button, which will allow you to either create a new file, or upload files from your computer. Select **Create New File**.
- The editing page will open: choose a name and an extension on the top of the page.
- On the editing page you can modify code as you see necessary (writing, pasting)

![img5](https://foss.cyverse.org/assets/git_5.png)

- You can also see your changes (if formatted) with the preview function (with the **Preview** button).
- To "Save" your changes, you will need to **commit** your changes:
	- navigate at the bottom of the page, specify your commit with a name and add a description if necessary.

 ![img6](https://foss.cyverse.org/assets/git_6.png)

- You will be able to see your newly created file on your repository home after **committing** your changes.

### History

**Committing** is the term used for *saving* changes you've made to your code. Each **commit** can be accessed within the GitHub web interface, which will show you the code prior and after the changes you've made. To see a list of all commits you made, click on the clock icon under the **Code** button.

- You can see from the picture below the lines that have been removed (in red), and the lines that have been added (in green).

![img7](https://foss.cyverse.org/assets/git_7.png)

- Additionally, you can also see the full list of commits made to the file or repository.
![img8](https://foss.cyverse.org/assets/git_8.png)

### Forks, Pull Requests and Issues

When you commit changes to your own code, there are no checks that force you to review your code (unless you specify them). However, when someone else wants to add to your code, they need to create a **Pull Request (PR)**. Pull Requests are created upon someone else's commit to your code. These need to be evaluated by you prior to **merging** (allowing the code to be added). You can view Pull Requests in the top menu of your Repository.

**How does someone create a Pull Request? Forks!**

One does so by "Copying" your repository, with an action called **Forking**. Forking creates a copy of your code in someone else's Account/Repository. Ultimately, this collaborator can "ask" to add the code they have worked on to yours by creating a PR. Everyone is able to Fork any public repository!

**But what if I don't want to Fork the code but still want to contribute? Issues!**

If you want to contribute to someone's code, let's say you spotted a bug for example, you can open an **Issue**. Issues are also available at the top of your Repository's menu. Issues can be created by anyone, and these are meant to notify the Repository's maintainer of problems, requests and conversations regarding the code and content.

---
