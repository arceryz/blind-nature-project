# Blind Nature Project Management
The project management repository for Liora's Blind Nature. This is the place where useful links, resources and documents can be uploaded. The actual project is managed in *Perforce: Helix Core*, which is a specialized version control system for games. Please read this document set up the Helix Core on your system and start contributing.

Our tech stack:
- Perforce to store the project and for version control. See [Setting up Perforce](#setting-up-perforce).

## Setting up Perforce
This paragraph will explain how to set up version control with Perforce in general. There is an extra section for integrating Perforce with Wwise for audio designers.

1. Start by downloading P4V, the Perforce 4 Visual client. [Link here](https://portal.perforce.com/s/downloads?product=Helix%20Visual%20Client%20%28P4V%29). It is faster on Windows if you open the Command Prompt application and type `winget install Perforce.P4V`.

2. Open up the P4V application. You will be prompted to log in on a Perforce server. For the "Server" field, enter `ssl:p4.liorainteractief.nl:1666`, which indicates that we want to connect securely with `ssl` to the server at `p4.liorainteractief.nl` at port `1666`. For the "User" field, click "Browse" to find your user in the list. You can ask me to create a new user for you.

3. You will be prompted for the password, which you can later change as well. By default, a session lasts 12 hours after which you must enter the password again.
