_Hello Everyone_

This repository demonstrates the integration of swagger in an existing Serverless Framework Project (Provider: AWS)

_Documentation link_: https://www.serverless.com/plugins/serverless-aws-documentation

**Steps to clone/execute this repository in your local machine**

1) Install Serverless CLI. After successful installation run the below command in your terminal:
    `satyaki@shaw:~$ sls --version` <br /><br />
    _Framework Core: 2.2.0 <br />
    Plugin: 4.0.4 <br />
    SDK: 2.3.2 <br />
    Components: 3.1.4_

2) Install AWS CLI. After successful installation run the below command in your terminal:
   `satyaki@shaw:~$ aws` <br /><br />
   _usage: aws [options] <command> <subcommand> [<subcommand> ...] [parameters] <br />
   To see help text, you can run: <br />
   
     aws help <br />
     aws <command> help <br />
     aws <command> <subcommand> help <br />
   aws: error: the following arguments are required: command_

3) Go to AWS IAM and create a user with Admin Access (Console and Programmatic both) and then configure <br />
    using this command: `satyaki@shaw:~$ aws configure`

4) Clone the repository on you machine: `git clone https://github.com/Satyaki-Roy/integrating-swagger-serverless-nodejs`

5) Install the dependencies: `npm i` or `npm install`

6) Deploy the serverless stack: `sls deploy -v` or `serverless deploy -v`

7) Extract the swagger documentation from AWS, using the below command: <br />
    `serverless downloadDocumentation --outputFileName=filename.ext` or <br />
    `sls downloadDocumentation --outputFileName=filename.ext` <br />
    
   Specify the ext as `.json` or `.yaml` or `.yml`

8) Open Swagger editor (https://editor.swagger.io/) and import the file which was generated using the above command.
