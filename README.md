# How to use git-crypt 

- This is a repo for testing git-crypt. I will also make some usage notes here.
### Install git-crypt
### Install gpg (if you need to collaborate with others)

### some useful command line
- list your gpg key id and other infomation : <br> ```gpg --list-keys```
- Add user to git-crypt so people can collaborate with other collaborators : <br> ```git-crypt add-gpg-user USER-ID``` (example: EEIHFOQ92RU0Q94294QIEFO9UQER0)
- Lock your secrets: ```git-crypt lock```
- Unlock your secrets: ```git-crypt unlock ```(if you use gpg key) or ```git-crypt unlock path/key```(if you export your git-crypt somewhere)

## Resources
* [Ubuntu git-crypt command line]([https://www.youtube.com/watch?v=Ej3ZVxljJfo](https://manpages.ubuntu.com/manpages/jammy/man1/git-crypt.1.html#:~:text=To%20share%20the%20repository%20with,encrypted%20key%20file%20in%20the%20.)https://manpages.ubuntu.com/manpages/jammy/man1/git-crypt.1.html#:~:text=To%20share%20the%20repository%20with,encrypted%20key%20file%20in%20the%20.)
* [git-crypt github](https://github.com/AGWA/git-crypt)
* [How to Manage Your Secrets with git-crypt](https://dev.to/heroku/how-to-manage-your-secrets-with-git-crypt-56ih)
* [Using git-crypt in Azure Devops](https://stackoverflow.com/questions/66590438/using-git-crypt-in-azure-devops)
