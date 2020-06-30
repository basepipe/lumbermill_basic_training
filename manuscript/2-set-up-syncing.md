# Set Up Syncing

Lumbermill has a syncing system designed for film production.  It allows companies to easily share
complex and large files with each other.  Since Lumbermill knows what's happening with all your files it can be smart
about which files and versions to sync, saving you a lot of time consuming syncing of versions you don't need.

Here's the Basic Steps.

1) [Set up AWS Credentials](#Set-up-AWS-Credentials)
2) [Set up Lumbermill Server](#Set-up-Lumbermill-Server)
3) [Set up Remote Workstation](#Set-up-a-Remote-Workstation)

## Set up AWS Credentials {#Set-up-AWS-Credentials}

### Ensure AWS CLI is installed

1) Open a CMD Window
2) type 'aws' and hit enter
    

If you got this message - move on to [Configure AWS Settings](#Configure-AWS-Settings)

```
    usage: aws [options] <command> <subcommand> [<subcommand> ...] [parameters]
    To see help text, you can run:

      aws help
      aws <command> help
      aws <command> <subcommand> help
    ws: error: the following arguments are required: command
```
    
If you don't get this message you'll need to install aws cli 

### Configure AWS Settings {#Configure-AWS-Settings}

Before starting this step you will need the following information:
* AWS Access Key
* AWS Secret Key
* AWS Region

Once you have that you can move on.

1) Open a cmd window
2) type 'aws configure'
3) if you see something like this:

```
AWS Access Key ID [****************IPHG]:
```
    
you have already set up aws, move on to [Setting up your Server](#Set-up-Lumbermill-Server)
    
Otherwise the following shows sample values. Replace them with your own values:

```
    $ aws configure
    AWS Access Key ID [None]: AKIAIOSFODNN7EXAMPLE
    AWS Secret Access Key [None]: wJalrXUtnFEMI/K7MDENG/bPxRfiCYEXAMPLEKEY
    Default region name [None]: us-east-1
    Default output format [None]: json
```


## Set up Lumbermill Server {#Set-up-Lumbermill-Server}

Most productions have a central "hub" where all data is stored.  This can be a network storage server at a studio, or simply the hard drive on your computer with a small team.  The computer tied to the storage is where you'll set up the lumbermill server for the project. Tasks will be "pushed" from here, and all files will be gathered back to here. 

Assuming you have already [Set up AWS Credentials](#Set-up-AWS-Credentials) - To set up a lumbermill server for your studio:

1) Open Lumbermill
1) Ensure Auto-Start is set to On. 
    1) if Sync>Auto-Start: Off toggle it to On.
    1) Restart Lumbermill
1) Click Sync>Set up Server
1) This will go though a bunch of various things.

You are now set up to start [sharing files](#Sharing-Files) with [remote collaborators](#Set-up-a-Remote-Workstation). 


## Set up a Remote Workstation {#Set-up-a-Remote-Workstation}

To set up a remote collaborator for syncing with lumbermill do the following:

1) Open Lumbermill
1) Ensure Auto-Start is set to On. 
    1) if Sync>Auto-Start: Off toggle it to On.
    1) Restart Lumbermill
2) Click Sync> Set up Workstation
1) You Should See the following printout in the Lumberwatch CMD window.  When you see this you know your machine registration has been sent to lumbermill.  In a minute or two you will start seeing the remote machines show up in the syncthing web browser.


## Sharing Files {#Sharing-Files}

With a [Server](#Set-up-Lumbermill-Server) and a [Remote Workstation](#Set-up-a-Remote-Workstation) set up you are now ready to share files.  To Share files log in to your server machine and:

1) Open Lumbermill
2) Click Sync>Share Files
3) Select assets or shots
4) Select anything you'd like to share.
5) Click the "Sync" button
