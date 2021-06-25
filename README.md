Insta App project is social media app that can post your favorite images/photos and give comments on it. it was created with "Create-React-App" utility.

On the Insta App project directory, you can use these commands to run it:

# npm start
Runs the app in the development mode.

# npm test
Launches the test runner 

# npm run build
Builds the app for production to the build folder.
The build command eill minify and the filenames include the hashes.

# npm run eject
This command will delete the single build dependency from insta app project. Once you do eject, you win't be able to undo it.


# Here are the dependecies that you need to install before running insta app project

npm install @material-ui/core 
npm i @material-ui/icons 
npm i material-ui-popup-state
npm i react-scripts 
npm i firebase 
npm install -g firebase-tools 
npm i react-instagram-embed
npm i react-expanding-textarea 
npm i react-instagram-embed  
npm i react-lazyload 
npm i react-linkify 
npm install get-user-locale 

# To run insta app locally:
1. Add a firebase.js file in src directory
2. Import firebase from npm into firebase.js file that we have created
3. Create new firebase project 
4. Set up your firebase database project 

5. Add the following codes here:

import firebase from "firebase";

const firebaseApp = firebase.initializeApp({
  apiKey: "your api key",
  authDomain: "your auth domain",
  databaseURL: "your database URL",
  projectId: "your project ID",
  storageBucket: "your storage bucket",
  messagingSenderId: "your messaging SenderId",
  appId: "your app Id",
  measurementId: "your measurement ID",
});

const db = firebaseApp.firestore();
const auth = firebase.auth();
const storage = firebase.storage();

export { db, auth, storage };

6. run npm start on your terminal/CMD