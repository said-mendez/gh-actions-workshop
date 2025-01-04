# gh-actions-workshop

## Context
This repository contains 2 applications

- A react app using node 22 
- A java api using gradle with gradle wrapper with java 17

**_NOTE:_** You do not need to run this applications locally, they are use in the workshop to have some real examples to run with github actions

## Workshop steps

1. Create a folder in the root called .github/workflows (if doesn't exist)
2. Create a file named ```CI_backend.yml``` and another one names ```CI_frontend.yml``` these files will contain the workflows for the ci of the backend and front end
3. Follow along in the creation of them, they will include
  - a name
  - the events to trigger the workflow (push and pull request)
  - the paths to only trigger it if the folder of the back or the front, respectively was modified
  - env variables
  - defaults set up (working-directory)
  - the jobs,
    * for the backend only a job that builds the java applicatioin
    * for the front end 2 jobs, one to build the application and another one that runs the tests 
