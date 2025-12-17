# Transform-Boring-Terminal-into-Interesting-Terminal-
![Screenshot](Screenshot%202025-12-17%20093205.png)

# Terminal Setup Guide

This guide will walk you through installing a Nerd Font, changing your terminal theme and font, and setting up your PowerShell profile.

---

## 1. Install JetBrains Mono Nerd Font

Download and install the **[JetBrains Mono Nerd Font](https://www.nerdfonts.com/font-downloads)** on your system or download from Repo.

---

## 2. Change Theme and Font via `settings.json`

1. Open your terminal folder and navigate to `settings.json`.  
2. Open your terminal, click the dropdown arrow, select **Settings**, and choose **Open JSON file**.  
3. Scroll to the bottom, select all contents, and delete everything.  
4. Paste in your copied configuration from `settings.json`.  
5. Save the file using `Ctrl + S`.

---

## 3. Locate or Create the PowerShell Profile

1. Check the location of your PowerShell profile by running:

    ```powershell
    $profile
    ```

2. Press **Enter** to see the path where your profile is located.  
3. If the folder is empty (no profile exists), create one by running:

    ```powershell
    New-Item -Path $profile.CurrentUserAllHosts -Type File -Force
    ```

4. Navigate to that location in **File Explorer**.  
   You should see a `Microsoft.PowerShell` folder, and inside it, the `profile.ps1` file.

---


## 4. Install Fastfetch

1. Copy the Winget installation command:

    ```powershell
    winget install fastfetch
    ```

2. Paste the command into your terminal and press **Enter** to install Fastfetch.

---

## 5. Configure Fastfetch Files

1. Download both the **config file** and the **ASCII art file**.  
2. In **File Explorer**, navigate to:

    ```
    This PC → C: drive → Users → your-username
    ```

3. Create a new folder called `.config`.  
4. Make the folder hidden:  
   - Right-click `.config` → **Show more options** → **Properties**  
   - Check the **Hidden** box and click **Apply** → **OK**  
   - *(If you cannot see it, ensure "View" → "Show hidden files" is enabled.)*

5. Inside the `.config` folder, create a folder named `fastfetch`.  
6. Move the downloaded **config file** and **ASCII art file** into the `fastfetch` folder.  
7. Open the **config file** and replace `%username` with your actual username.  
8. Save the config file.

---

## 6. Edit the PowerShell Profile Script

1. Navigate back to your PowerShell profile folder where `profile.ps1` is located.  
2. Open the `profile.ps1` file.  
3. Paste the code you copied from `Microsoft.PowerShell_profile.ps1` into `profile.ps1`.  
4. Replace `%username` within this script with your actual username.  
5. Save and close the file.

🎉 You are now ready to customize your PowerShell terminal with your preferred theme and font!
