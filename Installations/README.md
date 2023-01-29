# Installation

1. A **package manager**: Chocolatey (for Windows) or Homebrew (for Mac)
2. **Git & Github** - version control & platform used to store and manage code.
3. **VS Code** - a lightweight development environment (IDE).
4. **Python** - a software language useful for developing new programs and scripts.
5. **SQL** - Structured Query Language (SQL) is defined as a standard programming language utilized to extract, organize, manage, and manipulate data

## Installing Chocolatey and Core Tools

1. Open "cmd.exe" as an administrator.
2. Paste and run the [Chocolatey.org](https://chocolatey.org/docs/installation#install-with-cmdexe) install script:

```
cmd
```
```
@"%SystemRoot%\System32\WindowsPowerShell\v1.0\powershell.exe" -NoProfile -InputFormat None -ExecutionPolicy Bypass -Command " [System.Net.ServicePointManager]::SecurityProtocol = 3072; iex ((New-Object System.Net.WebClient).DownloadString('https://chocolatey.org/install.ps1'))" && SET "PATH=%PATH%;%ALLUSERSPROFILE%\chocolatey\bin"
    
```
    
```
  choco upgrade chocolatey
```


3. Install git.

```
choco install -y git.install --params "/GitOnlyOnPath /SChannel /NoAutoCrlf /WindowsTerminal"
```

4. Install core tools:

```
choco install -y choco-protocol-support chocolateygui sudo terraform vscode
#choco install -y python3
choco install python --version=3.9.5
choco install -y docker-desktop

choco install 7zip.install --pre
```


```
choco install dbeaver
```

```
choco install awscli
choco install saml2aws
```


## Installing additional tools

Install any of the below that would be useful for your project, or find additional packages using [chocolatey.org/packages](https://chocolatey.org/packages)

- [choco://anaconda3](choco://anaconda3) or [choco://miniconda](choco://miniconda)
- [choco://awscli](choco://awscli)
- [choco://GoogleChrome](choco://GoogleChrome)
- [choco://wsl](choco://wsl)
- [choco://wsl-ubuntu-1804](choco://wsl-ubuntu-1804)

```
python -m virtualenv .
.\scripts\activate
```



