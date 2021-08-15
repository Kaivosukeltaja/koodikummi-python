# koodikummi-python

Simple repository to demonstrate using VSCode devcontainers to speed up development environment setup

## Why devcontainers?

When a developer starts working on a project, there can be a lot of setup needed. You need to install build tools, runtime environments, libraries, tweak configuration files, and so on. On complex projects it can take days just to get the project to build and run on your machine.

[Devcontainers](https://code.visualstudio.com/docs/remote/containers) are a great solution to this. It is a way to run your development environment inside a Docker container, isolating all the dependencies from your own machine. This allows developers to just clone your repository, open it up in VSCode and have an immediately functional development environment.

## Requirements

- Linux, Mac or Windows (requires [WSL2](https://docs.microsoft.com/en-us/windows/wsl/install-win10))
- [Visual Studio Code](https://code.visualstudio.com/) (aka VSCode)
- [Docker](https://www.docker.com/)
- If on Windows, configure Docker to use the WSL2 backend and make sure your default WSL uses version 2 (see instructions in first step above)
- VSCode extension: [Remote - Containers](https://aka.ms/vscode-remote/download/containers)

## Instructions

1. Make sure you have everything installed from the list above!
2. Clone this repository to your own machine: `git clone git@github.com:Kaivosukeltaja/koodikummi-python.git`
3. Open the directory in VSCode: `cd koodikummit-python; code .`
4. VSCode should notice the presence of the devcontainer configuration file and ask if you want to `Reopen in Container`. Do it.
5. Wait a while as your environment is built.
6. If the lower left corner of your VSCode says "Dev Container: Python" in green, you're now running in a container.
7. Create a new terminal - note that it will be launched inside your devcontainer.
8. Write the command `python hello.py` to verify you have a working installation.
