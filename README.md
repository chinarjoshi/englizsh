# englizsh
A zsh plugin that defines 4 keybindings to intuitively interface with any command-line GPT program. The idea is to 
toggle the contents of the shell buffer between natural language and shell command using GPT as the translator.

## Usage

* Control + Space: Toggles the buffer between English and command. It assumes the buffer contains a command if the first word is a valid command according to `command -v`.
* Alt + Space: Translates the buffer from English to command. Useful when the first word is a command, for instance when you're typing a command but forgot some flags.
* Enter: Executes commands normally, but if command is not found and there appears to be English in the buffer, then it is translated to shell before executing.
* Control + Enter: Translates the buffer from English to command and executes it. Useful when you know you're executing English but it doesn't appear like it.

## Configuration

Englizsh can be configured through environmental variables before the script is sourced:

* 

## Installation

### Manually

Downloading/updating the script:

`curl https://raw.githubusercontent.com/chinarjoshi/englizsh/main/englizsh > ~/.englizsh`
