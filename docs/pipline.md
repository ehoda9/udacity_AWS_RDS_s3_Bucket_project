# Introduction

there are too many pipline platforms but in this app we will use [CircleCI]

- why use CircleCI ?
  because CircleCI setup&build and deploy servers so fast!
  also realtime watching for any new updates in our files
  we can too setup environment variables in CircleCI GUI

### How pipline work ?

We imagine that we have a team of developers working on a project
For example, we have a project repo in the Github platform
We associate this repo with the circleci
then upload the project files and then tell the pipline the tasks required of it in this project, for example uploading the project to our hosting and deploy it
The good thing is that circleci does these tasks at once without typing many commands
As we mentioned earlier, this platform monitors our repo in the event that there is any push request or any update in our repo, then it automatically returns these tasks automatically without the need to retype commands
You can learn more by reading the [docs](https://circleci.com/docs)

# steps to work

- first CircleCI read `.circleci/config.yml` file to know what pipline jobs will exactly do in our project we have 2 jobs [Frontend-Deploy & Backend-Deploy]
- second we will link our repo to CircleCI And do the tasks that we wrote in a file `.circleci/config.yml`
- third run CircleCI .

## CircleCI

- backend

##### Note : we can see all scripts in `udagram-api/package.json`

CircleCI will run build script , exports all environment variables from CircleCI configuration then runs deploy script Then uses AWS CLI to upload archive to S3.

- Frontend
  CircleCI will run build script , Then uses AWS CLI to upload assets to S3.

##### Note : we can see all scripts in `udagram-frontend/package.json`
