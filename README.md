# GhostDelivery
![GD](https://user-images.githubusercontent.com/51238001/59381305-9b0e1b00-8d4a-11e9-8e34-c72bf29f1ff1.PNG)
Python script to generate obfuscated .vbs script that delivers payload (payload dropper) with persistence and windows antivirus disabling functions.
# Heavy:

- Downloads payload to TEMP directory and executes payload to bypass windows smart screen
- Disables Defender
- Disables UAC/user account control
- Disables Defender Notifications
- Injects/creates Command Prompt and Microsoft Edge shortcuts with payload path (%TEMP%/payload.exe) to execute payload when opened
- Creates a scheduled task called "WindowsDefender" for payload to be run at login and obfuscates the vbs delivery script
- Includes a serveo function to deliver obfuscated vbs script
# Medium:

- Delivers/executes payload
- Creates a scheduled task named "WindowsDefender" to run payload at login for persistence
- Disables UAC and injects/creates Command Prompt and Microsoft Edge shortcuts with payload path
- Includes a serveo function to deliver obfuscated vbs script
# Light:

- Delivers/executes payload
- Creates a scheduled task named "WindowsDefender" to run payload at login for persistence
- Injects/creates Command Prompt and Microsoft Edge shortcuts with payload path
- Includes a serveo function to deliver obfuscated vbs script
# Prerequisites/requirements:

*Python 2.7 + Modules imported in script.
- random
- sys
- string
- os
- time
- base64
