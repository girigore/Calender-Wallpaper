# Calender-Wallpaper
Program to change a windows background based on a calender schedule.  
Base of the Wallpaper Class : https://stackoverflow.com/questions/1061678/change-desktop-wallpaper-using-code-in-net
  
  
NOTES:
- Works for windows 10, unsure as to earlier versions of windows.
  
  
DOWNLOAD:
- .exe download: https://www.dropbox.com/s/i8lgj6f4x0d99r6/Wallpaper%20Calender%20Caller.exe?dl=0
  
  
HOW TO USE:
1. Run the .exe normal without any command line parameters. Use the form to create your schedule for your wallpapers.  
    * Folders will pick a random (skipping the previously chosen one the next day) image from the folder each day.
2. Once scheduled save (this will create an .xml).
3. Using Windows Task Scheduler. (I would love to automate this with the GUI, but I have not.)
    * Create Task.  
    * Provide a Name.  
    * Triggers: Daily: At whatever time you want. On logon/At startup.  
    * Actions:  
      + Start a program: browse -> choose the exe. 
      + Add Arguments: -caller "C:\path\to\save.xml"
  
4. Done!
