# Configuring the Power Supply to Optimize Performance

### Choosing An Energy-Saving Plan

- For AMD and Intel processors of 12-14 generations: It is recommended to use the "Balanced" plan. For Ryzen users, don't forget to set the slider to the "Best Performance" position through the Windows Power Settings panel. For older Intel processors (11th generation and below): Enable the Ultimate Performance plan to maximize productivity.

### Open the command prompt as an administrator:

- Press Win + X and select "Command Prompt (Administrator)" or "Windows PowerShell (Administrator)".
- Enter the command to activate the plan: powercfg -duplicatescheme e9a42b02-d5df-448d-aa00-03f14749eb61

### Configuring USB Settings to Save Energy

- Set the value to "Forbidden" to prevent temporary disconnection of USB ports, which can be useful for connected gaming devices and peripherals that require constant
