# Transform-Boring-Terminal-into-Interesting-Terminal-
![Screenshot](Screenshot%202025-12-17%20093205.png)

Steps:
1) Install JetBrains Mono Nerd Font:
2) Change Theme and Font via settings.json:
      
      1. Open the terminal folder, then navigate to settings.json.
      2. Open your terminal, click the dropdown arrow, and select Settings, then choose Open JSON file.
      3. Scroll all the way down, select everything in the file, and delete it.
      4. Paste in the code you copied earlier from setting.json and save the file using Ctrl S.

3) Locate or Create the PowerShell Profile
   1.Check the location of your PowerShell profile by using the command: $profile.
   2.Press Enter; this will show you the path where your profile is located.
   3.If the folder is empty (meaning no profile exists), paste the code "New-Item -Path $profile.CurrentUserAllHosts -Type File -Force" into your terminal and press Enter to create the profile.
   4. Navigate to that location in File Explorer; you should see a Microsoft PowerShell folder, and inside that, the profile.ps1 file.

4) Install Fastfetch
   1. copy the wingit script : winget install fastfetch
   2.  Paste the script into your terminal and hit Enter to install fastfetch

5) Configure Fastfetch Files
   1. Download both the config file and the ASI art file.
   2. In File Explorer, navigate to This PC → C drive → Users → your username.
   3.  Create a new folder called .config.
   4.   Make the folder hidden: Right-click the .config folder, select "show more options," "properties," check the Hidden box, and click "apply + okay" (if you cannot see it, ensure "View" → "Show hidden files" is enabled).
   5.   Inside the .config folder, create a folder named fastfetch
   6.   Take the two downloaded files (config and ASI art) and cut and paste them into the newly created fastfetch folder
   7.    Open the config file and change %username to your actual username
   8. Save the config file

6) Edit the PowerShell Profile Script
   1.Go back to your PowerShell profile folder where the profile.ps1 file is located
   2. Open the profile.ps1 file
   3. Paste the code you just copied from Microsoft.PowerShell_profile.ps1 into profile.ps1
   4.  Replace %username within this script with your actual username
   5.   Save and close the file

      Enjoy>>>>>>>>
