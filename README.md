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



## Step 6: Run Project Build :

#### 6.1 )  Build the project scripts using this command:

```bash
          npm run build 
```



## Step 7: Initialize Firebase :

#### 7.1 )  Initialize Firebase using this command

```bash
          firebase init
```

#### 7.2 )  "Are you ready to proceed?" :
   
-  Type **` Y `** for " yes ".

#### 7.3 )  "Which Firebase features do you want to set up for this directory?"

   - Use the arrow down key on your keyboard to point to the option
   
   - #### "Hosting:Configure files for Firebase Hosting and (optionally) set up GitHub Action deploys".

   - Press the space bar and then hit enter.



## Step 8: Project Setup :

This step connects your project directory with the Firebase project.

#### 8.1 )  "select a default Firebase project for the directory"

   - select the particular Firebase project you created.



## Step 9: Setup Hosting :

This process will bring up some prompts you'll have to answer.

#### 9.1 )  "What do you want to use as your public directory?"

   - Type **` build `**.

#### 9.2 )  "Configure as a single-page app (rewrite all urls to /index.html)"

   - Type **` Y `** or **` Yes `**.

#### 9.3 )  "Set up automatic builds and deploys with GitHub?"

   - Choose **` Yes `** option.

#### 9.4 )  "File build/index.html already exists. Overwrite?"

   - Choose **` No `** option.



## Step 10: Authorize Firebse with Github :

####  You need to authorize Firebase with your GitHub account.
    
A window will open up on your browser that will require you to authorize Firebase into your GitHub,
     
   - **` input your GitHub password `**
     
After a successful authentication, you'll get a success message on your terminal with your GitHub username.



## Step 11: How to Choose a GitHub Repository and Set Up GitHub Workflow :

#### 11.1 )  Select Github Repo :

Type the GitHub repository you'd like to use to set up a GitHub workflow for Firebase deployments.

   - Format **` " github_username/repository " `** .

#### 11.2 )  Github Secret token :

After setting up a GitHub workflow, it will create a secret token.

You can also view this secret token on GitHub. 

To do this, go to the repository of the project and switch to the "Settings" tab. On the left-hand panel of the settings page, click on the "Secrets and variables" dropdown and select the "Actions" option.

#### 11.3 )  Set up Workflow :

#### 11.3.1 )  "Set up the workflow to run a build script before every deploy?"

   - Choose **` Yes `** option.

#### 11.3.2 )  "What script should be run before every deploy? (npm ci && npm run build) npm run build"

- Type this **` npm ci && npm run build `** into the terminal.

#### 11.4 )  Automatic deployment :

#### 11.4.1 )  "Set up automatic deployment to your site's live channel when a PR is merged"

 - Select **` Yes `** .

#### 11.4.2 )  "the name of the GitHub branch associated with your site's live channel ?"

 - Type or select **` main `** .



## Step 12:  Generate Folders :

The two operations performed above will generate two folders in your project directory.
     
One named "firebase.json" is where the configuration information will be written in, 
     
and the other named ".firebaserc" is where the project information will be written in.

   

# How to Deploy to Firebase :

## Run the Deployment Command 

```bash 
    firebase deploy 
```

 After running firebase deploy, your React app should be live on Firebase Hosting. You will get a URL in the terminal where your app is deployed.


## New Modifications / Updation of the App  

   Once new changes are made in the application then run the following commands ,

```bash
    npm run build
```

   and 

```bash 
    firebase deploy
```

