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

```yml
Next create a user for your Ubuntu terminal, the official Jaseci docs reference these docs: 
```

[Microsoft Docs for WSL setup](https://learn.microsoft.com/en-us/windows/wsl/setup/environment#set-up-your-linux-username-and-password)

- But if you happen to miss that step no worries! 
- You need to create a user so you are not using root in Ubuntu (very important step, don't feel bad I missed this step too, lol)!
  - If you get this `WARNING` message when installing using pip 

```bash
WARNING: Running pip as the 'root' user can result in broken permissions and conflicting behaviour with the system package manager. It is recommended to use a virtual environment instead: https://pip.pypa.io/warnings/venv
```

- This means you are using root, enter this command,

```bash
sudo adduser your-username-here
```

- It will prompt you to enter a password, and you will not be able to see the password as you enter it, but it is there!
- Once you have created your new user home, you can login using the `login` command,

```bash
login your-username-here
```

- if you need to move files from your Ubuntu root, it's no big deal, just run these commands in Ubuntu root for each folder that you need to move to your new user home,

```bash
root@YourComputerName:~# mv -v ~/your-project-folder-name-here/ /home/your-username-here/your-project-folder-name-here/
```

- You should get a return like this,

```bash
renamed '/root/your-project-folder-name-here/' -> '/home/your-username-here/your-project-folder-name-here/'
```

- You can check to see if it still listed in your root with this command,

```bash
root@YourComputerName:~# ls
your-project-folder-name-will-no-longer-be-here
```

- After moving this folder into your new user home directory, you should change ownership like this,

```bash
root@YourComputerName:~# chown -R your-username-here:your-username-here /home/your-username-here/your-project-folder-name-here
```

```yml
Create new project directory in Ubuntu:
```

- Create front end using a front-end frame work of your choice, I will be using Angular 15, but Next 13 would be fine too,
- In the root of Ubuntu run this command,


```bash
npm install -g @angular/cli
```

- After that login to your user home, it should look something like this

```bash
your-username-here@YourComputerName:~$
```

- Create a new project by running `ng new your-new-project-name-here`

```bash
your-username-here@YourComputerName:~$ ng new your-new-project-name-here
```

## Open a new VS Code window from task bar or Start menu, connect to WSL using Distro,

![Screenshot 2023-05-02 174818](https://user-images.githubusercontent.com/104662990/235808679-d7010b42-89e9-4275-8f6d-3db0887f7f72.png)

- Open the new project folder from here,

![Screenshot 2023-05-02 174524](https://user-images.githubusercontent.com/104662990/235808394-2f194548-db8b-4430-9ffe-2feac70c8a8a.png)

- Open a new terminal in VS Code and login to your user home, and `cd` into the project directory, 
- Create an virtual enviroment `.venv` with `virtualenv venv`

```bash
virtualenv venv
```

- Next rename the folder to `.venv` and activate it with `source .venv/bin/activate`,

```bash
source .venv/bin/activate
```

- Continue to install all required tools and dependencies,

```bash
yarn
```

## TODO - Work In Progress

- Create desired folder structure, according to your needs,

- Create Jac graphs, walkers, train_files, etc. according to your needs,

- Great job! 

- Now you have a start to your new Jaseci AI powered project!

- Keep up the good work and continue building your project from here!

- If you need help with getting your Jaseci project started, please join the Discord of fellow Jaseci Ninja programmers, I'm sure someone will be more than happy to help!








