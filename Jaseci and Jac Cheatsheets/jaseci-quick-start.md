# [Jaseci](https://www.jaseci.org/) Quick Start for Windows - Not Official Docs

- [Official Jaseci Installation Guide Found Here](https://docs.jaseci.org/docs/docs/getting_started/installation)

To run commands for Jaseci we need a terminal that accepts bash arguments. 
- The official Jaseci docs recommend using the Ubuntu terminal that comes as the default with WSL.
- To install WSL, first check if WSL is installed by running the following the Windows powershell terminal,

```bash
wsl -l -v
```

```bash
wsl --install
```

Next create a user for your Ubuntu terminal (this is not in the official Jaseci docs but they do reference these [Microsoft Docs](https://learn.microsoft.com/en-us/windows/wsl/setup/environment#set-up-your-linux-username-and-password).

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








