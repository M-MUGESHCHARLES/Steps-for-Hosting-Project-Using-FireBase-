# Firebase-Deploy

If you don't have an account on Firebase, go to this site to create an account on [**Firebase**](https://firebase.google.com/) or log in ;
After you've successfully logged in, you'll need to create a project on Firebase.

## Step 1: Firebase Console Dashboard :

   1.1)  Go to your Firebase console dashboard, where you should see the text **`Go to console`** at the top right-hand side of your page after logging in.

   1.2)  The page that opens up will have a **`Create a project`** button. Click on that button and it will take you to the page where you'll input your project details. (Step 2)

   1.3)  If you've previously used Firebase, that means you already have projects on Firebase. In that case, it will bring up a page displaying a list of your projects and a box to **`add a new project`**.

## Step 2: Create a New Project :

   2.1)  Click the **`Add project`** card ; name the project **" Project_Name "**.
   
   2.2)  Accept the **`Accept Firebase terms`** checkbox and the second checkbox.
   
   2.3)  Click the **`continue`** button. 

   2.4)  **`Disable the toggle`** as we don't need Google Analytics. 

   2.5)  Click the **`Create Project`** button and it should start creating your Firebase project.

## Step 3: Install Firebase and Firebase Tools :

   The next step is to go to your project terminal on your code editor you're using, 
   Ensure you're in the main folder of the project you want to deploy. 

   3.1)  install Firebase into the project using this command:
   
```bash
          npm install firebase
```

   3.2)  Next, install the Firebase tools using this command:

```bash
          npm install -g firebase-tools
```

## Step 4: Log in to Firebase Using the Terminal :

   4.1)  Log in to Firebase on the terminal using this command: 

```bash
          firebase login
```

   4.2)  "Allow Firebase to collect CLI and Emulator Suite usage and error reporting information" :

- Select the **`Yes`** option.

## Step 5: Select Account :

   A window will open up on the default browser that will require you to select your Firebase account for login.

   After successful authentication, a success message will appear on the terminal.

## Step 6: Run Project Build :

   6.1)  Build the project scripts using this command:

```bash
          npm run build 
```
## Step 7: Initialize Firebase :

   7.1)  Initialize Firebase using this command:

```bash
          firebase init
```

   7.2)  "Are you ready to proceed?" :
        - Type **`Y`** for " yes ".

  7.3)   "Which Firebase features do you want to set up for this directory?" :

   Use the arrow down key on your keyboard to point to the option
   
   "Hosting:Configure files for Firebase Hosting and (optionally) set up GitHub Action deploys" .
   
       - Press the space bar and then hit enter.


