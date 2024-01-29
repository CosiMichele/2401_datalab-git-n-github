# Github and Git

![git_def](https://swcarpentry.github.io/git-novice/fig/phd101212s.png) 

We have all been here, taken by the [Software Carpentry Version Control lesson](https://swcarpentry.github.io/git-novice/01-basics.html).

This lesson of the Data Science Tapas Series we are going to explore Git and GitHub, essential tools for the modern scientist. Likely, if you have to work with code or have to use the computer, you may have found yourself in a GitHub repository looking at someone else's code (or on [Stack Overflow](https://stackoverflow.com/)) addressing the issue you are encountering. The initial concept of Git was to give coders a way to save and [branch](https://www.atlassian.com/git/tutorials/using-branches) their code, and later on GitHub gave some of the fundamentals functionalities that allow code to easily be shared with collaborators as well as a myriad of other functionalities.

Here, we are going to go cover some of these basic functionalities, in an effort to help you understand how Git and GitHub can be essential to your work.

## Agenda

- [Git vs GitHub overview](#git-vs-github-overview)
- [Version Control]()
	- [Branches]()
- [Key Git Features]()
	- [Issues]()
	- [Pull Requests]()
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
	- Mainly administered through the web (it also has a [desktop app](https://desktop.github.com/){target=_blank}).
    - Acquired by Microsoft in 2018.

![git v hub simplified](https://devmountain.com/wp-content/uploads/2022/01/Gitvs_Github-1a-1.jpg) 
([Source](https://devmountain.com/blog/git-vs-github-whats-the-difference/))

## Introducing GitHub

Since we are talking about making science accessible, we invite you to use GitHub to save and share your code. Please start by creating a GitHub account at https://github.com/.

#### User Profile

Just like in any other social media platform, you can create a profile for yourself. This is where you can add a picture, a description of yourself, and a link to your website. You can also add your location, your organization, and your pronouns. You can have a list of your most important repositories and show off your daily contributions. You are able to customize your profile to your liking. Check out [this profile](https://github.com/Gchism94) for fancy example. 

![github_shot1](assets/github_shot1.png)

<br/>

#### Search

At the top of most pages, is a search bar. Use this to find repositories, users, and organizations. You can also use it to search for specific code within a repository.
![github_shot1](assets/github_shot2.png)

<br/>

#### Starring Repositories

You can star repositories that you like. This is a way to bookmark repositories that you want to come back to later. You can also use this to show your appreciation for a repository. You can see all of your starred repositories by clicking on your profile picture and then clicking on **Your stars**.

![github_shot1](assets/github_shot3.png)

<br/>

#### Create Your Own Repository

Repositories are where your code is stored. A suggestion is to have *one* repository for *one* project.

You can create repositories by clicking on the **Repositories** tab, and then clicking **New**.

![git_1](assets/git_1.png)

Here, you can choose the name of your own repository, choose to make it private or public, adding a README and a licence. It is **strongly** reccomended that you choose to add an empty README file.
<br/>
<br/>

![git_2](assets/git_2.png)

<br/>


!!! Info "So, why a README?"
    There are two main reasons why you would like a README file:
        
    1. It adds structure to your repository *automatically* - otherwise you would need to create said structure by yourself (not recommended for beginners).
    2. It is the "default" file that GitHub reads upon opening the repository. It can be treated as the go-to file that explains what the repository is for, what each file does, how to cite your reasearch, amongst other things.


!!! Info "Adding a Licence"
    The addition of a licence can heavily contribute to the shareability of your code. Make sure that whichever licence you choose is in line with your principals as well as your project's. GitHub comes with a list of licences which you can review. It is also common to choose a licence later on! We will cover licences in more depth [later](03_managing_data.md#licences) in the course.

<br/>


Ultimately, your new repository should look like the following screenshot. Notice the **LICENCE** document and the **README.md**

![git_3](assets/git_3.png)

!!! Info "Editing the README.md"
	The Github repository file has a .md extension which stands for Markdown. Markdown is a lightweight markup language for creating formatted text using a plain-text editor common throughout text files on the web. It uses symbols (*~-#`) for syntaxing text, and it is what GitHub (and this website!) use to format text. Markdown is easier to use than HTML. You can read more on Markdown on the [Markdown Guide](https://www.markdownguide.org/).

<br/>
<br/>

### Adding and Modifying Code in Github

GitHub allows you to add and modify code in two ways: 1. through the online portal (the webpage you're seeing), and 2. On your local computer. Throughout the following section, we will show you how to do it through the online portal. We will save the local computer for later for [Lesson 5](05_version_control.md) later in the course. 


Adding code to your repository through the web page is suggested if what you want to add is simple (Like a README file!).

- Click the **Add File** button, which will allow you to either create a new file, or upload files from your computer. Select **Create New File**.
- The editing page will open: choose a name and an extension on the top of the page.
- On the editing page you can modify code as you see necessary (writing, pasting)

![git_05](assets/git_5.png)

- You can also see your changes (if formatted) with the preview function (with the **Preview** button).
- To "Save" your changes, you will need to **commit** your changes:
	- navigate at the bottom of the page, specify your commit with a name and add a description if necessary.
 ![git_06](assets/git_6.png)
- You will be able to see your newly created file on your repository home after committing your changes.

!!! info "Committing changes"
	**Committing** is the term used for *saving* changes you've made to your code. Each **commit** can be accessed within the GitHub web interface, which will show you the code prior and after the changes you've made. To see a list of all commits you made, click on the :fontawesome-solid-clock-rotate-left: icon under the **Code** button.

	- You can see from the picture below the lines that have been removed (in red), and the lines that have been added (in green).
	![git_07](assets/git_7.png)

	- Additionally, you can also see the full list of commits made to the file or repository.
	![git_08](assets/git_8.png)
<br/>

#### Hosting Web Pages in Github

GitHub allows you to host web pages through the use of **GitHub Pages**. This is a free service that allows you to host a website directly from your GitHub repository. You can use this to host your personal website, or to host a website for your project.

For example, the [FOSS website](https://foss.cyverse.org/) is hosted through GitHub Pages. The repository for the website can be found [here](https://github.com/CyVerse-learning-materials/foss)


---
