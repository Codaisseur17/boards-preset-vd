# boards-preset-vd

vd preset for the [Boards CLI](https://github.com/SpoonX/boards-cli).

## Installing

`yarn add -D boards-preset-vd` or `npm i boards-preset-vd --save-dev`

## Tasks

This preset adds the following tasks to your project.

### vd:tasks

Outputs all available tasks for this preset. Could be useful if you don't have the README handy.

## License

MIT


Videodock React Redux Boilerplate
Development rules
When working on this project, keep these in mind:

Use yarn.
Use the boards-cli to generate uniform code.
Follow the commit guidelines documented.
Run the playbook through yarn storybook
Run the tests through yarn test
Lint through yarn lint
Getting started
Clone repo
yarn global add boards-cli
yarn to install dependencies
yarn start
(Optional) copy .env.local.dist to .env.local for local configuration.
(Optional) copy .npmrc.dist to .npmrc for deploys.
Structure
This application uses Redux, Redux saga, apisauce and seamless-immutable.

Boards.js
Using the boards command you can quickly scaffold boilerplate code. This project uses the vd preset. You can find the available commands there.

Create a React Component
Create a Button.jsx component will all related files:

$ boards vd:component button

Create a React Container
Create a connected Cinema.jsx component will all related files:

$ boards vd:container cinema

Create a Screen
Essentially the same as a container, but separated and only used in <Route /> components.

$ boards vd:screen about

Create a redux structure
$ boards vd:redux about

Create a redux action
Creates an action creator, reducer and type for a single action:

$ boards vd:action about type:findRetweets

Create a redux api
Creates multiple action creators, reducers and types for three actions: findRetweets, findRetweetsSuccess, findRetweetsFailure. This is mostly used in combination with a fetch in sagas. This requires the about sagas to be created first.

$ boards vd:api about type:findRetweets

Create sagas
$ boards vd:sagas about

Create a saga
$ boards vd:saga about type:findRetweets

.env files
The .env files are used to set environment variables for the application for your machine, production, dev and / or test.

Read more.

Services
The services directory is where you put arbitrary workers such as api calls and localstorage access.
