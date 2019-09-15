# Sea-Battle-2
This is an open source battleship clone made for CS232 (Computer Programming 2) in Fall 2017. 
It is a wonderful look at model view controller for beginners.


## Getting Started
This game can be utilized by any machine running Java.

### Prerequisites
Luckily, there is not much required to run the project. The GUI is a Swing GUI which is supported via Java 8 through 2025.

You'll need
```
Java
```
### Installing
Below are the instructions to install Java.

#### Java
```
1) Navigate to https://www.java.com.
2) Click Java Download
3) Read the Oracle Technology Network License Agreement for Oracle Java SE
4) If you agree to the above agreement, click the Agree and Start Download Button.
5) Once downloaded, open the installer and follow the on screen instructions.
6) Finally, you may need to add Java to the PATH.
```
##### Windows
###### Windows 10 and Windows 8
```
1) In Search, search for and then select: System (Control Panel)
2) Click the Advanced system settings link.
3) Click Environment Variables. In the section System Variables, find the PATH environment variable and select it. Click Edit. If the PATH environment variable does not exist, click New.
4) In the Edit System Variable (or New System Variable) window, specify the value of the PATH environment variable. Click OK. Close all remaining windows by clicking OK.
5) Reopen Command prompt window, and run your java code.
```
###### Windows 7
```
`) From the desktop, right click the Computer icon.
2)Choose Properties from the context menu.
3) Click the Advanced system settings link.
4) Click Environment Variables. In the section System Variables, find the PATH environment variable and select it. Click Edit. If the PATH environment variable does not exist, click New.
5) In the Edit System Variable (or New System Variable) window, specify the value of the PATH environment variable. Click OK. Close all remaining windows by clicking OK.
6) Reopen Command prompt window, and run your java code.
```
###### Windows Vista
```
1) From the desktop, right click the My Computer icon.
2) Choose Properties from the context menu.
3) Click the Advanced tab (Advanced system settings link in Vista).
4) Click Environment Variables. In the section System Variables, find the PATH environment variable and select it. Click Edit. If the PATH environment variable does not exist, click New.
5) In the Edit System Variable (or New System Variable) window, specify the value of the PATH environment variable. Click OK. Close all remaining windows by clicking OK.
6) Reopen Command prompt window, and run your java code.
```
###### Windows XP
```
1) Select Start, select Control Panel. double click System, and select the Advanced tab.
2) Click Environment Variables. In the section System Variables, find the PATH environment variable and select it. Click Edit. If the PATH environment variable does not exist, click New.
3) In the Edit System Variable (or New System Variable) window, specify the value of the PATH environment variable. Click OK. Close all remaining windows by clicking OK.
4) Reopen Command prompt window, and run your java code.
```
##### Mac OS X
To run a different version of Java, either specify the full path, or use the java_home tool:
```
% /usr/libexec/java_home -v 1.8.0_73 --exec javac -version
```

##### Linux/Solaris
To find out if the path is properly set:
In a terminal windows, enter:
```
% java -version
```
This will print the version of the java tool, if it can find it. If the version is old or you get the error java: Command not found, then the path is not properly set.
Determine which java executable is the first one found in your PATH
In a terminal window, enter:
```
% which java
```

###### Set the PATH permanently
To set the path permanently, set the path in your startup file.

###### Bash Shell
Edit the startup file (~/.bashrc)

1) Modify PATH variable
```
PATH=/usr/local/jdk1.8.0/bin:$PATH
export PATH
```
2) Save and close the file
3) Load the startup file
```
% . /.profile
```
4) Verify that the path is set by repeating the java command
```
% java -version
```

###### C Shell (csh)
Edit the startup file (~/.cshrc)

1) Set Path
```
set path=(/usr/local/jdk1.8.0/bin $path)
```
2) Save and close the file
3) Load the startup file
```
% source ~/.cshrc
```
4) Verify that the path is set by repeating the java command
```
% java -version
```

## Deployment
To run this as a standalone project:
1) Navigate to the completed executable
```
dist/
```
2) Run via the Command line or Terminal
```
java -jar build/libs/SeaBattleII.jar
```
## Usage as a Teaching Tool
This project is amazing to teach the ins and outs of MVC to new students.
To navigate to the source code:
```
src/edu/jsu/mcis/seabattleii
```
In this code, take a look at the abstract MVC as well as the Default MVC.

### Items of Note
Model
```
deployFleets - Shows interaction with the controller to update the view
setStatus - Show interaction with the controller to update the view
```
Abstract Controller
```
add/remove (model/view) - Registers a model and view with the controller
setModelPropoerty - Used to manipulate the model
```
ViewTrackingGrid/ViewPrimaryGrid/ViewMainWindow
```
modelPropertyChange - Initiates a property change within the controller to update the model (various uses across all three view classes)
```
Object Oriented Programming
```
Square - A simple class showcasing protected variables and public getters. Used as a parent class for various classes within the project.
Grid - A class that explores overriding of methods (see string builder) as well as the usage of custom classes within another class
```
## Built With
* [Java](https://www.java.com) - Main Language
* [Netbeans](https://netbeans.org/) - IDE

## Versioning
There is none!

## Authors
* Joshua Williamson - Final Product - [jwilliamson5](https://github.com/j-williamson5)
* Jay Snellen - Initial Framework/Abstract Classes - [jsnellen](https://github.com/jsnellen)

## Acknowledgments
Many thanks to Jay Snellen for writing the intial framework for this project as well as procuring the sounds/graphics!
Remember to have fun!
