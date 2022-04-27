- Back to Vue.JS Version 3
- https://github.com/monpopza/knowledge/blob/main/create%20Vue.js%203.md
# Create Firebase and Setup a Firbase Project file
## Docunment 
> https://github.com/monpopza/knowledge/blob/main/setup-vuejs-with-firebase.md

## Setting in Windows
> Use Terminal as Administrator
```
Set-ExecutionPolicy Unrestricted 
```
> if you use a cmd you can skip this step cause my terminal use a powershell 🐚

## Install Firebase 
```
npm install -g firebase-tools firebase init
```
> If npn warn bout deprecate somthing dont worry npm just said about security bug something

## Login Firebase
```
firebase login
```
> after that program will be quesion to you
```
i  Firebase optionally collects CLI usage and error reporting information to help improve our products. 
Data is collected in accordance with Google's privacy policy (https://policies.google.com/privacy) 
and is not used to identify you.

? Allow Firebase to collect CLI usage and error reporting information? Yes
i  To change your data collection preference at any time, run `firebase logout` and log in again.

Visit this URL on this device to log in:
https://accounts.google.com/******LOGIN URL******

Waiting for authentication...

+  Success! Logged in as YOUR@EMAIL.MAIL
```

## Create File Firebae
```
firebase init

     ######## #### ########  ######## ########     ###     ######  ########
     ##        ##  ##     ## ##       ##     ##  ##   ##  ##       ##
     ######    ##  ########  ######   ########  #########  ######  ######
     ##        ##  ##    ##  ##       ##     ## ##     ##       ## ##
     ##       #### ##     ## ######## ########  ##     ##  ######  ########

You're about to initialize a Firebase project in this directory:

  D:\USER\Documents\Project\web_n4mmon

? Are you ready to proceed? Yes
? Which Firebase features do you want to set up for this directory? Press Space to select features, th
en Enter to confirm your choices. 
Realtime Database: Configure a security rules file for Realtime Data
base and (optionally) provision default instance, 
Firestore: Configure security rules and indexes file
s for Firestore, 
Functions: Configure a Cloud Functions directory and its files, 
Hosting: Configure files for Firebase Hosting and (optionally) set up GitHub Action deploys, 
Hosting: Set up GitHub Action
deploys
? Please select an option: Use an existing project
? Select a default Firebase project for this directory: nammon-ks (n4mmon)
? What file should be used for Firestore Rules? firestore.rules
? What file should be used for Firestore indexes? firestore.indexes.json
? What language would you like to use to write Cloud Functions? JavaScript
? Do you want to use ESLint to catch probable bugs and enforce style? No
? Do you want to install dependencies with npm now? Yes
? What do you want to use as your public directory? dist
? Configure as a single-page app (rewrite all urls to /index.html)? Yes
? Set up automatic builds and deploys with GitHub? Yes
+  Wrote dist/index.html

i  Didn't detect a .git folder. Assuming D:\USER\Documents\Project\web_n4mmon is the project root.
i  Authorizing with GitHub to upload your service account to a GitHub repository's secrets store.

Visit this URL on this device to log in:
https://github.com/login/****LOGIN URL****

Waiting for authentication...

+  Success! Logged into GitHub as GITHUB_USER

? For which GitHub repository would you like to set up a GitHub workflow? (format: user/repository) mo
npopza/n4mmon
[THIS REPOSITORY YOU MUST CREATE AT GITHUB PAGE]

+  Created service account github-action-486306792 with Firebase Hosting admin permissions.
+  Uploaded service account JSON to GitHub as secret FIREBASE_SERVICE_ACCOUNT_NAMMON_KS.
i  You can manage your secrets at https://github.com/**/settings/secrets.
? Set up the workflow to run a build script before every deploy? Yes
? What script should be run before every deploy? (npm ci && npm run build)
? What script should be run before every deploy? npm ci && npm run build

+  Created workflow file D:\***\.github/
workflows/firebase-hosting-pull-request.yml
? Set up automatic deployment to your site's live channel when a PR is merged? Yes
? What is the name of the GitHub branch associated with your site's live channel? main

+  Created workflow file D:\***\.github/workflows/firebase-hosting-merge.yml

i  Action required: Visit this URL to revoke authorization for the Firebase CLI GitHub OAuth App:
https://github.com/settings/connections/applications/********
i  Action required: Push any new workflow file(s) to your repo

=== Storage Setup

Firebase Storage Security Rules allow you to define how and when to allow
uploads and downloads. You can keep these rules in your project directory
and publish them with firebase deploy.

? What file should be used for Storage Rules? storage.rules
+  Wrote storage.rules

i  Writing configuration info to firebase.json...
i  Writing project information to .firebaserc...
i  Writing gitignore file to .gitignore...

+  Firebase initialization complete!
```
## Copy Edit File to Vue Folder
> Additional
```
( Copy Text ) .gitignore (Firebase) >> .gitignore (Project)
( Copy Files ) All File (Firebase, เว้น .gitignore) > Project
```
