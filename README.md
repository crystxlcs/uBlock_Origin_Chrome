# uBlock_Origin_Chrome
Block your adware in Chrome with uBlock Origin 

# Download uBlock Extension
Download latest version from [uBlock](https://github.com/gorhill/uBlock/releases)
- Assets (/.chromium.zip)
- Unpack the .zip to whatever directory you wanna save it

# Setting Chrome Flags
Locate towards the `Chrome Flags`
- Go to Flags Tab --> chrome://flags/ 
- Set the Flags like in the Screenshot below
  
<img width="733" height="652" alt="Screenshot 2025-07-17 233845" src="https://github.com/user-attachments/assets/890fefcc-3de7-4969-b2d1-53d422033d92" />

If you dont have the `Manifest V2` Flags, do this step first
- Enter powershell via admin
- Type in ($path = registry::HKEY_LOCAL_MACHINE\SOFTWARE\Policies\Google\Chrome"; New-Item $path -Force; Set-ItemProperty $path -Name ExtensionManifestV2Availability -Value 2) and press enter
- Quit powershell
- Go back to the flags tab 
- Set the Flags like in the Screenshot shown above
- Restart Browser

# Load Extension
- Go to Extensions Tab --> chrome://extensions/
- Enable Developer mode
- Load upacked and select the unpacked folder
- uBlock should be shown in your extensions tab
  
# Applying Twitch AdBlock script
- Navigate to the uBlock Origin Dashboard (the extension options)
- Under the `My filters` tab add `twitch.tv##+js(twitch-videoad)`.
- Under the `Settings` tab, enable `I am an advanced user`, then click the cog that appears. Modify the value of userResourcesLocation from unset to the full url of the solution you wish to use (if a url is already in use, add a space after the existing url). e.g. `userResourcesLocation` `https://raw.githubusercontent.com/crystxlcs/uBlock_Origin_Chrome/refs/heads/main/adblock-twitch.js`
- To ensure uBlock Origin loads the script I recommend that you restart your Browser.\
\
To stop using a script remove the filter and make the url `unset`.
