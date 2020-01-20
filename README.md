# Instructions

The PsynaryExtractor is command line program to be run from the command line or terminal.

Download all of the files here in the GitHub repository related to your operating system.

## Mac Setup

If you are using a Mac, you can just download the files in osx.10.14-x64.  Copy them to someplace on your PC.  Keep them all in the same directory. (Yes, there are a lot of files, I'm not currently sure if they all are needed, so best to begin with them all)

The program requires .NET Core framework.  Supposedly, these files are already installed on most modern PCs and even Macs.  However, if not, you can download installers for the framework from here: https://dotnet.microsoft.com/download/dotnet-core/3.0

To test if you have .NET support, try running the following command: in terminal:
dotnet

If it is currently installed, you will see a help screen.  Otherwise, you may need to install it from the link above.

## Running the application

To run the application, do the following:

1. Open a command line window (cmd.exe) or Terminal on a Mac.
2. Go to the directory where you stored the files by typing something like:
cd /path/to/files
Replacing '/path/to/files' with the actual path to the files.
3. Run the program like so:

PsynaryExtractor <hostname> <username> <password> <database name>

The program requires a few parameters from you to run.  These are:

1. The location (server) of the database.  This is most likely 'localhost' (which is your pc).  You might also try '127.0.0.1'.

2. The user name of the database.  If you created the database on your pc, you gave it a username.  This will be same.

3. Password - same as above (2).

4. Finally, the name of the database. Probably 'psynary'.  But if you created one locally, this will be whatever you used to name the local database.

So, for me, I run this like:

PsynaryExporter.exe localhost james MyPassword psynary

For the mac, it would be something like:

./PsynaryExporter localhost james MyPassword psynary

You will be prompted with a serious of questions.  Each question has a default answer that can be used by simply pressing enter.

On a hefty database, the program can take some time to run.

When the program is complete, you will have a CSV file with a name of the date and starting time.
