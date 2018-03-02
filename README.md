# BasicLinuxCommands
This is a list of useful linux commands you should know.

1. sudo

In any linux system, there needs to be an "administrator" that has access to everything and can do anything.  The username for this all-knowing-all-powerful user is "root" and this user can do <i>anything</i> (including completely destroying your system!).  

Obviously, we don't want to give a regular user "root" privileges.  However, sometimes a regular user needs to do some of the tasks that "root" or the superuser does. To do this, we use sudo to allow other users to do some of the things that root can.  Sudo stands for <b>SuperUserDo</b> and is the most important command Linux newbies will use. Every single command that needs root's permission, needs to be preceded by the sudo command.

2. ls (list)

With the list command, the terminal will show you all the files and folders of the directory that you're working in. There is one useful parameter that go with ls.  ls -l will give a "long" list which means that listed files and directories will have additional information including read/write permissions, size, date modified etc.

3. cd

Changing directory (cd) is the main command that always be in use in terminal. It's one of the most Linux basic commands. Using this is easy. Just type the name of the folder you want to go in from your current directory. If you want to go up just do it by giving double dots (..) as the parameter.

Let's say I'm in /home directory and I want to move in usr directory which is always in the /home. Here is how I can use cd commands -

> /home$ cd usr

> /home/usr$

4. mkdir

Just changing directory is still incomplete. Sometimes you want to create a new folder or subfolder. You can use mkdir command to do that. Just give your folder name after mkdir command in your terminal.

> ~$ mkdir folderName

5. cp

copy-and-paste is the important task we need to do to organize our files. Using cp will help you to copy-and-paste the file from terminal. First, you determine the file you want to copy and type the destination location to paste the file.

> $ cp source_file destination_folder

Note: If you're copying files into the directory that requires root permission for any new file, then you'll need to use sudo command.

6. rm

rm is a command to remove your file or even your directory. You can use -f if the file need root permission to be removed. And also you can use -r to do recursive removal to remove your folder.

> $ rm myfile.txt

> $ rm -r directory/

7. apt-get

This command differs distro-by-distro. In Debian based Linux distributions, to install, remove and upgrade any package we have Advanced Packaging Tool (APT) package manager. The apt-get command will help you installing the software you need to run in your Linux. It is a powerful command-line tool which can perform installation, upgrade, and even removing your software.

> $ sudo apt-get update

8. whereis

You want to execute a command but you don't know where it is located.  Use whereis to find the location.

> $ whereis hdfs

hdfs: /usr/local/hadoop/bin/hdfs /usr/local/hadoop/bin/hdfs.cmd

9. cat

As a user, you often need to view some of text or code from your script. Again, one of the Linux basic commands is cat command. It will show you the text inside your file.

> $ cat alice.txt 

10. gedit

There are many text editors available on a linux system.  Most users pick their favourite and stick with it.  gedit is a very user friendly editor that can be used to edit many types of text based files (we used it to edit the .xml files).

> gedit alice.txt

Remember that with any text editor, if the file does not exist, the editor will create it for you.  So if you are looking to edit a file that you expect to have some text in it but then opens as empty, this usually means that you made a subtle spelling mistake in it (and so created a new file with no text inside).

11. reboot

Often you would like to reboot your system to have changes you wrote take effect.  Make sure to precede this with sudo.

> $ sudo reboot
