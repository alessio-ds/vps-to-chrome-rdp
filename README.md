# colab-to-chrome-rdp

Install Chrome Remote Desktop on Google Collab 

This script was forked from alok676875 RDP repo (https://github.com/alok676875/RDP/) with more detail about user credentials and more useful information provided.

# How to use ?

Paste this to new collab notes and execute:
```
! wget https://raw.githubusercontent.com/AlessioScarlet/colab-to-chrome-rdp/main/code.sh &> /dev/null
! chmod +x code.sh
! ./code.sh
```
This will create a new username alessioscarlet with password:scarlet,then install xfce and chrome remote desktop server

You might want to change alessioscarlet's password using "passwd" (without quotes and sudo)

You can also change root user password using "sudo passwd" (without quotes)

And you now have a free VPS (lol)
## NOTE: alessioscarlet's password is: scarlet
# Prevent from disconnecting.
You can keep your session running by creating a new code block (Ctrl+ M B) and put: 
```
while True:pass
```
and execute on the same notes.
#### Or use javascript by opening developer console (Ctrl+Shift+I) and type this:
```
function ClickConnect(){
    console.log("Working"); 
    document.querySelector("colab-toolbar-button#connect").click() 
}
setInterval(ClickConnect,60000)
```
