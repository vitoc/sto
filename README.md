# Sprint-based Technical Onboarding

This is the approach that I use to onboard someone to a technical developer/architect role.

> This is an opinionated approach with a skew towards Node.js, React, GitHub,  Azure and Office.

## Sprints

### Sprint 1: Version control and Github

* Do: [Hello World!](https://guides.github.com/activities/hello-world/)
* Read: [Understanding the GitHub flow](https://guides.github.com/introduction/flow/)
* Do: [Schedule the next sprint review with Outlook](https://support.office.com/en-us/article/schedule-a-meeting-with-other-people-5c9877bc-ab91-4a7c-99fb-b0b68d7ea94f)

For the last item above, please actually send an invite to your human onboarding guide :) I.e. me :)

### Sprint 2: Collaborating and communicating around code

* Read: [Communicating with Markdown](https://lab.github.com/githubtraining/communicating-using-markdown)
* Read: [Forking projects](https://guides.github.com/activities/forking/)
* Do: Fork this project, replace the bullet points for tasks within this document with ticks on tasks that you'd completed (You can just use the edit functio in GitHub to do this).


### Sprint 3: Getting familiar with VS Code as an IDE

* Do: [Download and install VS Code](https://code.visualstudio.com/download)
* Do: [Clone the **fork (your fork)** of this repository locally using VS Code](https://code.visualstudio.com/docs/editor/versioncontrol#_cloning-a-repository)

### Sprint 4 Be aware of the Integrated Terminal

* Read: [Learn how to bring up the Integrated Terminal in VS Code](https://code.visualstudio.com/docs/editor/integrated-terminal)
* Do: Bring up the Integrated Terminal in your VS Code. In the Bash command line, do:
```
$ git remote add upstream https://github.com/vitoc/stoo.git
```
* From the command line, check for updates from upstream:
```
$ git pull upstream master
```
> From now on, do pull from upstream whenever you start a new sprint to ensure you have the latest tasks and notes.

### Sprint 5 Edit locally and push to remote 

* Do: Continuing from the previous sprint, make a local edit in VS Code by adding the
  keyboard shortcut to open the Integrated Terminal here:
```
REPLACE WITH KEYBOARD SHORTCUT
```
* Do: [Commit and push this back to your forked repository.](https://code.visualstudio.com/docs/editor/versioncontrol#_commit)

### Sprint 6 Node.js and NPM

* Do: [Download and install LTS version of Node.js](https://nodejs.org/en/)
* Do: Check that Node.js is installed
```
$ node --version
```
* Do: Check that NPM is installed
```
$ npm --version
```

### Sprint 7 Understand the Agile manifesto

* Read: [The Agile Manifesto](https://agilemanifesto.org/)
* Read: [Principles behind the Agile Manifesto](https://agilemanifesto.org/principles.html)
* Read: [What is Scrum?](https://docs.microsoft.com/en-us/azure/devops/learn/agile/what-is-scrum)

### Sprint 8 React immersion 

* Do: [Go through (via Codepen) the Step-by-Step Guide to React](https://reactjs.org/docs/hello-world.html)
* Do: [Go through Jason Watmore's NodeJS - JWT Authentication Tutorial with Example API](https://jasonwatmore.com/post/2018/08/06/nodejs-jwt-authentication-tutorial-with-example-api)
* Do: [Go through Json Watmore's React + Redux - JWT Authentication Tutorial & Example](https://jasonwatmore.com/post/2017/12/07/react-redux-jwt-authentication-tutorial-example)

### Sprint 9 Create a front-end

* Do: Clone ```https://github.com/vitoc/rad```
> Please clone this to a separate directory, do not clone this within the ```sto``` directory
* Do: Follow through the Mods in the repository.
> By following the demo, you should arrive at a functional login / logout app

### Sprint 10 

* Do: [Deploy a website to Azure App Service using the VSCode extension](https://code.visualstudio.com/tutorials/app-service-extension/getting-started)
* Do: Apply similar method to deploy ```node-jwt-authentication-api``` to Azure App Service
* Do: Check that your deployed app returns:

```{"message":"Invalid Token"}```

going to the root route. It should return the following going to ```/token``` via GET:

```Cannot GET /token```

This is because ```/token``` only functions with a POST.

> ```app.js``` and ```bin\www``` helps make ```node-jwt-authentication-api``` work on Azure App Service


## Optional and additional resources
* [GitHub Learning Lab](https://lab.github.com/)
* [GitHub Training & Guides](https://www.youtube.com/githubguides)

> This is a WIP
