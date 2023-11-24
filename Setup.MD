# **Setup Notes**

## For most of the tasks, you will need your workstation to be setup with the programs listed below in addition to having the [GitHub repository](https://github.com/TheWillN/Enlightenment) setup locally

> Programs needed:
>
> * Windows Subsystem for Linux ([WSL](https://learn.microsoft.com/en-us/windows/wsl/install)) or a Linux OS
> * [Python](https://www.python.org/)
> * [Ansible](https://www.ansible.com/)
> * [Visual Studio Code](https://code.visualstudio.com/)
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

> _Note_ that instead of using PowerShell, you can accomplish all of these steps from within [Visual Studio Code](https://code.visualstudio.com/) by to _Terminal_ then selecting _New Terminal_.  
> Alternatively you can use the keyboard shortcut ```Ctrl Shift ` ```
