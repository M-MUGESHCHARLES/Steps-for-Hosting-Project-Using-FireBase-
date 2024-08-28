# Host and Deploy a React App with Firebase

If you don't have an account on Firebase, go to this site to create an account on [**Firebase**](https://firebase.google.com/) or log in ;
After you've successfully logged in, you'll need to create a project on Firebase.

## Step 1: Firebase Console Dashboard :

#### 1.1 )  Go to your Firebase console dashboard, where you should see the text **` Go to console `** at the top right-hand side of your page after logging in.

#### 1.2 )  The page that opens up will have a **` Create a project `** button. Click on that button and it will take you to the page where you'll input your project details. (Step 2)

#### 1.3 )  If you've previously used Firebase, that means you already have projects on Firebase. In that case, it will bring up a page displaying a list of your projects and a box to **` add a new project `**.



## Step 2: Create a New Project :

#### 2.1 )  Click the **` Add project `** card ; name the project **" Project_Name "**.
   
#### 2.2 )  Accept the **` Accept Firebase terms `** checkbox and the second checkbox.
   
#### 2.3 )  Click the **` continue `** button. 

#### 2.4 )  **` Disable the toggle `** as we don't need Google Analytics. 

#### 2.5 )  Click the **` Create Project `** button and it should start creating your Firebase project.



## Step 3: Install Firebase and Firebase Tools :

   The next step is to go to your project terminal on your code editor you're using, 
   Ensure you're in the main folder of the project you want to deploy. 

#### 3.1 )  Install Firebase into the project using this command:
   
```bash
          npm install firebase
```

#### 3.2 )  Next, install the Firebase tools using this command:

```bash
          npm install -g firebase-tools
```



## Step 4: Log in to Firebase Using the Terminal :

#### 4.1 )  Log in to Firebase on the terminal using this command: 

```bash
          firebase login
```


#### 4.2 )  "Allow Firebase to collect CLI and Emulator Suite usage and error reporting information" :
   
-  Select the **` Yes `** option.



## Step 5: Select Account :

   A window will open up on the default browser that will require you to select your Firebase account for login.

   After successful authentication, a success message will appear on the terminal.



## Step 6: Initialize Firebase :

#### 6.1 )  Initialize Firebase using this command

```bash
          firebase init
```

#### 6.2 )  "Are you ready to proceed?" :
   
-  Type **` Y `** for " yes ".

#### 6.3 )  "Which Firebase features do you want to set up for this directory?"

   - Use the arrow down key on your keyboard to point to the option

   - Select the option :    
   - #### "Hosting:Configure files for Firebase Hosting and (optionally) set up GitHub Action deploys".

   - Press the space bar and then hit enter.



## Step 7: Project Setup :

This step connects your project directory with the Firebase project.

#### 7.1 )  "select a default Firebase project for the directory"

   - select the particular Firebase project you created.



## Step 8: Setup Hosting :

This process will bring up some prompts you'll have to answer.

#### 8.1 )  "What do you want to use as your public directory?"

   - Type **` build `**.

#### 8.2 )  "Configure as a single-page app (rewrite all urls to /index.html)"

   - Type **` Y `** or **` Yes `**.

#### 8.3 )  "Set up automatic builds and deploys with GitHub?"

   - Choose **` No `** option.



## Step 9: Run Project Build :

#### 9.1 )  Build the project scripts using this command

```bash
          npm run build 
```

## Step 10: Deploy to Firebase :

#### 10.1 )  Run the Deployment Command 

```bash 
    firebase deploy 
```

 After running firebase deploy, your React app should be live on Firebase Hosting. You will get a URL in the terminal where your app is deployed.


# Updations :

### New Modifications / Updation of the App  

   Once new changes are made in the application then run the following commands ,

```bash
    npm run build
```

   and 

```bash 
    firebase deploy
```

