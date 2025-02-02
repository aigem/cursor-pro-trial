# Cursor Device Identifier Generator  

A secure, simple, and fast tool for resetting the Cursor Pro Trial device identifier.  

## Features  

- 🔒 **Secure & Reliable** – Fully frontend-based, no backend service required  
- 🚀 **Fast & Convenient** – Generate a new device identifier with one click  
- 💻 **Cross-Platform Support** – Works on Windows, macOS, and Linux  

## Usage Instructions  

1. Log out of your Cursor account and ensure Cursor is completely closed (including background processes). Usually, closing Cursor is enough.  
2. Open the tool page and click the **"Regenerate ID"** button. The page is available [here](https://cursor-id.duu.men/) or check the description link.  
3. Locate and open the corresponding configuration file based on your operating system:  
   - **Windows (Win + R, then enter)**: `%APPDATA%\Cursor\User\globalStorage\storage.json`  
   - **macOS**: `~/Library/Application Support/Cursor/User/globalStorage/storage.json`  
   - **Linux**: `~/.config/Cursor/User/globalStorage/storage.json`  
4. Copy and replace the following three identifiers in the configuration file with the newly generated ones:  
   - `telemetry.macMachineId`  
   - `telemetry.machineId`  
   - `telemetry.devDeviceId`  
5. Save the file.  
6. Restart Cursor and log in.  
7. Ensure your Cursor Pro Trial account is working correctly.  

## Quick Access to Configuration File  

### Windows  
1. Press `Win + R` to open the Run dialog.  
2. Paste `%APPDATA%\Cursor\User\globalStorage\storage.json`.  
3. Click **OK**.  

### macOS  
1. In Finder, press `Command + Shift + G`.  
2. Paste `~/Library/Application Support/Cursor/User/globalStorage/storage.json`.  
3. Click **Go**.  

### Linux  
Open the file in a text editor using the terminal:  
```bash
nano ~/.config/Cursor/User/globalStorage/storage.json
# or
vim ~/.config/Cursor/User/globalStorage/storage.json
```  

## Important Notes  

- ⚠️ Make sure Cursor is completely closed before making changes.  
- 💾 It is recommended to back up the original configuration file before modifying it.  
- 🔄 If the changes do not take effect, check if Cursor is still running in the background.  

## Disclaimer  

This tool is for educational and research purposes only. Users assume full responsibility for any issues or risks arising from its use. Cursor is an excellent editor—if possible, consider purchasing it to support development.  