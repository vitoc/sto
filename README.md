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

### Sprint 10b (Optional)

This is an optional sprint to take if you're keen to run your the app on the App Service instance from the previous sprint optimally 24/7

* Read: Azure App Service plan overview (https://docs.microsoft.com/en-us/azure/app-service/overview-hosting-plans)
* Do: Change the pricing tier for the App Service plan that the instance in the previous sprint reside in from F1 (free) to B1.

### Sprint 11

* Do: [Deploy a static website to Azure](https://code.visualstudio.com/tutorials/static-website/getting-started)
* Do: Build ```react-redux-jwt-authentication-tutorial-example```. Within the directory:

```
$ npm run build
```
* Do: Apply similar method to deploy ```react-redux-jwt-authentication-tutorial-example``` to Azure Storage

> You may need to do ```npm install -g webpack-cli``` if this isn't already installed

### Sprint 12

* Do: Obtain the URL of the deployment from the previous sprint:

![Storage website](/images/storage_website.PNG)

* Do: Replace the ```frontendUrl``` in  ```config.json``` of ```node-jwt-authentication-api``` with the URL from the previous sprint AND path ```/login``` postfixed.
* Do: Deploy ```node-jwt-authentication-api``` again to the appropriate Azure App Service

### Sprint 13

* Read: [Hosting a React JS single page application on Azure Blob Storage & Azure CDN for SSL and to rewrite client routing traffic to the default document](https://medium.com/@antbutcher89/hosting-a-react-js-app-on-azure-blob-storage-azure-cdn-for-ssl-and-routing-8fdf4a48feeb)
* Do: Add a CDN to the deployment in Sprint 12, configure the endpoint and rules as per above

![Custom origin](/images/CustomOrigin.PNG)

* Please: Wait for 5 hours before the added endpoint and the rules to propagate
* Do: Change the ```frontendUrl``` in ```config.json``` from ```node-jwt-authentication-api``` to use the login URL with the new CDN-based URL from the previous sprint in place. I.e. if you have the value of ```frontendUrl``` as ```https://fkycstatic.z23.web.core.windows.net/login```, this should now be ```https://fkyc.azureedge.net/login```.

> Make sure the ```/login``` route is in place!


## Optional and additional resources
* [GitHub Learning Lab](https://lab.github.com/)
* [GitHub Training & Guides](https://www.youtube.com/githubguides)

> This is a WIP
