# uBlock_Origin_Chrome
Block your adware in Chrome with uBlock Origin\
This is only for self documentation !

# Download uBlock Extension
Download latest version from [uBlock](https://github.com/gorhill/uBlock/releases)
- Assets (/.chromium.zip)
- Unpack the .zip to whatever directory you wanna save it

# Setting Chrome Flags
Locate towards the `Chrome Flags`
- Go to Flags Tab --> chrome://flags/ 
- Set the Flags like in the Screenshot below
  
<img width="733" height="340" alt="image" src="https://github.com/user-attachments/assets/45cc1610-738c-48ee-b9fe-7d68a310b9ab" />

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

# Credits

[@pixeltris](https://github.com/pixeltris) for JavaScript\
[@gorhill](https://github.com/gorhill) for uBlock Chrome Extension\
[@frequencycs/fpsheaven](https://github.com/fpsheaven) for Chrome and registry settings\  
