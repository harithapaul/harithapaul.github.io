---
layout: post
title: How to run C/C++ code in VSCode for Windows-in 2 minutes!
author: haritha
categories: [ Technology ]
tags: [ Hacks ]
image: assets/images/VSCode.jpg
description: A quick tutorial to use your favorite VSCode editor to run C or C++ programs in under 2 minutes.
disqus: true
---
When Visual Studio Code or VSCode becomes your favourite editor, and when you don’t feel like switching into any other IDE just to compile your C/C++ program, to top it all off that too on a Windows System.!, can be a little tricky.

I’ve searched it, so have you, and the easiest solution that you get online is to install CodeBlocks and test your snippets in that, while using Windows. Nah, I want to do it in my VSCode itself.

## So How?

Visual Studio Code has a plethora of extensions and choosing the right extensions can make the job hassle free.

**Disclaimer**: This small hack is to run only individual programs - while you’re learning C/C++, if you want to test your snippets, verify algos in text so on and so forth. This method cannot be extended for development purposes using C/C++. Building projects is not possible in this method. 
So if your purpose is former, keep reading.!

### Install GCC/G++ compiler:
 
I realized I didn’t even have a gcc compiler installed in my machine. Searching online gave me a hefty amount of solutions which I think was not that simple and lucid enough, but of course it was doable. Here, I’m just consolidating my easiest way to set your compilers:

#### Step 1: Install chocolatey

Chocolatey is a package manager for windows that helps to install packages easily without the burden of downloading exe files and hitting numerous ‘nexts’.
- Open Powershell in Administrator mode
- Type following commands:
```sh
Set-ExecutionPolicy Unrestricted
```
```sh
Set-ExecutionPolicy Bypass -Scope Process -Force; [System.Net.ServicePointManager]::SecurityProtocol= [System.Net.ServicePointManager]::SecurityProtocol -bor 3072; iex ((New-Object System.Net.WebClient).DownloadString('https://chocolatey.org/install.ps1'))
```

#### Step 2: Install MingW
MingW is a collection of compilers for windows. To install MingW, after installing chocolatey, run the command:
```sh
choco install mingw
```

### Install Extension in VSCode
Go to Extensions-> **Install Code Runner (.run)** and **C/C++** extension by Microsoft.

Type in your code snippet and hit the play button at top right corner.

Enjoy the output.!




