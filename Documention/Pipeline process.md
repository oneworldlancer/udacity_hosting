## Pipeline Process

## DEV

- First DEV creates RDS manually to be able to connect to EB when active, SETUP confirgration in APP

## REPO

- DEV creates a new REPO on GITHUB, then PUSH the data from local-PC to to GITHUB using Git Commands

## CircleCI (CCI)

- Checks if the REPO changed then it starts processing the build-test-deploy steps to be able to PUSH the new data to AWS
- Building an app just creates its final build that work on browsers
- Testing the app to check if there is any errors inside it - if there is any error - it wpn't proceed 
- CCI PUSH backend data to Elastic beanstalk
- CCI PUSH frontend data to S3 Storage
- CCI saves secret ENV data
