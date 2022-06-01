<h2 align="center">
  firebase-example-api
</h2>
<h5 align="center">
 Backend example developed <br/> using Node.js, Typescript and Firebase.
</h4>

### Technologies

This project was developed, using the following technologies:

- [Node.js](nodejs)
- [TypeScript](https://www.typescriptlang.org)
- [Express](https://expressjs.com)
- [ESLint](https://eslint.org)
- [Prettier](https://prettier.io)
- [Firebase](https://firebase.google.com)

## Tools

These tools were essential for the development of the entire project.

- [VS Code][vc] - Best IDE :)
- [Git CZ](https://github.com/commitizen/cz-cli) - To make this repo Commitizen-friendly
- [Git Flow](https://danielkummer.github.io/git-flow-cheatsheet/index.html) - To improve organization between branches
- [Insomnia](https://insomnia.rest/) - To manage and test api requisitions

## Dependencies

- express
- eslint
- firebase-admin
- firebase-functions

## How To Use

To run this application, you'll need:

- [Git](https://git-scm.com) - To use git commands
- [Node.js v16.13.0][nodejs] or higher - To run this project
- [Yarn v1](https://yarnpkg.com) or higher - To manage the project dependencies

[nodejs]: https://nodejs.org/
[vc]: https://code.visualstudio.com/

After, from your command line:

### Clone this repository using this command

```bash
$ git clone https://github.com/alexandre1921/firebase-example-api
```

### Install the project dependencies in each folder:

```bash
$ yarn
```
Or

```bash
$ yarn install
```

### Setup your emulators
Setup your .firebaserc
- set your default project
- in .firebaserc.example rename to .firebaserc

Setup your runtime variables to use as .env
- in .runtimeconfig.example.json and rename to .runtimeconfig.json

Setup service account to access firebase servers resources instead locally resources
- in .serviceaccount.example.json rename to .serviceaccount.json

### Finally, run your app with yarn dev on project folder

```bash
$ yarn dev
```

### Success 🚀. The app is running in 0.0.0.0:5000.

```bash
i  emulators: Starting emulators: auth, functions, firestore, pubsub
⚠  functions: The following emulators are not running, calls to these services from the Functions emulator will affect production: database, hosting
✔  functions: Using node@16 from host.
i  firestore: Firestore Emulator logging to firestore-debug.log
i  pubsub: Pub/Sub Emulator logging to pubsub-debug.log
i  ui: Emulator UI logging to ui-debug.log
✔  functions[userHelloWorld]: http function initialized (http://0.0.0.0:5001/firebase-example-api/us-central1/userHelloWorld).
✔  functions[getUserByName]: http function initialized (http://0.0.0.0:5001/firebase-example-api/us-central1/getUserByName).
✔  functions[welcomeNewUser]: firestore function initialized.
✔  functions[adminHelloWorld]: http function initialized (http://0.0.0.0:5001/firebase-example-api/us-central1/adminHelloWorld).

┌──────────────────────────────────────────────────────────────┐
│ ✔  All emulators ready! View status and logs at 0.0.0.0:4000 │
└──────────────────────────────────────────────────────────────┘

┌────────────────┬──────────────┬────────────────────────┐
│ Emulator       │ Host:Port    │ View in Emulator UI    │
├────────────────┼──────────────┼────────────────────────┤
│ Authentication │ 0.0.0.0:9099 │ 0.0.0.0:4000/auth      │
├────────────────┼──────────────┼────────────────────────┤
│ Functions      │ 0.0.0.0:5000 │ 0.0.0.0:4000/functions │
├────────────────┼──────────────┼────────────────────────┤
│ Firestore      │ 0.0.0.0:8080 │ 0.0.0.0:4000/firestore │
├────────────────┼──────────────┼────────────────────────┤
│ Pub/Sub        │ 0.0.0.0:8085 │ n/a                    │
└────────────────┴──────────────┴────────────────────────┘
```

### IMPORTANT!!!

To test these routes and update documentation with new ones use [Insomnia](https://docs.insomnia.rest/insomnia/design-documents).
