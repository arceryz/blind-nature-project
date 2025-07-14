# Blind Nature Project Management
The project management repository for Liora's Blind Nature. This is the place where useful links, resources and documents can be uploaded. The actual project is managed in *Perforce: Helix Core*, which is a specialized version control system for games. Please read this document set up the Helix Core on your system and start contributing. If you do not have permission for a certain resource, contact me.

Tools we use:
- Perforce to store the project and for version control.
- Canva for whiteboarding, worldbuilding, art inspiration, idea sharing. [Go here](https://www.canva.com/design/DAGrTBQaV34/1gaO3hmYpI18O-d-SNbPig/edit?utm_content=DAGrTBQaV34&utm_campaign=designshare&utm_medium=link2&utm_source=sharebutton).
- GitHub projects for managing the tasks. [Go here](https://github.com/users/arceryz/projects/4)
- Discord for communication. 

Inspired by:
- [The Vale](https://store.steampowered.com/app/989790/The_Vale_Shadow_of_the_Crown/)

Table of contents:
- Perforce
	- [Setting up Perforce](#setting-up-perforce)
	- [Integrating Perforce and Wwise](#integrating-perforce-and-wwise)
 - Task Management
	- [Using GitHub projects and issues](#using-github-projects-and-issues)
# Setting up Perforce
1. Start by downloading P4V, the Perforce 4 Visual client. [Link here](https://portal.perforce.com/s/downloads?product=Helix%20Visual%20Client%20%28P4V%29). It is faster on Windows if you open the Command Prompt application and type `winget install Perforce.P4V`.

2. Open up the P4V application. You will be prompted to log in on a Perforce server. Enter the fields:
   - Server = `ssl:p4.liorainteractief.nl:1666`
   - User = Click "Browse" to find your user in the list. Ask me to create a new user for you.

3. You will be prompted for the password, which you can later change as well. By default, a session lasts 12 hours after which you must enter the password again.

You have now set up the basic Perforce client. Before you can start downloading the project and make changes, we must create a workspace for you. A workspace in Perforce is a local folder on a specific computer where you will do your work. For every device that you work on, you need a different workspace. In the workspace folder, you will be downloading parts of the project you want to work on through Perforce.

4. Open up P4V, then go to "Workspace". Click on the line below where it says "no workspace" and then click "New Workspace". Set the name of the workspace to the form "username_devicename" like admin_RyzenLaptop. Select the `mainline` stream to work on and find a suitable project folder on your PC.


![](/res/workspace.png)

5. You can now "Get latest revision" for any files in the Depot (the server).

6. To start working on a certain file **it is critical that you "Check Out" the file** (right mouse click). This will lock the file for you and prevent anyone else from working on it as well. Everyone can see which files are being worked on.

7. To submit you changes simply click "Mark for Add", which will add the changes to the *Changelist* (a group of changes). A changelist can be submitted by pressing the button. Add an informative message to indicate what you have changed.

# Integrating Perforce and Wwise

1. In Wwise go to the Project Settings and select Perforce as the source control method.
2. Press config, then fill out the details of the Perforce server:
	- Server = `ssl:p4.liorainteractief.nl`
	- Port = `1666`
	- User = Your username
	- Workspace = Your workspace name (see in P4V)
  
3. Perforce is now integrated. You can now add Wwise things with "Mark for Add" in Wwise itself. The integration has many features, please read them yourself. Going to the "File Manager" in Wwise shows a list of all files and if they have been changed. This is a nice UI for submitting your changes.

# Using GitHub projects and issues

We use GitHub projects for managing the project and organizing tasks. It starts with an *issue* that you can create on a repository. See the "Issues" tab at the top. You can create an issue to track a new task or bug or anything. Make sure to
1. Set the correct labels for your task (Audio, Art, Programming etc)
2. Set the correct milestone for your task (if applicable)
3. Set the correct project for your task (my Liora's Blind Nature project)

The project is where we have a Kanban board to track the issues, a timeline and so on. You must be set as collaborator on the project page as well. Don't worry if you forget to set anything on your task, we can always do so later. As long as we can see what everyone is working on.
