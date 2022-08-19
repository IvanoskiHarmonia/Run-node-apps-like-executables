# Runnable for node applications

## Why this repo?
Let me explain, it's not really runnable but it is a way to run your node apps like a runnable.

-	Disclaimer! This is not some breakthrough in programming, nor did I invent it, but I was wondering since there is an executable for most apps that run with a double click on them, there must be a way to do something similar with the node applications that I have already built.
-	Starting a node application is not really easy as everybody who deals with it know, actually it is quite hard:
	1. First you need to go to the folder where your node file is
	2. You need to open the terminal and write ```node app```, or a ```node <name of your function>```,
	3. Then open your browser and write ```localhost:3000/```
- This for me it is a to much trouble to do whenever I want to use one of my apps, but as the name of my repo suggests. 

## How to create runnable for Node apps - Windows

First and for most, credit where credit is due, I found how to do this, on this [Thread](https://stackoverflow.com/a/25817258/15541450) on stack overflow.

1. Create a shortcut file on the desktop like this: 
![Create shortcut](https://github.com/ivanoskiHarmonia/Run-node-apps-like-executables/blob/main/images/shortcut.jpg?raw=true)
2. When you approach this window:
![Create shortcut](https://github.com/ivanoskiHarmonia/Run-node-apps-like-executables/blob/main/images/location_of_command.jpg?raw=true)
	You can follow this logic: ```C:\Windows\System32\cmd.exe /k your-command```
	-	The command for opening node apps for my last project [Notes-app](https://github.com/IvanoskiHarmonia/Notes-app), which is on my local machine is: 
```cd "path/to/my/folder/on/local/machine" && node app | start chrome http://localhost:<listened_port>```
		* If you want to know more about the symbols meaning between the commands, here is a [thread](https://stackoverflow.com/a/8055430/15541450) from stack overflow that explain everything, and also you should probably check the [documentation](https://docs.microsoft.com/en-us/previous-versions/windows/it-pro/windows-xp/bb490954(v=technet.10)).
	- This is how my final version of the script looks before I press the Next button: 
``` C:\Windows\System32\cmd.exe /k cd "path/to/my/folder/on/local/machine" && node app | start chrome http://localhost:3000```
3. After pressing yes you will encounter this window: 
![Final phase](https://github.com/ivanoskiHarmonia/Run-node-apps-like-executables/blob/main/images/Final_phase.jpg?raw=true)
	- Here we see the cmd.exe, you can enter whatever name you desire. for me, I entered **Notes** and pressed finish.
4. In the end you will see your app on your desktop and the only thing you need to do now is double-click it and your node application will run immediately.

---

If anyone has done anything like this on other OSs and wants to add the **macOS** and **Linux** way of doing this, please reach out to me on social media or submit a pull request and I will approve it immediately.