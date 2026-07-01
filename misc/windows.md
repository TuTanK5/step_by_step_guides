# Activation

https://github.com/massgravel/Microsoft-Activation-Scripts

# Disable web search in start menu

```
New-Item -Path "HKCU:\SOFTWARE\Policies\Microsoft\Windows\Explorer" -Force | Out-Null
New-ItemProperty -Path "HKCU:\SOFTWARE\Policies\Microsoft\Windows\Explorer" -Name DisableSearchBoxSuggestions -PropertyType DWord -Value 1 -Force
Stop-Process -Name explorer -Force
```
