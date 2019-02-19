###how to use github
* * *

>#1. Installing and using Git and GitHub on Linux
* * *

You have to install git file. if you don't have git file in you server, you use this command:
	<sudo apt-get install git>

>#2. Configuring GitHub
* * *

The next step to do is to set up the configuration details of GitHub user. To do this use the following two commands by replacing "user_name" with your GitHub username and replacing "email_id" with your email_id you used to create your GitHub account.
Use the following two commands:
	<git config --global user.name "user_name">
	<git config --global user.email "email_id">

>#3 Creating a local repository
* * *

Create a folder on your system. This will serve as a local repositroy which will later be pushed onto the GitHub website. Use the following command:
	<git init repository_name>
If the repository is created successfully, then you will get the following line:
	<Initialized empty Git repository in /home/user_name/repository_name/.git/>
This line may vary depending on your system. So here, repository_name is the folder that is created and "init" makes the folder a GitHub repository. Change the directory to this newly created folder:
	<cd repository_name>

>#4 Creating a README file to describe the repository
* * *

Nowcreate a README file and enter some text like "anything". The README file is generally used to describe what the repository contains or what the project is all about.

>#5 Adding repository files to and index
* * *

This is an important step. Here we add all things that need to be pushed onto the website into an index. These things might be the text files or programs that you might add for the first time into the repository or it could be adding a file that already that you might add for the first time into the repository or it could be adding a file that already exist but with some changes(a newer version/updated version).

Here we already have the README file. So, let's create another file which contains a simple Python program and call it hello.py. The contents of it will be:
'''python
hi="hello"
print(hi)
'''
So, now that we have 2 files that are 'README' and 'hello.py'
add it to the index by using the following 2 commands:
	<git add README>
	<git add hello.py>

>#6 committing changes made to the index
* * *

Once all the files are added, we can commit it. This means that we have finalized what additions and/or changes have to be made and they are now ready to be upladed to our repository. Use the command:
	<git commit -m "some_message">
"some_message" in the above command can be any simple message like "my first commit" or edit in readme", etc.

>#7 Creating a repository on GitHub
* * *

Create a repository on GitHub. Notice that the name of the repository should be the same as the repository's on local system. In this case, it will be "repository_name".
Once this is created, we can push the contents of the local repository onto the GitHub repository in your profile. Connect to the repository on GitHub using the command:
Important Note : Make sure your replace 'user_name' and 'repository_name' in the path with your GitHub username and folder before running the command!
	<git remote add origin https://github.com/user_name/repository_name.git>

>#8 Pushing files in local repository to GitHub repository
* * *

The final step is to push the local repository contents into the remote host repository(GitHub), by using the command:
	<git push origin master>
Enter the login credentials [user_name nad password]
