# Additional

## Azure Cloud Shell

Azure Cloud Shell is a browser-accessible command-line experience for managing Azure resources. Rather than having to configure an Azure CLI or PowerShell session from your workstation, you can access Cloud Shell on any standard, compliant browser.

- Open a secure command-line session from any browser-based device.
- Interact with Azure resources without the need to install plug-ins or add-ons to your device.
- Persist files between sessions for later use.
U- se either Bash or PowerShell, whichever you prefer, to manage Azure resources.
- Edit files (such as scripts) via the Cloud Shell editor.

Azure Cloud Shell provides access to CloudDrive natively from inside the Cloud Shell session.
Saving your script directly on the CloudDrive is the most appropriate method.
You open Azure Cloud Shell once logged into your Azure subscription with a web browser.

## BASH

### Commands

ps -  command lists processes currently running on the system.
cat - short for concatenate. It displays the contents of a file or files in the terminal without having to open the file for editing. It is convenient for viewing the contents of small text files, joining together and displaying multiple files' contents, or piping the output into other commands for further processing.
cat [options] [file path]

## POWER SHELL

Command-line shell and a scripting language all in one. It was designed as a task engine that uses cmdlets to wrap tasks that people need to do. In PowerShell, you can run commands on local or remote machines. You can do tasks like managing users and automating workflows. You can use it to address various tasks, such as managing cloud resources and continuous integration and continuous delivery (CI/CD).

### Advantages

- Interacting with a console is often faster than using a graphical interface.
- Ideal for task automation for continuous-integration pipelines.
- Store commands and scripts in a text file and use a source-control system.

### Commands PS

- GetCommand
- Run the flag -Noun. Specify File to find anything related to files.
-- Get-Command -Noun File*
- Get-Command. Specify the flags -Verb and -Noun.
-- Get-Command -Verb Get -Noun File*