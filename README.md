# Installation guide for NVM in windows
Node Version Manager (NVM) on Windows

### Prerequisite:

Uninstall existing node
Uninstall existing npm

Uninstall existing version of node since we won’t be using it anymore
Delete any existing nodejs installation directories.( e.g. “C:\Program Files\nodejs” OR C:\Program Files (x86)\nodejs ) that might remain. NVM’s generated symlink will not overwrite an existing (even empty) installation directory.

Delete the npm install directory at C:\Users\[Your User]\AppData\Roaming\npm We are now ready to install nvm. Download the installer from https://github.com/coreybutler/nvm/releases

Delete the existence of nvm (C:\Users\xxx\AppData\Roaming\nvm), basically, manually delete the nvm dir.

To upgrade, run the new installer. It will safely overwrite the files it needs to update without touching your node.js installations. Make sure you use the same installation and symlink folder. If you originally installed to the default locations, you just need to click “next” on each window until it finishes.


### Installation

 1. Download nvm for Windows

 2. Choose nvm-setup.zip

 3. Unzip & click on installer.

 4. Check if nvm properly installed, In new command prompt type nvm.

 a. Add in Environment variable: 
    Nodejs, Nvm and Npm installation directory path

    * C:\Program Files\nodejs 
    * C:\Users\[Your User]\AppData\Roaming\nvm
    * C:\Users\[Your User]\AppData\Roaming\npm

 5. Install node js using nvm : nvm install <version> : The version can be a node.js version or "latest" for the latest stable version

 6. check node version - node -v 

 7. (Optional)If you want to install another version of node js - Use STEP 5 with different version.

 8. Check list node js version - nvm list

 9. If you want to use specific node version do - nvm use <version>


###  NVM Basic Commands

+ View remote available versions of Node.

`$ nvm ls-remote`

+ View local installed versions.

```sh
$ nvm ls
```

+ Install a specific version.

```sh
$ nvm install <version number>
```

+ Switch to a specific version of Node.

```sh
$ nvm use <version number>
```

+ Uninstall a specific version.

```sh
$ nvm uninstall <version number>
```

+ Displays the current running version of NVM for Windows.

```sh
$ nvm version 
```

### Errors
  - If you get error like npm/nvm/node not recognized as an internal or external command => Go to step 4


#### Reference Links

* [DigitalDrummerj]
* [MS DOCS]

[DigitalDrummerj]: https://digitaldrummerj.me/windows-running-multiple-versions-of-node/
[MS DOCS]: https://docs.microsoft.com/en-us/windows/nodejs/setup-on-windows

**Please feel free to contribute to the project,create a pull request**

