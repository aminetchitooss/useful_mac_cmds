# Useful_mac_cmds


## For Installing 

Installing Sublime

      rm /usr/local/bin/subl
      ln -s "/Applications/Sublime Text.app/Contents/SharedSupport/bin/subl" /usr/local/bin/subl

### <ins> Adding the following commands into .bash_profile to avoid repeat running them</ins>

### For debuggin Cloud functions in VS

      alias functions="`npm config get prefix`/bin/functions-emulator"

### For Installing firebase tools

      alias firebase="`npm config get prefix`/bin/firebase"
      
## For Utilities

>To save the current direcrtory into a stack and move into a new directory

    pushd /...
    popd

>To search for <ins> **files**</ins> updated last 30 min

      find . -type f -mmin -30 
      
>To search for <ins> **directories**</ins>   with name start with "test"  case insensitive

      find . -type d -iname "test*" 
      

### check before deleting delete
      find . -type f -name "*mid*.png" -maxdepth 1
      
>To delete

      find . -type f -name "*mid*.png" -maxdepth 1 -exec rm {} +
      
>To change access mode **(permissions)**

      find . -type f -name "*mid*.png" -maxdepth 1 -exec chmod 775 {} +
