# powershell_tricks

--Fix for PowerShell Script Not Digitally Signed
Example: (“.ps1 is not digitally signed. The script will not execute on the system.")

To fix it you have to run the command below to run Set-ExecutionPolicy and change the Execution Policy setting.
Fix: Set-ExecutionPolicy -Scope Process -ExecutionPolicy Bypass

This command sets the execution policy to bypass for only the current PowerShell session after the window is closed, the next PowerShell session will open running with the default execution policy. “Bypass” means nothing is blocked and no warnings, prompts, or messages will be displayed.
