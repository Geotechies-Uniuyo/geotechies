# Contribution

This 

## Git Workflow
Here is the proposed git flow for contributors:

For every feature, bug or chore, you must create a branch.

**Example for a feature**  
Create a new branch, your branch name must follow this convention: 

naming: feat/user-login 
```
git checkout -b feat/user-login 
```
**Use lower case and separated by dashes**  
Example of a bug ?
Home Page Typo: Your branch naming: bug/homepage-typo

Example of a chore ?
Update Read Me: Your branch naming: chore/update-readme

Once you are assigned a task on clubhouse, create a branch on your local git and only push to that branch. 
If you push to any other branch, you will be heavily penalized.

A typical way to do so:
run: git pull origin develop - You must pull from develop before or after checkout
git checkout -b feat/user-login - You are in the feat/user-login branch now

To push to github;
git add .
git commit -m "feat: implemented user login
git push origin feat/user-login - note how it ends with a branch. 


on github, you must make a PR to the develop branch, any PR to the master branch must be closed with immediate alacrity.

When making a PR, your PR is expected to have the following:
What is the task completed ?
What the PR actually does  ?
How can this PR be manually tested ?
Any background contexts ? (maybe something a tester might not notice and be useful for testing)
Screenshots (of your implementation - a web page, a mobile app screen or an API payload

Your commit messages should follow a consistent pattern:
Remember, chore, feature, bug
So i do not want to see stuff like I tried my best in your commit messages;
For a feature: git commit -m "feat: implemented user log-in
For a bug: git commit -m "bug: fixed inconsistency in log in screen"
For a chore: git commit -m "chore: updated read me to include API endpoints"