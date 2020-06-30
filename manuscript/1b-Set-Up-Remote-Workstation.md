# Setup Lumbermill on a Remote Workstation {#setup-remote-workstation}
 
## Windows install

1) [Download](https://cgl-developeronboarding.s3.amazonaws.com/lumbermill_installer.zip) the lumbermill installer. 
1) Unzip the folder

Your Folder should look something like this:

![Extracted Zip Folder](lmill_install_folder.jpg)

### Video
![Set Up Lumbermill for an Existing Company](https://www.youtube.com/watch?v=BE8X5HWJiuA)


### Details
**Company Name:** You'll need this in step 4 - you should have been told what "company name" to use by your producer.  

1) double-click "step_1_install_chocolatey.bat"
2) double-click "step_2_python_env_setup.bat"
3) double-click "step_3_setup_cglumberjack.bat"
4) double-click "step_4_configure_lumbermill.bat"
  - You'll need your company name at this stage.
  - ![Config Dialog](build_config.png)
5) double-click "step_5_launch_lumbermill.bat"
  - Fill in the Login Dialog - this connects the user of your machine to your project management software
  - ![Project Management Login](proj-man-login.png)
    * Login Email - the email used when connecting to Ftrack
    * email - your email (if different) - often this is just the same email.
    * First Name
    * Last Name
6) copy "lumbermil.bat" to your desktop for general use.
7) [configure aws](#configure-aws)




 


