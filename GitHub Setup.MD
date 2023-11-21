# MeshONE-T

## Directions

* To view templates for various site tiers go [here](https://github.com/Sev1Tech/MeshONE-T/tree/master/documentation/ansible/roles/create-cable-table/templates).
* To view items/cable runs for sites go [here](https://github.com/Sev1Tech/MeshONE-T/tree/master/documentation/ansible/configs).

## **Setup Notes**

### For most of the tasks, you will need your workstation to be setup with the programs listed below in addition to having the [GitHub repository](https://github.com/Sev1Tech/MeshONE-T/blob/master/documentation/Instructionals/GitHubLocalSetup.MD) setup locally

> Programs needed:
>
> * Windows Subsystem for Linux ([WSL](https://learn.microsoft.com/en-us/windows/wsl/install)) or a Linux OS
> * [Python](https://www.python.org/)
> * [Ansible](https://www.ansible.com/)
> * [Visual Studio Code](https://code.visualstudio.com/) (optional)
>
> _Note_ You can edit files with the online VSC Editor which can be accessed by pressing the `.` button here.  
___

* To install the Windows Subsystem for Linux or [WSL](https://learn.microsoft.com/en-us/windows/wsl/install) open [Powershell](https://www.howtogeek.com/662611/9-ways-to-open-powershell-in-windows-10/) then use the command `wsl --install` and press enter.  
  * From within Powershell you will now be able to access WSL by simply typing the command `wsl`.  
  * You will be able to return to the Windows CLI by typing `exit`.  

* Python 3 should be pre-installed within the WSL. You can check with command `python3 -V`.
  * If you need to install Python 3, use [these instructions](https://www.geeksforgeeks.org/how-to-install-python-on-linux/).

* Check to see if [Ansible](https://www.ansible.com/) is installed with command `ansible --version`.  If not already installed, you will need to install Ansible.  
  * This can be performed via Linux CLI ([WSL](https://learn.microsoft.com/en-us/windows/wsl/install)) with command `sudo apt install ansible`.
  * _Note_ -  [Ansible does not run natively on WIndows](https://docs.ansible.com/ansible/latest/installation_guide/intro_installation.html).  

___

> _Note_ that instead of using PowerShell, you can accomplish all of these steps from within [Visual Studio Code](https://code.visualstudio.com/) or another text editor/IDE.


# GitHub Local Setup

## Credentials

> If you are reading this, then it is assumed that you have a GitHub account.  However, you will need to generate a personal access token which you will use as a password for pulling and pushing the repository remotely.  

 To do this login to GitHub then:

* On the top right corner of the screen click on your profile icon.  When the drop-down appears click on **Settings**.
![image info | ](./images/GitHubSettingsDropdown.png)

* Once on your profile page, there is a list of options of the left side.  Click **Developer Settings** at the bottom.  
![image info | ](./images/GitHubDeveloperSettings.png)
* Now click **Personal access tokens**, on the drop-down that appears click **Tokens (classic)**.  
![image info | ](./images/GitHubPersonalAccessTokens.png)
* Click the button, **Generate new token**, in the drop-down select **Generate new token (classic)**.  
![image info | ](./images/GitHubGenerateNewToken.png)
* Here input a name in the **Note** field and select an expiration timeframe.
* Under **Select scopes** click the parent box for **repo** (this  will auto-check child boxes) then scroll to the bottom and click the **Generate token** button.  
* The new screen that appears will display your personal access token, be sure to copy it.  

___
> Below is a brief rundown of what you need to get started. If you want more thorough or diverse instructions, check out [GIt Guides](https://github.com/git-guides) or [Git Docs](https://git-scm.com/docs).  

## **Git commands**

> _These commands would be performed in the command line (CLI), text editor or IDE where you can access the terminal to manipulate both your local and the main repository._
>
> Follow the below instructions from top to bottom.  

```git
git config --global user.name "GitHub-username"
```

```git
git config --global user.email "GitHub-email"
```

* Setup your account locally by inputing the email and username GitHub account within quotations.

___

```git
git clone https://github.com/your_repo
```

* This command will clone the MeshONE-T repository for you to use locally.  
* This should only need to be done once.  

___
> After you have made your changes to the files within your local repository, check the status using the following command.

```git
git status
```

* This shows the status of the commit, displaying everything that you have changed.
  * Red = not ready to be sent.
  * Green = ready to be sent.

![image info](./images/red.png)
___

```git
git add -A
```

* This adds all the untracked files to the commit.  This should catch all the "red" files/changes.

  * _Note -  Be sure to save the files before adding them to the commit._

___

> At this point check the status (`git status`) again to ensure that all files are now showing green.  
>
>![image info](./images/green.png)
>
> If they are, then continue on with the commit command below.  

```git
git commit -m "commit message"  
```

* Commits / stages for push to origin repo.  Within the quotations you can leave a message stating what you changed.  

___

```git
git push -u origin master       
```

* Pushes the commit to the origin repository.  

> Here you will be asked to input your GitHub username and password, the password will be your personal access token.  
___

```git
git pull
```

* This pulls the most recent repository from main to your local machine.  You should do this every time to refresh your local repository before you start working.  

___

## **Key Terms**

* IDE - Integrated development Environment such as [PyCharm](https://www.jetbrains.com/pycharm/).  
* Text editor - such as [Visual Studio Code](https://code.visualstudio.com/).  
* CLI - Command line interface or terminal such as [WSL](https://learn.microsoft.com/en-us/windows/wsl/install) and [Powershell](https://www.howtogeek.com/662611/9-ways-to-open-powershell-in-windows-10/).  
