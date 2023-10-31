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


## HW1

### Q1 A Plus Abs B

Ans: sub add

Caution: the f is the operator

### Q2 Two of Three

Ans ：`(i*i+j*j+k*k-max(i,j,k)*max(i,j,k));`

### Q3 : Largest Factor

Ans:

```
m = 2
    while m < n :
        if n % m == 0 :
            return (int)(n / m)
        else :
            m = m + 1       
    return 1;
```

#### Caution

·format of python

·transform double to int when return

### Q4 Hailstone

Ans : 
```
   step = 1
    print(n)
    while n != 1 :
        if n % 2 == 0 :
            n  = (int)(n / 2) 
            print(n)
        else :
            n = (int)(n * 3 + 1) 
            print(n)
        step = step + 1 ;
    return step;
```
#### Caution : 

##### format of print

##### return is not print 


## Lab01

### Q2

```
 def how_big(x):
...     if x > 10:
...         print('huge')
...     elif x > 5:
...         return 'big'
...     elif x > 0:
...         print('small')
...     else:
...         print("nothing")
>>> how_big(7)
? big
-- Not quite. Try again! --

? none
-- Not quite. Try again! --

? 'big'
-- OK! --
```
Caution: return is not print

```
 positive = 28
>>> while positive: # If this loops forever, just type Infinite Loop
...    print("positive?")
...    positive -= 3
(line 1)? positive?
-- Not quite. Try again! --

(line 1)? 28?
-- Not quite. Try again! --

(line 1)? Infinite Loop
-- OK! --
```
Caution: **Only** while 0 will terminate the while loop

### Q3

#### S1C1

```
 True and 13
? 1
-- Not quite. Try again! --

? True
-- Not quite. Try again! --

? 0001
-- Not quite. Try again! --

? 14
-- Not quite. Try again! --

? 13
-- OK! --
```
Caution: 
1.and,or,not calculate from left to right.
2.When and and both true(include int not zero), return the rightest value
3.When or and all false, return the latest value
```
Boolean operators
使用 and、or、not

注意and和or都是从左到右计算，如and左边为False就返回该False值了

并且这里返回的True或者False不一定是Bool值，如 8 and 9 会返回9

and中，如果所有值都为True，返回最后一个值

or中，如果所有值都为False，也返回最后一个值
```
[参考文献](https://www.cnblogs.com/lcyfrog/p/17020967.html#cs61a%E5%AD%A6%E4%B9%A0%E7%AC%94%E8%AE%B0-week2)

#### S1C7

```

Q: What is the best way to look at an environment diagram to investigate a failing test for question sum_digits in assignment lab01?
Choose the number of the correct choice:
0) python3 ok -q sum_digits
1) python3 ok -q sum_digits --trace
2) python3 ok -q sum_digits -i
3) python3 -i lab01.py
? 1
-- OK! --
```
```
You can quickly generate most ok commands at ok-help.

To use Ok to run doctests for a specified function, run the following command:

python3 ok -q <specified function>
```

[CITE](https://inst.eecs.berkeley.edu/~cs61a/fa22/lab/lab01/#required-questions)


