- [Back to Knowledge Page](https://github.com/monpopza/knowledge/blob/main/README.md)
# Update version 062022
## [Vue.JS Link](https://github.com/monpopza/knowledge/blob/main/create%20Vue.js%203.md)
## [Firebase Link](https://github.com/monpopza/knowledge/blob/main/Firebase.md)

# Setup vueJS, Firebase and Bootstrapvue 2020
> This Document make for 🦖 
## All Document
- [Node.JS](https://nodejs.org/en/)
- [Git-CSM](https://git-scm.com)
- Code Editor (WebStorm, VSCode)
- Browser (Chromium base/Firefox/Safari)
- [Notepad++](https://notepad-plus-plus.org/downloads/)
- [Bootstrao](https://getbootstrap.com)
- [Popper-JS](https://popper.js.org)
- [PortalVue](https://portal-vue.linusb.org)
- [Bootstrap-vue](https://bootstrap-vue.org)

- ### MacOS
   - How to Install NodeJS and NPM on MacOS (https://gist.github.com/nerdenough/d288f2e732637f55f9858070c6b8b15b)
- ### Other
   - TMUX: https://danielmiessler.com/study/tmux/


## Install NodeJS and Git
### For Windows 
- Download NodeJS and install with Link: https://nodejs.org/en/
- Download Git and Install with Link: https://git-scm.com
### For MacOS
#### NEW!!!✨😤 [Node.JS](https://nodejs.org/en/)

#### Install Homebrew
```
/usr/bin/ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"
```
#### Install Git
```
brew install git
```
#### Install NVM
```
curl -o- https://raw.githubusercontent.com/creationix/nvm/v0.33.1/install.sh | bash
```
### Add nvm to bash profile
```
export NVM_DIR="$HOME/.nvm"
[ -s "$NVM_DIR/nvm.sh" ] && . "$NVM_DIR/nvm.sh" # This loads nvm
```
#### Install NodeJS with NVM
```
nvm install node
```
## Install vueJS, git and Firebase
### Install VueJS
```
npm install -g vue @vue/cli 
```
### Install Firebase
```
npm install -g firebase-tools firebase init
```
### Setup Git
```
git commit -m "Add  existing file"
git push origin master
```

## Setup Vue Project
```
vue create project-name
```
```
----------Configuration VUEJS ----------
 Setup VUEJS
Project name: Your-Name-Project
Project Description: Your-Project-Description
Author: Your name
Vue Build:
ESLint: N
Test runner: No test
Nightwatch: No
select >
Check the features needed for your project:
	(*) Babel
	(*) Progressive Web App (PWA) Support (ควรให้เว็บทำงาน offline ได้)
	(*) Router
	(*) Vuex
	(*) CSS Pre-processors
	( ) Linter / Formatter (ตัวบังคับว่า โค้ดต้องมีระเบียบ)
Use history mode for router? (Requires proper server setup for index fallback in production) (Y/n)    Y
Pick a CSS pre-processor (PostCSS, Autoprefixer and CSS Modules are supported by default): > Sass/SCSS (with node-sass)
Where do you prefer placing config for Babel, PostCSS, ESLint, etc.? (Use arrow keys) > In dedicated config file
Save
----------END----------
```

## Setup Firebase
### Firebase Login
```
firebase login
```
### Firebase Initial
```
firebase init
```
```
----------Configuration Firebase----------
> Create firebase folder and use it
firebase login
firebase init
Yes
	? Are you ready to proceed? Yes
	? Which Firebase CLI features do you want to set up for this folder? Press Space to select features, then Enter to confirm your choices. Database: Deploy Firebase Realtime Database Rules, Firestore: Deploy rules and create indexes for Firestore, Functions: Configure and deploy Cloud Functions, Hosting: Configure and deploy Firebase Hosting sites
	? Please select an option: Use an existing project
	? Select a default Firebase project for this directory: yourproject (yourproject)
	? What file should be used for Database Rules? database.rules.json
	? What file should be used for Firestore Rules? firestore.rules
	? What file should be used for Firestore indexes? firestore.indexes.json
	? What language would you like to use to write Cloud Functions? JavaScript
	? Do you want to use ESLint to catch probable bugs and enforce style? No
	? Do you want to install dependencies with npm now? Yes
	? What do you want to use as your public directory? dist
	? Configure as a single-page app (rewrite all urls to /index.html)? Yes
	? Set up automatic builds and deploys with GitHub? (y/N)  YES
	>> //to web and login//
	? For which GitHub repository would you like to set up a GitHub workflow? (forma
	t: user/repository) monpopza/nammonmen
	? Set up the workflow to run a build script before every deploy? (y/N) yes
	Yes and yes
----------END----------
```

### Deploy to Firebase
```
firebase deploy --only hosting 
```

## Configuration
> After Install VUE and Firebase
### Text and File Transfer
```
( Copy Text ) .gitignore (Firebase) >> .gitignore (Project)
( Copy Files ) All File (Firebase, เว้น .gitignore) > Project
```
## Install Componence and Run project
### Install Project
> Run this command to download Important file and build a project 
```
npm install
npm init
```

### Install other Components
```
npm install bootstrap@next portal-vue @popperjs/core bootstrap-vue
Add bootstrap-vue and other
vue add bootstrap-vue portal-vue popperjs
npm install @babel/polyfill intersection-observer
Add This in main.js || app.js
	import BootstrapVue from 'bootstrap-vue'
	import 'bootstrap/dist/css/bootstrap.css'
	import 'bootstrap-vue/dist/bootstrap-vue.css'
	import 'core-js/stable'
	import 'regenerator-runtime/runtime'
	import 'intersection-observer' // Optional
	Vue.use(BootstrapVue)

Add This in index.html
	<!-- Add this to <head> -->
	<!-- Load required Bootstrap and BootstrapVue CSS -->
	<link type="text/css" rel="stylesheet" href="//unpkg.com/bootstrap/dist/css/bootstrap.min.css" />
	<link type="text/css" rel="stylesheet" href="//unpkg.com/bootstrap-vue@latest/dist/bootstrap-vue.min.css" />
	<!-- Load polyfills to support older browsers -->
	<script src="//polyfill.io/v3/polyfill.min.js?features=es2015%2CIntersectionObserver" crossorigin="anonymous"></script>
	<!-- Load Vue followed by BootstrapVue -->
	<script src="//unpkg.com/vue@latest/dist/vue.min.js"></script>
	<script src="//unpkg.com/bootstrap-vue@latest/dist/bootstrap-vue.min.js"></script>
	<meta name="viewport" content="width=device-width, initial-scale=1, shrink-to-fit=no">
```
- [Back to Knowledge Page](https://github.com/monpopza/knowledge/blob/main/README.md)


