# Lab - Class 16 (built with lab 01; see below)

## Project: AWS Cloud Servers -- Deploy a server via Elastic Beanstalk

### Author: Nathan Cox

### Links

- [GUI Deploy](http://cf401lab16-env.eba-tmmz2p7h.us-east-2.elasticbeanstalk.com/)
- [CLI Deploy](http://server-deployment-practice-dev.us-west-2.elasticbeanstalk.com/)

### Process

#### Deploying via GUI

- zip up server files sans node_modules and .env
- navigate to elastic beanstalk
- click on create application
- choose node.js as your platform (opting for the latest version)
- upload zipped files
- click create application
- if health check passes, click on your application's url

#### Deploying via CLI

- Update brew
- download AWS
- eb init
- eb create
- follow prompts (defaults)
- beware of using code-commit, because it might throw an insurmountalbe type error
- eb deploy
- eb open

---

# LAB - Class 01

## Project: Server Deployment Practice

### Author: Nathan Cox

### Links and Resources

- [ci/cd](https://github.com/nathanrhead/server-deployment-practice/actions)
<!-- - [back-end server url](http://xyz.com) -->
- [front-end application](https://natecox-server-deploy-prod.herokuapp.com/)

### Setup

#### `.env` requirements (where applicable)

i.e.

- PORT=3001
<!-- - `MONGODB_URI` - URL to the running mongo instance/db -->

#### How to initialize/run your application (where applicable)

- `npm start` or `nodemon`.

#### How to use your library (where applicable)

#### Tests

- How do you run tests?: the tests were written by CF; the tests were run on the command line: npm test.
- Any tests of note? (Possibly too specific to be useful.)
- Describe any tests that you did not complete, skipped, etc.: my code initially didn't pass tests 3 (error handling) and 4, but copying the demo code EXACTLY--and only the code that was pushed to GitHub around four or five o'clock--made the tests past. We had to do some sleuthing to get the code base to deploy on heroku.
