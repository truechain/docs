## Installation - How to get and install TrueChain

### TrueChain Development Preparation- Building Environment for Mac Users

Author: Wubin Yang
Review: rectinajh  
Translator: Paul Wang

The development language for TrueChain is Golang, we need to install the Golang development environment, and the version of Golang is required to be 1.7 or above.

#### Download and install Golang
First download the Golang installation package, as the official website is blocked by the Great Firewall, you can download from the following address. (currently it’s accessible, if not, please find other available download address.)

[https://studygolang.com/dl/golang/go1.10.3.darwin-amd64.pkg](https://studygolang.com/dl/golang/go1.10.3.darwin-amd64.pkg)

Click the link to download the installation package, and then execute the installation package to install Golang.

#### Configuration environment
### Check installation results
After successful installation, execute the following command in the console window:

`go version`

If the installation is successful, you will get the following output in the console window:

`go version go1.10.3 darwin/amd64`

We are now installing the latest version of the current go v1.10.3. You can then view Golang other command-line tools through the `go help` command.

#### Setting GOPATH environment variables
Add a GOPATH environment variable, set the GOPATH value to your Golang download code path. Open terminal and type
`cd ~`

enter user home directory in Mac, then type 
`ls -all`

command to see if there is a .bash_profile. Use vim to open the .bash_profile 
and add the following line of code: 
`export GOPATH=/Users/yangwubing/go`

it means that our Go code and dependency packages are placed under this directory. After setting up, you can check with the .

`go env`

command to see if the configuration is successful. There will be a value of `GOPATH` in the output, and if it is set successfully, the value should be the `"/users / yangwubing / go"` as you just set. 
Then the Golang environment is installed and configured.

#### Install Git environment
Most of the Golang code and dependency packages are downloaded using git, you need to install the Git environment. There are many ways to install Git on Mac. The easiest way is to install Xcode Command Line Tools. In Mavericks (10.9) or later, try running the git command in Terminal. you will be prompted to install Git package if the command-line developer tool has not been installed, 

If you want to install newer versions, you can use the binary installer. The officially maintained OSX Git installer can be downloaded from the Git official website at
 [http://git-scm.com/download/mac](http://git-scm.com/download/mac)


#### Installation of Integrated Development Environment
IDE can improve development efficiency, here I recommend GoLand as Golang IDE

#### Install Goland IDE
Since IntelliJ Idea Go plug-in is no longer available, I introduce GoLand, as it is has 30 days free trial. go to the Web site.
 [https://www.jetbrains.com/go/download/#section=mac](https://www.jetbrains.com/go/download/#section=mac)
 to download the GoLand installation package.
Double-click the installation package to complete the installation.

![](https://gitee.com/ywbrj042/myimages/raw/master/truechain/goland.jpg)
After installation, find the GoLand icon in Launchpad, launch GoLand, you can choose the option of 30 days trial in pop up window, then switch the GoLand main interface.


#### Download the code and import
#### Download Source code
Import the TrueChain source code in the console using the following command

`go get github.com/truechain/truechain-engineering-code`

the source code will be downloaded to the configuration of the GOPATH path.
![](https://gitee.com/ywbrj042/myimages/raw/master/truechain/download_truechain_code.jpg)


## Import Source Code
You can import the source code by Choose File -> Open -> select GOPATH/src/github.com/truechain/truechain-engineering-code

![](https://gitee.com/ywbrj042/myimages/raw/master/truechain/import_truechain_code.jpg)

When the directory is opened, a new go project is automatically generated, so you can start writing or modifying the TrueChain code.
![](https://gitee.com/ywbrj042/myimages/raw/master/truechain/goland_truechain_project.jpg)

## Note
By now, the TrueChain development environment has been built. In the actual operation process, due to the domestic network environment limitation, there might be some problem such as link failure or slow download speed of GitHub. you may not be able to follow the document steps, you can search the latest available website address in the Internet. Or use proxy servers to speed up and other methods to solve the problem.

