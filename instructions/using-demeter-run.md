
# Instructions for setting up your development environment with Demeter.Run  

**ATTENTION:** The Demeter.Run platform is frequently updated and instructions provided in this file may not be up to date at any given time. 

The following instructions guide you through setting up a Plutus development environment in Demeter.Run: 
* Open your browser, navigate to https://demeter.run/ and click the Login option on the top navigation menu. Login with your Google or GitHub account. You can also sign up for a new account. 
+ Under the Projects section you can click on **New project**. Then type in project Name, an optional description and select an organization, which will basically be the account your logged in with. 
* After you clicked **Create project** you will see the project's admin page. You will need to add some DCUs (Demeter computing unints) to you project. You can specify a payment method and buy DCUs. 
* Once you have DCUs you can start up your project. You can click on the **Open console** button. Under Workloads you can click **Create new** and select if you want a workspace, frontend, backend or backend with storage. 
* If you select a frontend or backend you will need to enter a name of a Docker image that is publicly available. You can then add some arguments, environment variables and configuration. At the end you have to select a container size and the network you want to connect to. 
* If you select workspace you will be asked if you are cloning and existing repository and if yes you can provide the URL of the repository and the branch you want to wrok on. Next you can select your toolchain which means which libraries and languages you want to be added to your environment. Then you can also select some extras as Nix and Cardano binaries. You will also have to select your workspace size and network you want to connect to and in the end set a workspace name. 
* Once you click create your workspace will be created. After that you will be redirected to the project main page and the workspace information will be displayed. The workspace also needs some time before it builds. After its build, it will automatically go into run mode. You can click the **Pause workspace** button on the right side to pause it and then click again on the same button that will have the tool tip *Run workspace* to run it again. 
* Under the **Extensions** section in the top menu you can add some extenstions to your project like a cardano or hydra node. Under the **Starter kits** section in the top menu you can add some example code repositories to your project that you can use for learning or as a starting point. 
* Once everything is set up you can click the VSCode logo and a VSCode editor will appear that will contain all the files from the repository if you specified ont in the workspace creation step. 

**IMPORTANT:** Demeter.run will charge you DCUs for a running workspace. So after you finish with your work, always pause your workspace. 