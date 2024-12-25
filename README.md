# Duplicate Firebase Initialization

This repository demonstrates a common error in Firebase applications: initializing the Firebase SDK multiple times with different configurations.  This leads to unexpected behavior and crashes.  The solution shows how to correctly initialize Firebase only once, even across multiple modules or components.

## Steps to Reproduce

1. Clone the repository
2. Run `npm install`
3. Run `node multipleFirebaseInit.js`

You'll see the error message from Firebase indicating duplicate initialization.

## Solution

The `multipleFirebaseInitSolution.js` file demonstrates the correct approach: using a single initialization point and checking for existing app instance before initializing.