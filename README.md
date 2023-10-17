# CS61A
## Lab0
### Set up
#### step 1 : Install ubuntu in windows

Search powershell in 'start' menu, right click and check 'Run as administator'.
Then, type `wsl --install ` to install the setup progress（虚拟机？）.

And following the instruction which powershell give to you.(My is to restart the system(needs update).

Finally, type `wsl --install -d ubuntu`

**Note**: When type new username in ubuntu, remember not to type upper character.

#### step 2 : Install Python 3

Type `sudo apt install python3 ` to install  <!--apt: an instruction progress which install, update, delete and control application packs.-->

To view the version, you can type ` python3 --version`

#### step 3 ： Install a text editor

Install the extension in VSCode.

There are some instruction to use VSCode to open files in WSL.

[Insturction for opening files in VSCode](https://code.visualstudio.com/docs/remote/wsl#_open-a-remote-folder-or-workspace)

#### step 4 : Try to use VSCode like a WSL terminal

What we just to do is:

Type　` wsl ` in windows powershell, then type ` code .`

### Using the Terminal

First make sure we are in wsl(Windows) or Terminal（MacOS).

#### 1 : have a look at home directly

` echo $HOME`

### Walkthrough : Organizing your files

#### 1 : Directories

type ` ls ` to look through files in this directory

ls : short of list

Caution : Since I have my dell initialization in Japanese and setup backup, my path of desktop is `~/Onedrive/デスクトップ　`

#### 2 : Changing directories

My home directory is `/home/aki `, type ` cd /home/aki' to enter the home directory.

command : short of change directory

#### 3 : Making new directories

Now I wanna create a CS61A directory to save my note and code in CS61Aa, just type ` mkdir cs61a ` in the directory which I wanna create cs61a.

mkdir : short of making new directory

#### 4 :  More directory changing

` cd .. ` : return to the parent directory. ` .. ` means **the parent directory**

` cd ~ ` ： return to the home directory. ` ~ ` means the home directory

#### 5 ： Downlanding the assignment

If we've already downloaded ` lab00.zip`. type ` ls ~/Downloads ` to check whether the zip is in Downloads.

#### 6 ： Extracting starter files ( to unzip .zip files )

too lazy to install unzip in powershell

#### 7 : Moving files

When move a from A to B ( A and B is directories )

Type ` mv A B `

### Review Python basics 

### Finish Lab

Following the instruction in lab00.py, and type ` python3 ok ` when in lab00.

### Some WSL Instruction in Chinese 

[Chinese WSL Instruction](https://mp.weixin.qq.com/s?__biz=MzA3NjY2NzY1MA==&mid=2649740495&idx=1&sn=a7c98cc5db24a572ce78b24f581fe425&chksm=8746baa2b03133b467dd869409f6cf45a5e4438a6e3f8368372806ad45ff6933923b2946eb93&scene=27)

