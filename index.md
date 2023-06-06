## Part 1 – Debugging Scenario

In Part 1 of this lab report, a hypothetical student encounters a bug in their program and submits a post on edStem detailing the problem. Their post is as follows:

_Note: This is based on a real bug I ran into during a lab however the project is made up. Chat GPT and online resources were used to write portions of the hypothetical programming project._

### Original Student Post

Hi, I have encountered a bug in my program. My program consists of a bash script which gives the first argument as an input to a java program.

The project layout consists of the following files: 

![image](screenshot1.png)

_penguin.txt_, _polarbear.txt_, and _reindeer.txt_ are .txt files containing information about each animal from Wikipedia. The program is run from the command line by running the bash script when the current directory is the program folder. The program also requires the .java file which it compiles.

The Java program I have written is as follows: 

![image](screenshot2.png)

And the Bash script I have written is as follows:

![image](screenshot3.png)


**What environment are you using (computer, operating system, web browser, terminal/editor, and so on)?**

I am using Windows 10 and VSCode for my program. 


**Detail the symptom you're seeing. Be specific; include both what you're seeing and what you expected to see instead. Screenshots are great, copy-pasted terminal output is also great. Avoid saying “it doesn't work”.**

The symptom I am seeing is that when I run the bash script I get the following error code:

![image](screenshot4.png)

As I have both Java and Java JDK installed on my computer, I do not understand why I am getting this error which tells me that 'javac' and 'java' are not recognized.

**Detail the failure-inducing input and context. That might mean any or all of the command you're running, a test case, command-line arguments, working directory, even the last few commands you ran. Do your best to provide as much context as you can.**

The failure inducing input is running the program with one of the three recognized input strings as arguments.

### TA Response

Hi, I'm not sure exactly what the bug is yet but I was wondering if you are on Windows why are you running it with 'bash' in front? Usually you would use git-bash or run the program in a Linux VM as Windows does not natively have Bash commands.

### Student Response

Hi, I have installed Windows Subsystem for Linux which you can use to run Bash commands in a Linux VM integrated into Windows. Your response made me realize the source of the bug: although I have Java and the Java JDK installed on Windows I did not have it installed in the Linux subsystem I was running the commands in. To fix the bugs I had to run the following commands in my Linux VM:

![image](screenshot5.png)

![image](screenshot6.png)

After installing Java and the Java JDK the program worked as expected as you can see in the output below! Thank you very much for your help and I hope you have a good rest of your day!

![image](screenshot7.png)

### Final TA Response

Thank you! I am glad your error is resolved and I hope you have a good rest of your day!

## Part 2 – Reflection

My favorite thing that I learned in the second half of the labs of this quarter was SSH Keys. Logging in is always a time consuming and repetitive task and the ability to reduce that time using SSH keys was extremely helpful both in labs and in personal projects. Although I gained a large amount of knowledge while taking this course, using SSH keys may in the short term be my most frequently used application of the course material as logging into Github is itself such a common and frequent occurence.
