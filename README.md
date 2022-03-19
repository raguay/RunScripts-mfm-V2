# Run Scripts Extension for Modal File Manager

This extension for [Modal File Manager](https://github.com/raguay/ModalFileManager) gives the user the ability to create and run scripts. All scripts are kept in the `~/.config/modalfilemanager/scripts/` directory. Upon loading the extension for the first time, this directory is created and some example scripts are copied to it.

To run this extension, you have to have Modal File Manager version 0.1.4 or greater. This is due to additions to the extension API needed for this extension to work.

Before a script is ran, some environment variables are created in the run environment. These are in addition to the environment variables setup in the preferences. These are:

| Environment Variable | Description |
| ---- | -------- |
| CURRENT_DIRECTORY | The current directory for the cursor |
| CURRENT_FILE | The current file name for the cursor |
| LEFT_PANE | The directory of the left file pane |
| LEFT_PANE_SELECTED_FILE | The last highlighted file in the left file pane |
| RIGHT_PANE | The directory of the right file pane |
| RIGHT_PANE_SELECTED_FILE | The last highlighted file in the right file pane |
| FILES_SELECTED | A newline separated list of selected files |

## Commands available in the Command Prompt

The following commands are available to use in the Command Prompt:

| Command | Description |
| --- | ------ |
| Run Script | A list of scripts will be given to chose from. That script will be ran. | 
| Run NPM Script | A list of npm scripts in the current directory will be given to choose from. That script will be ran. |
| Run Mask Script |  A list of mask scripts in the current directory will be given to choose from. That script will be ran. |
| Create Script | The user will be prompted for a new script name. That script will be created, populated with a template, and the user's editor will open the script. |
| Toggle Show Output | Toggles the displaying of the results from running the script. |
| Run Command Line | This will run a command line just like a script. |
| Edit Script | A list of scripts will be given to choose from. That script will be opened in the user's defined editor. |
| Go To Scripts Directory | This will open the current pane in the Modal File Manager to the scripts directory. |
| Install Example Scripts | This will install the example scripts into the scripts folder |
