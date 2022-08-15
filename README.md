# Customize PS1

Provide bash file to custom PS1.

## Prerequisite

To have the proper PS1 you need to have the project `git-aware-prompt`

```bash
cd $HOME
mkdir .bash
cd .bash
git clone https://github.com/jimeh/git-aware-prompt.git
```

## How to use

1. Get the file `.bash_customize_ps1` on your host and source it in your bashrc file:

  ```bash
  source $HOME/.bash_customize_ps1
  ```

2. Call the function `custom_ps1` with corresponding colors

  ```bash
  PRIMARY_COLOR=$COLOR_BLUE
  WORKSPACE_COLOR=$COLOR_GREEN
  TIME_COLOR=$COLOR_YELLOW
  SEPARATOR_COLOR="$COLOR_PURPLE"
  
  custom_ps1 $PRIMARY_COLOR $WORKSPACE_COLOR $TIME_COLOR $SEPARATOR_COLOR
  ```

## List of color

A list of colors has been exported from the providing file and each have named **COLOR_XXXX**

## Example

![Example ps1 colorized](img/example-ps1-colorized.png)
