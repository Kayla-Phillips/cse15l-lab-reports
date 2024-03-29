# Lab Report 1
## cd
* If no arguments are given, the directory will change to the home directory. This is not an error. The working directory before running this example was `/home/lecture1/messages`.\
![Image](cdNoArg.png)
* If a path to a directory is given as an argument, the directory will change to the current directory + the path to the directory given, assuming that the given path is inside the current directory. If the path isn't accessible,then there will be an error message. Assuming the path is accessible, this will not produce an error.The working directory before running this example was `/home`.\
![Image](cdPath.png)
* If a path to a file is given as an argument, this will result in an error because a file isn't a directory and therefore you can't change directory to a file. The terminal will print an error message saying that the argument is not a directory.The working directory before running this example was `/home/lecture1`.\
![Image](cdFile.png)
## ls
* If no arguments are given, the terminal will print a list of all of the contents (files and folders) in that current directory. The folders will be bolded and blue. The command doesn't change the directory. This is not an error. The working directory before running this example was `/home/lecture1`.\
![Image](lsNoArg.png)
* If a path to a directory is given as an argument, it will list the contents of that new directory without changing the current directory. This is assuming that the given path is accessible within the current directory. If the path isn't accessible, then there will be an error message. Assuming the path is accessible, this will not give an error. The working directory before running this example was `/home`.\
![Image](lsPath.png)
* If a path to a file is given as an argument, then the terminal will print the file name, if the file is accessbile. This is not an error. If the file is not accessible, then there will be an error message. The working directory before running this example was `/home/lecture1`.\
![Image](lsFile.png)
## cat
* If no arguments are given, the command never finishes. Therefore, it will print back to you anything you enter into it. Typing control + c will quit the command. This is not an error. The working directory before running this example was `/home/lecture1`.\
![Image](catNoArg.png)
* If a path to a directory is given as an argument, this will result in an error, and the terminal will print and error message saying that the argument is a directory. This command can only print the contents of a file, so in order to see the contents of a folder, the `ls` command would be more suitable. The working directory before running this example was `/home`.\
![Image](catPath.png)
* If a path to a file is given as an argument, the terminal will print the contents of that file, assuming the file is accessible within the current directory. This is not an error. If the file is not accessible, then there will be an error. The working directory before running this example was `/home/lecture1/messages`.\
![Image](catFile.png)

