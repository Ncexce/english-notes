# A Long Road - Security Break



## Seed of Breaking

   10:00 p.m. , Technology Center.  

> Radio: Caution! Caution! Kernel panic. Kernel panic.  
> Radio: Kernel replacing required.  
> Radio: Kernel file not found. Please replace the kernel file and reboot.  



## Decision I "Working System Replacing"

   The next morning, we wake up shocked. The security border is destructing. This is not a good new. One of the basic fact is that the security system's security border is the basic defense of the technology center. Without it, the technology center will be attacked by a bunch of useless data.  
   Unfortunately, the department's teacher is not here recently. This means that we need to solve this problem ourself. Checking the system log, we surprisingly found that the system was hit by a malicious command which only would be done by the people Inside the department.  
   But we don't have any time to be suspicious of other people. After a while of calculation, we know that the border will halt in 3 months.  
   Emergency meeting was held. And we've been allocated some missions. I has the busiest mission: Rewrite the kernel code in order to rebuild it. I got my permission to bring my personal laptop. Phew. Time for work. First things first, I decided to get my working system replaced.  
   After some trouble, the new system - Ubuntu 20.04 LTS was installed.



## First Construction

### 1. Gedit

   Gedit is the main editor of the desktop environment GNOME.  When I first opened it, I was attracted by its fantastic interface. This is the simplest text editor I have ever used. At this moment, I've decided to use gedit as mt default text editor.

### 2. GCC

   After transforming into linux, I found there is no build tools in linux yet, so I can't possibly click a button to build a project. To make matters worse, I don't even have a compiler to compile source codes. Searching the application store and browsing the internet, I found that the compiler in linux is GCC - GNU Compiler Collection. I used the command that the web gave:  

```shell
sudo apt-get install gcc
```

Installation complete. I think I have the compiler now, for even though I still don't know how to use it.



## GNOME Terminal

> #### Remote Assist #38CAD7 - 2 active connections  
>
> ##### Thread #1  - ID: Auto-email  
>
> If you are watching this, it means that you are stricken by three things.  
> First, I cannot come back right now but the security system bay be broken. So you have to repair it yourselves.  
> Next, The kernel files may be missing and you may still don't know the infos of the security system. This is the most complicated thing because a kernel needs the traffics with the base hardware.  
> Finally,  I guess it's you, Ncexce to do the job of programming. Considering on your side, you should been already switched on the new OS linux. This is a good thing because its legacy development route is very useful, especially for kernel developing.  
> Let me guess that you have switched to Ubuntu 20.04 LTS since it's the most popular system right now.
>
> ##### Thread #2 - ID: Description
>
> Ubuntu 20.04 LTS Uses the GNOME desktop system, which uses the GNOME shell as the terminal. Use the keyboard shortcut <kbd>Ctrl</kbd> + <kbd>Alt</kbd> + <kbd>T</kbd> to open the terminal. You can invoke the GCC compiler directly using the gcc command. There are many other ways of invoking the compiler. Now you've get to be use to using the terminal. I will talk about the shell usages. Firstly, the shell will execute the command that we give, this is with no doubt. And when we give commands, the shell will also show us the process usually.  
> Shell commands are all programs, and many of them was build-in programs, such as `mkdir`,`shutdown`,`rm`,etc. the gcc which you installed was also like this.  
> A full command will act like this:
>
> ```shell  
> command-name [-arg1|-arg2][--argument1|--argument2] IOFiles
> ```
>
> `command-name` is the name of the command.  
> `-arg1`,`-arg2`,`--argument1`,`--argument2` is the arguments, which the abbreviations written in one dash and the full one in two dashes.
> `IOFiles` is the file\(s\) you want to process. For example:  
>
> ```shell
> gcc -c -o outputexecutive main.cc
> ```
>
> this will let the compiler read the source code `main.cc` and output the executable file `outputexecutive` to the working directory.  
> As for the working directory, it's even easier. it is where the shell is located at. you can check it by the command `pwd` .  
>
> GCC have some main arguments including the `-o`,`-c`. The `-o` option will let you specify where the processed file will be placed. The `-c` option will let the compiler only compile without linking directly. This is very useful if you are using multiple headers.
>
> If you have some extra needs or need some more help, always use the `man` command. This command's usage is: `man command-name`. i.e.`man gcc`  
> 
>
> This is the end of this remote assist. Now make your first try. Good luck.
>
> ***



## First Failure

   Completed reading this remote assist, and now I know how to use my programming skill to repair it. So after several hours of practicing, I started to write my first header. thanks to the editor gedit, my process has become faster.  
   Then, I made my first try. it was easy at first,but then I found that the code cannot be compiled successfully. It need a debugger to guide e through the code so I can know what's going on with the code I wrote.  
   Finally, the compilation was finished. But when I opened it, something hilarious happened. The program started twitching oddly on the screen. I had it enough. I must look for a debugger in unix right now.  



## GDB

   Browsing the internet, I have found the popular debugger for the linux system. It seems it's called GDB, full name GNU Debugger. I haven't research its usage yet. Then I've tried the command `man gdb`, but I only got a lot of complicated arguments and descriptions. Yet, I only know that it's a powerful debugger.  
   Opening a browser, I tried to find something about the GDB. Then I run some commands on the web, such as: `gdb run`, `gdb filename`, etc.  
   Then, I gradually got on the operation of the debugger GDB. It was indeed a powerful debugger, but a it was a little hard to use.  
   However, I still don't know how to set a breakpoint.

## Another Chance Unselected

   Recently, I've noticed a newly upped stream, it's called the IDE, The `Integrated Development Environment`. It combined the compiler, the debugger, the text editor together. It seems it's a much more convenient option, so I decided to give it a try.  
   The one I've seen is called the Kdevelop, the most "Advanced" one. I followed their command:

```shell
sudo apt-get install kdevelop
```

   Installation complete. `Alt+F2`,`kdevelop`, launch. Well, in my expectations, I've seen a complicated GUI, just like in windows. However, getting used to the mode in linux, I have no interests in it.  
   I tried to build a simple software, but then a message box popped up and showed that I needed a kit to build. I was fed up. Even it's powerful, I don't want to use it anymore.

## Happy Vimming!

> #### Overall Development Progress: 20%  |  Security Break Countdown: 75 days

   Recently, Gedit cannot meet smy requirements anymore. Its operations relies on the mouse too much, which makes me sick. I need to find a brand new text editor for my development. Wait. What is this?

> #### Remote Assist #7DC524 - 2 Active Connections
>
> ***
>
> ##### Thread #1  ID: Auto-email - Displaying in: RAW
>
>    I think the time is up now. You may need a new text editor which uses only the keyboard to operate. Don't worry. I've found a nice editor for you before, and I think you may be familiar with it.  
>    It is called `Vim` .  
>    It can only run in terminal mode without a gvim GUI. Its operation is very easy. I will transfer you a tutorial. Well, Remember to read the manual carefully. Bye.
>
> ##### Thread #2  ID: File-transfer - Displaying in: Transferred
>
> ```shell
> # Install the Vim editor:
> sudo apt-get install vim
> 
> #run the vim with a file i.e. filetoedit.cc
> vim filetoedit.cc
> 
> #Save
> :w
> 
> #Quit
> :q
> 
> #Save and quit
> :wq
> 
> #Force operation
> :some-command! #Add a character "!"
> 
> #Enter insert mode
> i, a
> 
> #Go back to command mode
> Esc
> #Get help
> :help some-topic
> ```
>
>    Well, this is the basic operation. Remember!
>
> ***

   Phew. Well, I think this is the start of my journey of using Vim. Good luck to me!

## Full Terminal Operations

   After implementing vim to my operations, I found one thing, the operation can nearly be completed in the GNOME Terminal. Then I discovered that Vim can execute external command, which means I can do everything in the vim editor. Things cannot be better. Then, what I need to do is to try my best to develop faster.  
   Things can be changed. When browsing the stack overflow website, I found that there is another compiler called `clang` . Trying and testing this compiler, I found that this compiler can compile faster, but not all the library functions implemented.  
   So, I'm going my next phase - using multiple compiler, and using the terminal in several different ways.



## Incident Fall

> #### Overall Development Progress: 32% | Security Break Countdown: 68 days

   Incident can happen at any time, especially when you are busy dealing with some difficult problems such as debugging a important header file.  
   The worst header, the hardware header, `touchscreenbase.h`, needs me to customize the debugger GDB. I didn't want to do that at first, but I found I can improve my speed if I do that. So, I decided to customize.  

### Phase I

   The first step was to update the configuration file, `preference.conf`. I chose to simplify a few commands in order to improve my speeds.  
   I also added a few new commands for me set breakpoints. Save. OK, the first phase was finished.

### Phase II

   Entering the second phase, I felt a bit of stress. After all, I need to refresh the whole debugger without any other manuals and debuggers. All I have is a shell and some other applications.