# Sprint-based Technical Onboarding Objectives

Get technically onboarded to the Microsoft Azure approach to field-based development work in 6 sprints :)
Each sprint is planned for a week. We review the onboarding outcome on the Thursday of every week, and set about 
talking about the next sprint if all is well.

## Sprints

### Sprint 1: Version control and Github

- [x] Do: [Hello World!](https://guides.github.com/activities/hello-world/)
- [x] Read: [Understanding the GitHub flow](https://guides.github.com/introduction/flow/)
- [x] Do: [Schedule the next sprint review with Outlook](https://support.office.com/en-us/article/schedule-a-meeting-with-other-people-5c9877bc-ab91-4a7c-99fb-b0b68d7ea94f)

For the last item above, please actually send an invite to your human onboarding guide :)

### Sprint 2: Collaborating and communicating around code

- [x] Read: [Communicating with Markdown](https://lab.github.com/githubtraining/communicating-using-markdown)
- [x] Read: [Forking projects](https://guides.github.com/activities/forking/)
- [x] Do: Fork this project, replace the bullet points for tasks within this document with ticks on tasks that you'd completed

### Sprint 3: Getting familiar with VS Code as an IDE

- [x] Do: [Download and install VS Code](https://code.visualstudio.com/download)
- [x] Do: [Clone the **fork (your fork)** of this repository locally using VS Code](https://code.visualstudio.com/docs/editor/versioncontrol#_cloning-a-repository)

### Sprint 4 Be aware of the Integrated Terminal

- [x] Read: [Learn how to bring up the Integrated Terminal in VS Code](https://code.visualstudio.com/docs/editor/integrated-terminal)
- [x] Do: Bring up the Integrated Terminal in your VS Code. In the Bash command line, do:
```
$ git remote add upstream https://github.com/vitoc/stoo.git
```
- [x] From the command line, check for updates from upstream:
```
$ git pull upstream master
```
> From now on, do pull from upstream whenever you start a new sprint to ensure you have the latest tasks and notes.

### Sprint 5 Edit locally and push to remote 

- [x] Do: Continuing from the previous sprint, make a local edit in VS Code by adding the
  keyboard shortcut to open the Integrated Terminal here:
```
{
  "key": "ctrl+`",
  "command": "workbench.action.terminal.sendSequence",
  "args": { "text": "\u001b[1;5D\u0060" }
}
```
- [x] Do: [Commit and push this back to your forked repository.](https://code.visualstudio.com/docs/editor/versioncontrol#_commit)

### Sprint 6 Create a front-end

- [ ] Do: Clone ```https://github.com/vitoc/react-redux-jwt-authentication-example.git```
> Please clone this to a separate directory, do not clone this within the ```stoo``` directory
- [ ] Do: Rename the project directory to ```stoo-frontend```
- [ ] Create a repository on GitHub named ```stoo-front-end```
- [ ] Add the created repository as a remote on your local ```stoo-frontend```


## Optional and additional resources
* [GitHub Learning Lab](https://lab.github.com/)
* [GitHub Training & Guides](https://www.youtube.com/githubguides)

> This is a WIP
