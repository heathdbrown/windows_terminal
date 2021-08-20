# windows_terminal
> Configuration settings for my Windows terminal

## Getting Started
- https://docs.microsoft.com/en-us/windows/terminal/get-started

## PowerLine
- https://docs.microsoft.com/en-us/windows/terminal/custom-terminal-gallery/powerline-in-powershell
- https://github.com/microsoft/cascadia-code/releases

## Installation

- https://github.com/microsoft/cascadia-code/wiki/Installing-Cascadia-Code

```
copy settings.json $USERPROFILE\AppData\Local\Packages\Microsoft.WindowsTerminal_8wekyb3d8bbwe\LocalState
```

## SSH-agent

https://docs.microsoft.com/en-us/windows-server/administration/openssh/openssh_keymanagement

In an administrative powershell terminal add the following to have the ssh-agent start automatically
```Powershell
get-service -name ssh-agent | set-service -StartupType Automatic
```

In a standard powershell/windows terminal add the key
```Powershell
ssh-add ~/.ssh/idrsa
```
