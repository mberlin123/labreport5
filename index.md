# Lab Report 5

## Part 1 – Debugging Scenario

In Part 1 of this lab report, a hypothetical student encounters a bug in their program and submits a post on edStem detailing the problem. Their post is as follows:

_Note: This is based on a real bug I ran into during a lab however the project is made up. Chat GPT and online resources were used to write portions of the hypothetical programming project._

### Original Student Post

Hi, I have encountered a bug in my program. My program consists of a bash script which gives the first argument as an input to a java program.

The project layout consists of the following files: 

![image](https://github.com/mberlin123/labreport5/assets/122565198/74479ab5-5f08-4387-92de-014aa71db963)

_penguin.txt_, _polarbear.txt_, and _reindeer.txt_ are .txt files containing information about each animal from Wikipedia. 

The Java program I have written is as follows: 

![image](https://github.com/mberlin123/labreport5/assets/122565198/acee55a8-db83-4038-a439-6856fffcd149)

And the Bash script I have written is as follows:

![image](https://github.com/mberlin123/labreport5/assets/122565198/f94bab87-75c3-43a2-8195-89bac0a6b415)

The 


**What environment are you using (computer, operating system, web browser, terminal/editor, and so on)?**

I am using Windows 10 and VSCode for my program. 


**Detail the symptom you're seeing. Be specific; include both what you're seeing and what you expected to see instead. Screenshots are great, copy-pasted terminal output is also great. Avoid saying “it doesn't work”.**

The symptom I am seeing is that when I run the bash script I get the following error code:

![image](https://github.com/mberlin123/labreport5/assets/122565198/fdd5517d-c838-41f3-89a0-069c77d894e1)

As I have both Java and Java JDK installed on my computer, I do not understand why I am getting this error which tells me that 'javac' and 'java' are not recognized.

**Detail the failure-inducing input and context. That might mean any or all of the command you're running, a test case, command-line arguments, working directory, even the last few commands you ran. Do your best to provide as much context as you can.**

The failure inducing input is running the program with one of the three recognized input strings as arguments.

### TA Response

Hi, I'm not sure exactly what the bug is yet but I was wondering if you are on Windows why are you running it with 'bash' in front? Usually you would use git-bash or run the program in a linux VM as Windows does not natively have Bash commands.

### Student Response

Hi, I have installed Windows Subsystem for Linux which you can use to run Bash commands in a Linux VM integrated into Windows. Your response made me realize the source of the bug: although I have Java and the Java JDK installed on Windows I did not have it installed in the Linux subsystem I was running the commands in. After installing Java and the Java JDK the program worked as expected! Thank you very much for your help.
