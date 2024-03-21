# secure file or your secret in repo

- This is a repo for testing git-crypt and some other way to secure files in repo. I will also make some usage notes here.

## Use git-crypt
### 1) Install git-crypt
```brew install git-crypt```

### 2) Install gpg (if you need to collaborate with others)
```brew install gpg```

### 3) some useful command line
- list your gpg key id and other infomation : <br> ```gpg --list-keys```
- Add user to git-crypt so people can collaborate with other collaborators : <br> ```git-crypt add-gpg-user USER-ID``` (example: EEIHFOQ92RU0Q94294QIEFO9UQER0)
- Lock your secrets:<br> ```git-crypt lock```
- Unlock your secrets:<br> ```git-crypt unlock ```(if you use gpg key) or ```git-crypt unlock path/key```(if you export your git-crypt somewhere)
## Resources - git-crypt
* [Ubuntu git-crypt command line](https://manpages.ubuntu.com/manpages/jammy/man1/git-crypt.1.html#:~:text=To%20share%20the%20repository%20with,encrypted%20key%20file%20in%20the%20.)
* [git-crypt github](https://github.com/AGWA/git-crypt)
* [How to Manage Your Secrets with git-crypt](https://dev.to/heroku/how-to-manage-your-secrets-with-git-crypt-56ih)
* [Using git-crypt in Azure Devops](https://stackoverflow.com/questions/66590438/using-git-crypt-in-azure-devops)

## Use secure file in Azure Devops
Secure files give you a way to store files that you can share across pipelines. Use the secure files library to store files such as:
<br>
- signing certificates
- Apple Provisioning Profiles
- Android Keystore files
- SSH keys
  
## Resources - secure file
* [Use secure files](https://learn.microsoft.com/en-us/azure/devops/pipelines/library/secure-files?view=azure-devops)
  
