[![Review Assignment Due Date](https://classroom.github.com/assets/deadline-readme-button-22041afd0340ce965d47ae6ef1cefeee28c7c493a6346c4f15d667ab976d596c.svg)](https://classroom.github.com/a/GvXCZgfk)
[![Open in Visual Studio Code](https://classroom.github.com/assets/open-in-vscode-2e0aaae1b6195c2367325f4f02e2d04e9abb55f0b24a779b69b11b9e10269abc.svg)](https://classroom.github.com/online_ide?assignment_repo_id=15600579&assignment_repo_type=AssignmentRepo)
# SE-Assignment-4
Assignment: GitHub and Visual Studio
Instructions:
Answer the following questions based on your understanding of GitHub and Visual Studio. Provide detailed explanations and examples where appropriate.

Questions:
Introduction to GitHub:

What is GitHub, and what are its primary functions and features? Explain how it supports collaborative software development.
Repositories on GitHub:

GitHub is a cloud-based platform where you can store, share, and work together with others to write code.

Primary functions and features:
1. To showcase and share your work
2. It tracks and manages changes made to code over time
3. It allows others to review your code and make suggestions to improve it
4. It collaborates on a shared project.

How it support collaborative software development
It allows people to collaborate on shared project without worrying that the changes will impact the work of the collaborators before it is ready to be integrated. This collaboration is made possible by the open source software, Git, upon which Github is built


What is a GitHub repository? Describe how to create a new repository and the essential elements that should be included in it.
Version Control with Git:

The Github repositories act as essential places for storing the files with maintaining the versions of development. By using GitHub repositories developers can organize, monitor, and save their changes of code to their projects in remote environments.

How to create a new repository?
1. Login to the Github account
2. Click on new repository at the home page
3. Type a name for the repository and sect either public (anyone on the internet can see this repository)  or private (you choose who can see and commit to this repository)
4. Click create a new repository button
5. Create a readme file to tell more about the repository

   
Explain the concept of version control in the context of Git. How does GitHub enhance version control for developers?
Branching and Merging in GitHub:

A VCS or the Version Control System is used to track versions of the files and store them in a repository. 

Git is a distributed version control system that enables software development teams to have multiple local copies of the project's codebase independent of each other. These copies, or branches, can be created, merged, and deleted quickly, empowering teams to experiment, with little compute cost, before merging into the main branch

What are branches in GitHub, and why are they important? Describe the process of creating a branch, making changes, and merging it back into the main branch.
Pull Requests and Code Reviews:

Branches allow you to develop features, fix bugs, or safely experiment with new ideas in a contained area of your repository.
Branches are important because one can create a new branch from the default branch of the repository. It can then be worked on in isolation from changes that other people are making to the repository.

To create a new branch, use the following command
  
  git branch <branch_name>

To check the brach, use the command
  git branch

To switch to the new branch, use the command
  git checkout <branch_name>

To make changes in the newly created branch, use the command 
git add .

To merge to the main branch, use the command 
git merge <branch-name>

What is a pull request in GitHub, and how does it facilitate code reviews and collaboration? Outline the steps to create and review a pull request.
GitHub Actions:

A pull request is a proposal to merge a set of changes from one branch into another. In a pull request, collaborators can review and discuss the proposed set of changes before they integrate the changes into the main codebase. Pull requests display the differences, or diffs, between the content in the source branch and the content in the target branch.

Steps to create and review a pull request
1. Create a branch
2. Making changes and committing
3. Push the changes
4. Open a pull request
5. Review the pull request
6. Approve and merge
   
Explain what GitHub Actions are and how they can be used to automate workflows. Provide an example of a simple CI/CD pipeline using GitHub Actions.
Introduction to Visual Studio:

GitHub Actions is a continuous integration and continuous delivery (CI/CD) platform that allows you to automate your build, test, and deployment pipeline. You can create workflows that build and test every pull request to your repository, or deploy merged pull requests to production.

Example of a simple CI/CD pipeline
1. create a github/workflos directory in the repo and add a YAML file to define the owrkflow
2. Define workflow actions
3. Trigger workflow on events
4. Test and deploy

E.G
Copy code
name: CI/CD Pipeline

on:
  push:
    branches:
      - main

jobs:
  build:
    runs-on: ubuntu-latest

    steps:
      - name: Checkout Repository
        uses: actions/checkout@v2

      - name: Install Dependencies
        run: npm install

      - name: Run Tests
        run: npm test

      - name: Build Artifact
        run: npm build

      - name: Deploy to Production
        uses: some-deployment-action
        with:
          environment: production
          token: ${{ secrets.DEPLOY_TOKEN }}


What is Visual Studio, and what are its key features? How does it differ from Visual Studio Code?
Integrating GitHub with Visual Studio:
Visual Studio is a powerful developer tool that you can use to complete the entire development cycle in one place. It's a comprehensive integrated development environment (IDE) that you can use to write, edit, debug, and build code. Then deploy your app.

Features:
Comprehensive integrated development environment (IDE) for writing, editing, debugging, and building code.
Modular installation with customizable workloads.
Support for multiple programming languages.
Ability to build cross-platform apps and games.
Connectivity to databases.
Debugging, testing, and code improvement tools.
Deployment of finished applications.
Extensibility through extensions.

Differences between VS and VSCODE
Visual Studio is an integrated development environment (IDE) while Visual Studio Code is a rich text editor
VS takes more space to download but VSCODE takes less space


Describe the steps to integrate a GitHub repository with Visual Studio. How does this integration enhance the development workflow?
Debugging in Visual Studio:

1. Open visual studio
2. open account settings i.e. File>account settings
3. add an account and select Github
4. sign in with github credentials
5. After password authorization, a success message will be displayed

The integration makes workflow easier to push your finished work to the repository online.

Explain the debugging tools available in Visual Studio. How can developers use these tools to identify and fix issues in their code?
Collaborative Development using GitHub and Visual Studio:

Step through code - executing the application code one statement at a time
Using Breakpoint - Breakpoints are most commonly used to interrupt a running program immediately before the execution of a programmer-specified instruction.
Call stack - This shows all methods that have been called at the point when code breaks

Discuss how GitHub and Visual Studio can be used together to support collaborative development. Provide a real-world example of a project that benefits from this integration.

Authenticate your GitHub account to create a repository, and push your first commits to GitHub, all through Visual Studio.
You can clone a Github repository from VS code to start committing and pushing
Take local code and push it to a new repository on GitHub in one step. Visual Studio handles the local and remote repository creation.
Create and switch between branches from the status bar of the VS. View your changes, stage the files you want to commit, and make commits with GitHub
Merge or rebase branches after completing features directly from within Visual Studio. You can also choose  to merge or rebase when pulling, or prune branches when fetching.
Create a pull request from remote branches in the new pull request window. You can add your title, description with Markdown support, reviewers, and see your changes summarized all at once inside Visual Studio.

References:
https://docs.github.com/
https://about.gitlab.com/
https://www.geeksforgeeks.org/
https://dev.to/
https://learn.microsoft.com/
Submission Guidelines:
Your answers should be well-structured, concise, and to the point.
Provide real-world examples or case studies wherever possible.
Cite any references or sources you use in your answers.
Submit your completed assignment by [due date].
