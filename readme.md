# Welcome to the Anythink Market repo

To start the app use Docker. It will start both frontend and backend, including all the relevant dependencies, and the db.

Please find more info about each part in the relevant Readme file ([frontend](frontend/readme.md) and [backend](backend/README.md)).

## Development

When implementing a new feature or fixing a bug, please create a new pull request against `main` from a feature/bug branch and add `@vanessa-cooper` as reviewer.

## First setup

**[TODO 05/01/2018 @vanessa-cooper]:** _It's been a while since anyone ran a fresh copy of this repo. I think it's worth documenting the steps needed to install and run the repo on a new machine?_

## Setting Up a local environment
 1 Clone the provide repository to your local machine and open it using your favorite code editor

2 Add a file i.e CODEOWNERS file to your local repository

3 Initialize your git by using git init and create a new branch using the following command: git branch {branch name} and switch to it using git checkout {branch name}, where {branch name} is a name of our choice.
A shorter method to create branch and switch to it is using the -b flag e.g git checkout -b {branch name}

4 Add a file to the root directory by using the command git add {file name}

5 Commit your change using git commit -m "commit message".
 Push it to git hub using 
 git push -u origin {branch name} or git push {repository url} {branch name}

6 Make a github pull request (PR) using  git request-pull {repository url} {branch name} 
Use github desktop for easier and faster experience.

After You request has been successfully reviewed and given a go-ahead, you can merge it to the main.

If you are asked to remove a certain line of code e.g removing @carl from CODEOWNERS, just delete it, add the file via git add {file name}, commit the change and make a pull request

7 To enable Backend and frontend, install docker and after a sequence of simple setups, run the following command to confirm if Docker has been installed: docker -v  to check version, docker-compose

8 Then run docker-compose up in your root repository to load backend and frontend  and connect to your local database. 

 9 Incase of bugs, update the node modules using npm i npm@latest
 If it is a mongo error regarding compatiblity with your devise, degrade the mongodb version to mongo: 4.4.6 [worked at the time of writing this]
 and everything should run as intended.

 10 Use docker-compose up command to run all scripts on one of the containers you created, you can use docker exec command to run commands on a running container