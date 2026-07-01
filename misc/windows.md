# Activation

https://github.com/massgravel/Microsoft-Activation-Scripts

# Disable web search in start menu

```
New-Item -Path "HKCU:\SOFTWARE\Policies\Microsoft\Windows\Explorer" -Force | Out-Null
New-ItemProperty -Path "HKCU:\SOFTWARE\Policies\Microsoft\Windows\Explorer" -Name DisableSearchBoxSuggestions -PropertyType DWord -Value 1 -Force
Stop-Process -Name explorer -Force
```

# Debloat (NOT TESTED, TO BE CHECKED)

Note: I recalled copying the command from one of the debloaters on github, check for things I want to debloat and manually run it in Powershell, but I don't remember which one.

https://github.com/ChrisTitusTech/winutil
