Capstone-Project-5

Poised Project Final

Project Details:

Description

The Poised Project is a program written the Java language that was created to fulfill the level 2 task requirements for the Hyperion Development Software Engineering Bootcamp. The program is designed to be a project management system for a small structural engineering firm called 'Poised'. The company Poised works on various buildings in an engineering capacity to ensure structural integrity. The Java program was written to assist the company in keeping track of the many projects that they work on. The program keeps track of project information by writing and saving details of projects to external text files.

Functionality

There are five Java classes that run the project management system for the user. These will be explained briefly to outline the overall functionality of the program:

The 'InputChecks.java' class file is a superclass that basically contains code to check different types of user inputs that may be used with the program. It has three methods that check whether a user has correctly entered a string (list of words or sentence), integer (number) or double (number with decimal points) respectively and if not, the user is repeatedly asked to re-enter their input until it is correct. This type of defensive programming ensures that the program is robust and able to deal with user errors.

The 'Project.java' class file contains a method to add a new project object, which is then written to the external text file, 'CurrentProjects.txt'. When called on in the main menu class, this method will prompt the user for new project information (e.g. project name, project number etc.), display the project object once complete, and write the project details to the text file.

The 'Person.java' class file contains a constructor and method which allow the user to add a new person object for a project; which basically contains contact details for a particular person (e.g. a contractor, customer etc.). When accessed from the main menu class, this method prompts the user to enter new person information (e.g. name, contact number, address etc.) and then displays the completed person object to the user once completed.

The 'ExistingProjects.java' contains various methods which pertain to user options for existing projects. It has a FindProject() method which, when accessed, will search through the 'CurrentProjects.txt' file to locate a project by name or number. It also contains methods which allow the user to view all existing projects, view only incomplete projects, and to view only overdue projects, if they wish to do so. Another method in this class allows the user to update project information, and then re-writes the updated information to the external text file. The FinaliseProject() method allows a user to mark a project as 'finalised', create an invoice for the customer and thereafter store the completed project in another external text file called 'CompletedProjects.txt'.

The 'Menu.java' class file is where the main program is run from. When initiated, it displays a clear menu to the user, with options to view existing files, add a new file, update existing project info, view specific projects, or to find a specific project. Depending on the user choice, methods from the other previously mentioned classes above will be called on to perform the user's desired action. All outputted information is displayed to the user in a clear, easy-to-read format (e.g. new projects, person details etc.). The user is returned to the main menu after each option, until they choose the last numbered option to 'exit' the program.
