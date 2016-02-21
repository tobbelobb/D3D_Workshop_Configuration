# D3D_Workshop_Configuration
Configuration files for configuring various programs in the Porteus Live USB sticks used in D3D Workshops.

To make a xzm package of this repo from within Porteus, first ensure you've got git installed.
Then clone this repo (as the guest user)
 git clone git://github.com/tobbelobb/D3D_Workshop_Configuration.git
Then remove all files that are not directories
 find D3D_Workshop_Configuration -maxdepth 1 -type f -delete
Then remove git's files within the repo
 su
 rm -r D3D_Workshop_Configuration/.git
Create the xzm
 dir2xzm D3D_Workshop_Configuration D3D_Workshop_Configuration.xzm
 exit
Delete the directory
 rm -r D3D_Workshop_Configuration
 
When you feel comfortable with the procedure, put it in a script...
