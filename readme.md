# Welcome to the Anythink Market repo

To start the app use Docker. It will start both frontend and backend, including all the relevant dependencies, and the db.

Please find more info about each part in the relevant Readme file ([frontend](frontend/readme.md) and [backend](backend/README.md)).

## Development

When implementing a new feature or fixing a bug, please create a new pull request against `main` from a feature/bug branch and add `@vanessa-cooper` as reviewer.

## First setup

**[TODO 05/01/2018 @vanessa-cooper]:** _It's been a while since anyone ran a fresh copy of this repo. I think it's worth documenting the steps needed to install and run the repo on a new machine?_

Step 1: Install Docker. Learn how [here](https://docs.docker.com/get-docker/)
Step 2: After completing installation, verify if docker is ready by running the following commands in the terminal: `docker -v` and `docker-compose -v`.
Step 3: Run `docker-compose up` in the terminal of the project root directory to load Anythink's backend and frontend. If docker is working perfectly, the backend should be running and be able to connect to the local database. Test this out by pointing it to [http://localhost:3000/api/ping](http://localhost:3000/api/ping). It should return a success json.
Step 4: If the frontend is working correctly, then you should be able to create a new user on [http://localhost:3001/register](http://localhost:3001/register)
Step 5: Make sure to run all the scripts in the next quests on one of the containers created by `docker-compose up`. Also, you can use `docker exec` to run commands on a running container.
