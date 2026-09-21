#Github Actions Workflow Analysis
## 1. What triggers this workflow to run? 
The workflow runs when code is being pushed to the main branch or when a pull request is created for that branch.
## 2. What are the four main steps this workflow performs? 
    1. **Checkout code**
    2. **Validate HTML**
    3. **Check Links**
    4. **Upload Files**
    5. **After testing you actually deploy to pages**
## 3. What does the "Checkout code" step do and why is it necessary?
It is necessary because that's how you  get the code from the repo for github actions to work. It gets files from the website! it also prepares for deployment
## 4. What is the purpose of the environment configuration?
It basically gets the github pages to work properly and gives a link to the actual page.
## 5. How does this automated deployment improve reliability compared to manual deployment?
The same tests automatically done each time. It reduces the chances of you forgetting a step.
## 6. What would happen if you pushed code to a different branch (not main)?
So the  workflow runs a pull request, the site doesn't change until you push to main. It only deploys when the event is a push to "main".