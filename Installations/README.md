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

## MacOS Development

## Installing Homebrew and Core Tools

1. Open "Terminal".
2. Paste and run the [Homebrew](https://brew.sh) install script:

```bash
/usr/bin/ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"
```

3. Install git.

```cmd
brew install git
```

4. Install core tools:

```cmd
brew install cask docker python3 terraform
brew cask install cakebrew visual-studio-code
```

## Installing additional tools

After following the instructions from the above, you should now have the **Cakebrew** app installed, which gives a friendly GUI on top of the Homebrew installer.

To install any additional programs, either open the **Cakebrew** app or copy-paste the below samples into a Terminal window. (You can also find additional packages at [https://brew.sh](https://brew.sh).)

- `brew install awscli`
- `brew cask install google-chrome`


##  [VSCode](https://code.visualstudio.com/docs/python/python-tutorial) [Setup](https://code.visualstudio.com/docs/setup/linux)
```
brew install --cask visual-studio-code

# sudo snap install --classic code # linux
```
