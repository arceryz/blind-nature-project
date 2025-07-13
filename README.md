# Blind Nature Project Management
The project management repository for Liora's Blind Nature. This is the place where useful links, resources and documents can be uploaded. The actual project is managed in *Perforce: Helix Core*, which is a specialized version control system for games. Please read this document set up the Helix Core on your system and start contributing.

Tools we use:
- Perforce to store the project and for version control.
- Canva for whiteboarding, worldbuilding, art inspiration, idea sharing. [Go here](https://www.canva.com/design/DAGrTBQaV34/1gaO3hmYpI18O-d-SNbPig/edit?utm_content=DAGrTBQaV34&utm_campaign=designshare&utm_medium=link2&utm_source=sharebutton)
- GitHub projects for managing the tasks. [Go here](https://github.com/users/arceryz/projects/4)

# Setting up Perforce
1. Start by downloading P4V, the Perforce 4 Visual client. [Link here](https://portal.perforce.com/s/downloads?product=Helix%20Visual%20Client%20%28P4V%29). It is faster on Windows if you open the Command Prompt application and type `winget install Perforce.P4V`.

2. Open up the P4V application. You will be prompted to log in on a Perforce server. For the "Server" field, enter `ssl:p4.liorainteractief.nl:1666`, which indicates that we want to connect securely with `ssl` to the server at `p4.liorainteractief.nl` at port `1666`. For the "User" field, click "Browse" to find your user in the list. You can ask me to create a new user for you.

3. You will be prompted for the password, which you can later change as well. By default, a session lasts 12 hours after which you must enter the password again.

You have now set up the basic Perforce client. Before you can start downloading the project and make changes, we must create a workspace for you. A workspace in Perforce is a local folder on a specific computer where you will do your work. For every device that you work on, you need a different workspace. In the workspace folder, you will be downloading parts of the project you want to work on through Perforce.

To create a workspace in Perforce, go to "Workspace". Click on the line below where it says "no workspace" and then click "New Workspace". Set the name of the workspace to something of the form username_pcname like admin_RyzenLaptop. Select the `mainline` stream to work on and find a suitable project folder on your PC.

![](/img/workspace.png)
