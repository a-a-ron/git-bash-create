# Creating a New GitHub Repository
After listening to a RubyRouges episode about sharpening our tools by making our lives easier with scripts and git shortcuts, i've been inspired to perform GitHub requests through the command line using bash functions. This bash function provides the ability to create a new GitHub repo by calling the bash function in .bash_profile. 

## Getting Started

Copy this function into your ~/.bash_profile, open a new terminal window or source ~/.bash_profile to refresh the opened terminal window, and the function will be loaded up and ready for use.

Replace the "USERNAME" with your GitHub username and the "MY_PERSONAL_ACCESS_TOKEN" with your access token generated from GitHub.com. You can create an access token in your user's `Settings > Personal access tokens`

## Features of the Bash Function

This function allows you to create a repo with a description to GitHub by simply calling the bash function and answering the prompt questions. The function then creates the repo and pushes up any local repo to GitHub with the same name of the created repo. 

## Considerations

As is, this function is used to create a new local repo and push it to GitHub. This will automatically run 'git init' on the local repo and create a new README.md file. If you  want to run 'git init' manually and add files before running this function to push to GitHub, you will need to omit 'auto_init' from the request body. Otherwise, this function will fail. 



