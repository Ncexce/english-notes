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
   Then, I made my first try. it was easy at first,but then I found that the code cannot be compiled successfully. It need a debugger to guide e through the code so I can know what;s going on with the code I wrote.  
   Finally, the compilation was finished. But when I opened it, something hilarious happened. The program started twitching oddly on the screen. I had it enough. I must look for a debugger in unix right now.  



## GDB

   