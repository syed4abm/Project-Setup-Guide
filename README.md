# Project Setup Guide - Initially Targeting Windows Users (Frontend Developer)

## Install NodeJs

Visit `https://nodejs.org/en` and download and install the LTS version

## Install NVM

Visit `https://github.com/coreybutler/nvm-windows#install-nvm-windows`

Follow the instructions.

## Switch to required NodeJs version
`nvm use 14.17.3`

---
---

## Clone Github Repository 

Create a new folder at appropriate location on your machine.

Open bash shell and clone the repo with below code syntax:

`git clone -b fix/step-fixes https://github.com/abmerp/UpyogHR.git`

OR

`git clone -b fix/patwari-field-changes https://github.com/abmerp/UpyogHR.git`

once cloned it will create a folder named `UpyogHR`.

## Project folder - Frontend Developers

Folder to work on: `UpyogHR/frontend/micro-ui/web/micro-ui-internals`

Open VS Code on this path.

This is our project's Root Folder `micro-ui-internals`

---
---

## Install Yarn

Run this command in bash shell `npm install --global yarn`

## Check installation

Check that Yarn is installed by running:

`yarn --version`

---
---

### Add yarn.lock file at project root folder (file provided with this setup guide.)

### Add .env file inside examples folder (file provided with this setup guide.)

---
---

## Install project dependencies

First check node version

`node -v`

Then run this command

`yarn install`

if you face issue with node engine you can try below command

`yarn install --ignore-engines`

## Run the application

`yarn start`

OR

`yarn start:dev`

OR - if you face cache issue 

`yarn start -c`
`yarn start:dev -c`


## Final Note

Once application started successfully make some UI/text changes in code and verify it in the browser.

## If you get Heap Memory issue

Run this command before running the app.

`export NODE_OPTIONS=--max_old_space_size=8096 #8GB`
