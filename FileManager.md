#** FileManager

An amazingly useless tool!


##** File Manager prompts

######** Some basic commands of FileManager
'''
- list
- info
- mkdir
- rename
- copy
- quit
'''

######** What the commands can do
'''
If a user wanted to create a folder, they would use mkdir to make the folder inside the java file manager. 
If a user wanted to see the list of folders in a folder they can use this input to look through the folder contents.
If a user wanted to check the info of the file and check to see the history, size, absolute and relative path they could use this input.
If a user wanted to rename the folder, they would call the path of the folder and rename it with a different name. 
If a user wanted to copy the folder and its contents they would need to enter the folder name and chose the path of where the copy folder should be found. 
If a user wants to move a folder they would need to chose the folder and set the path of where it should be moved.
If a user wants to delete a folder, the user must chose the correct folder path. If a user wants to quit the program they can just enter quit and leave.
'''
'''
The main method for the program to do anything is to ask the user for a command, then a folder path and then follow extra instructions if you want to move, copy
and rename. 
'''

######** How would you add the idea of a current folder?
'''
So I think I would implement this command similar to the chose the path file prompt.
I think it would make sense to ask the user when they enter the path if they want to look at any specific folder or not.
If I wanted to make it as a command, it would work similarly to the info command. Ask the user to choose the folder it wants to adjust without opening it, then
continue asking what the user wants to do with the file.
'''

######** How would you add a change folder command?
'''
I think for this command I would implement it similarly as copy/move.
I don't want to open the folder, but I would need to be able to ask the user for the current folder and the next folder they want to see. 
Or I would ask the user to enter the folder that they would like to change from, but I would still need the current folder command to make the change.
'''

######** How would you add a command to display the contents of a file?
'''
I think for this command I would set up similar to info.
The command would need a specific folder to enter and then the user would need to input the specific file to look at.
The only job is to display the contents like info or the command line prompt more.
'''

######** How would you change list to show the difference between files and folders?
'''
I think an adjustment I would make would be in the method. 
It would need to be able to identify folders with some key indication, like if it sees a folder in the path there would need to be a string that identifies it.
The same could be done with the files, it would need to be able to identify them by some ending.
In a normal finder the files have .txt,.pdf or some indication.
Folders don't have any indication, but for a basic command prompt like this it would be important to identify the difference. 
'''
######** How could you clean up some of the code by sing an enum instead of strings for the commands?
'''
The enums would allow more freedom to have them change along the way and call them in different situations.
The strings have to be written out in every prompt, an enum would take the place at each point without having to write it out every time.
The repetition of the code would be less apparent.
'''
######** How would you use the FileOperator class to test the FileOperator class?
'''
One way to test the class would be to set the test class with a lot of assertEquals to check if the message is printed based on the conditional statements.
Making sure methods will work effectively in the code when called.
It's possible certain methods will need a boolean check to test if and when the code is called an assertTrue or assertFalse will work.
It would also be important to following with any classes being called from other sides to call the correct methods.
'''
######** How would test this code? Ho are the testing methods different for each class? Which class cannot be easily tested with unitTests?
'''
As I discussed in the previous question, the testing methods would require a lot of assertEquals for messages and a lot of assertTrue's/assertFalse's.
The tests would differ based on the methods actions and understanding if you need to make the expected equal to the actual or if you are just focused on checking
a true or false condition. 
I think the console class would be difficult to test, because it requires an input from the user to return the input.
Other then that the FileManager method processCommand would be difficult to test because of the amount of case statements that would have to be tested.
'''

######** Does the code, as is, have any obvious bugs? How would you find out?
'''
So there are situations when running the program that it won't identify the folders created even with the correct format.
It is difficult to use the program effectively without any instructions or directions.
The best way to find out anything in this course for bugs is to just throw things at it and see if the try/catch will activate. 
'''

######** Why is the console passed as a parameter to the two constructors?
'''
I think it is because it would be easier to use the console function without having to make it an object every single time.
Being able to designate the class as an instance variable will make the coding process easier to work with.
'''
