# [Jaseci](https://www.jaseci.org/) Quick Start for WSL using Ubuntu - Not Official Docs

- *These are only my notes, not official docs here, official docs are found in the link provided above*

- and [Official Jaseci Installation Guide Found Here](https://docs.jaseci.org/docs/docs/getting_started/installation)

<p align="left"> 
<img src="https://komarev.com/ghpvc/?username=jaseci-quick-start&label=Profile%20views&color=f79952&style=flat" alt="jaseci-quick-start" /> 
</p>

To run commands for Jaseci we need a terminal that accepts bash arguments. 
- The official Jaseci docs recommend using the Ubuntu terminal that comes as the default with WSL.
- To install WSL, first check if WSL is installed by running the following command in Windows powershell terminal,

```bash
wsl -l -v
```

- If nothing is returned like this,

```powershell
  NAME          STATE           VERSION
* kali-linux    Stopped         2
  Ubuntu        Running         2
```

- Run this in Windows powershell terminal to install WSL,

```bash
wsl --install
```

- Next restart your computer and open Ubuntu terminal
- Once opened again, make sure Ubuntu is updated, and feel free to do this regularly,

```bash
sudo apt update && sudo apt upgrade
```

- You need to create a user so you are not using root in Ubuntu (very important step, don't feel bad I missed this step too, lol)!
  - If you get this `WARNING` message when installing using pip 

```bash
WARNING: Running pip as the 'root' user can result in broken permissions and conflicting behaviour with the system package manager. It is recommended to use a virtual environment instead: https://pip.pypa.io/warnings/venv
```

- This means you are using root, and you should consider creating a user in Ubuntu, we can do this by creating a user like this,

```yml
Next create a user for your Ubuntu terminal, the official Jaseci docs reference these docs: 
```

[Microsoft Docs for WSL setup](https://learn.microsoft.com/en-us/windows/wsl/setup/environment#set-up-your-linux-username-and-password)

- But if you happen to miss that step no worries! 
  - If you did not setup up a user that way, you can setup a new user in your Ubuntu terminal,

- Launch Ubuntu terminal, and enter this command,

```bash
sudo adduser your-username-here
```

- It will prompt you to enter a password, and you will not be able to see the password as you enter it, but it is there!
- Once you have created your new user home, you can login using the `login` command,

```bash
login your-username-here
```

## TODO - Work In Progress

```yml
Create directory in Ubuntu:
```

- Create a new folder for your new jaseci project using `mkdir`,
- Use `ls` command for a list of current directories and files in current working directory.

- Use `cd` command to change directory to the new folder you choose to create,
- After that use `code .` to launch VS Code using WSL; Ubuntu while opening the folder you just created.
  - Note I have not found any other way to open both the folder from Ubuntu and WSL:Ubuntu in VS Code, and you have to have them both using Ubuntu. 

- VS Code will automatically launch in a new window, it should look like this, notice in the far left corner in blue it says WSL:Ubuntu, this is what we want!

- VS Code must be using WSL if you are using Windows. 
- You can also see the folder is open from the correct place at the top of VS Code, it needs to be from Ubuntu also.

- Create front end using a front-end frame work of your choice, I will be using Angular 15, but Next 13 would be fine too:

- Continue to install all required tools and dependencies,

- Create desired folder structure, according to your needs,

- Create Jac graphs, walkers, train_files, etc. according to your needs,

- Great job! 

- Now you have a start to your new Jaseci AI powered project!

- Keep up the good work and continue building your project from here!

- If you need help with getting your Jaseci project started, please join the Discord of fellow Jaseci Ninja programmers, I'm sure someone will be more than happy to help!








