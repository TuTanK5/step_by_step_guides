# Setup WSL
To be sure, follow the manual install guide → https://learn.microsoft.com/en-us/windows/wsl/install-manual 

Basically:
Enable the Windows Subsystem for Linux Windows Feature:

```dism.exe /online /enable-feature /featurename:Microsoft-Windows-Subsystem-Linux /all /norestart```

Enable Virtual Machine Windows Feature 

```dism.exe /online /enable-feature /featurename:VirtualMachinePlatform /all /norestart```

Update WSL

```wsl --update```

Set WSL2 as default version 

```wsl --set-default-version 2```

Install WSL with default distribution (Ubuntu)

```wsl --install```

# Setup Ubuntu
Wait for Ubuntu to be extracted, should be a couple of minutes, then set up a username & password.

Update packages with sudo apt update & sudo apt upgrade.

Install zsh → https://github.com/ohmyzsh/ohmyzsh/wiki/Installing-ZSH

Intstall oh-my-zsh https://github.com/ohmyzsh/ohmyzsh

Install poetry → https://python-poetry.org/docs/#installing-with-the-official-installer

Set git-credential-manager https://github.com/git-ecosystem/git-credential-manager/blob/release/docs/wsl.md#configuring-wsl-with-git-for-windows-recommended
# Setup VS Code
Make sure VS Code is installed on host, then from wsl home 

```code .```

# Setup Docker
Follow the official guide to install Docker Desktop with WSL support → https://docs.docker.com/desktop/features/wsl/#download

To verify, go to wsl home 

```dir & run docker ps -a & docker run hello-world```
