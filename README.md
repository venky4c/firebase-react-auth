# firebase-react-auth
Basic email password authentication using Firebase and React
Live Project: https://serene-haibt-9b3f4d.netlify.app/login

This email password authenitcation uses [React Context](https://github.com/venky4c/firebase-react-auth/blob/master/dist/src/Auth.js) to store the current user and decide if the user is logged in or not with the help of Firebase API.

The creation of initialization of Firebase app instance is tucked in this code snippet here(https://github.com/venky4c/firebase-react-auth/blob/master/dist/src/base.js)
```javascript
const app = firebase.initializeApp({
  apiKey: process.env.REACT_APP_FIREBASE_KEY,
  authDomain: process.env.REACT_APP_FIREBASE_DOMAIN,
  databaseURL: process.env.REACT_APP_FIREBASE_DATABASE,
  projectId: process.env.REACT_APP_FIREBASE_PROJECT_ID,
  storageBucket: process.env.REACT_APP_FIREBASE_STORAGE_BUCKET,
  messagingSenderId: process.env.REACT_APP_FIREBASE_SENDER_ID
});
```
