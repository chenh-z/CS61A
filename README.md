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

#### 2 : 

### Some WSL Instruction in Chinese 

[Chinese WSL Instruction](https://mp.weixin.qq.com/s?__biz=MzA3NjY2NzY1MA==&mid=2649740495&idx=1&sn=a7c98cc5db24a572ce78b24f581fe425&chksm=8746baa2b03133b467dd869409f6cf45a5e4438a6e3f8368372806ad45ff6933923b2946eb93&scene=27)

