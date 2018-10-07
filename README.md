# Setting up colors for the prompt

## .bashPedro-Mendes
* This code snipped should be pasted inside the ~/.bashrc file:
> code ~/.bashrc
* You can set which colors you like by changing the "COLOR_ID" in the code:
> echo -e $COLOR_GREEN

> echo -e $COLOR_RED

And so on...
But if you would like to choose your own, you can choose between the following by using declaring COLOR_YOURCOLOR="\e[38;5;<COLOR_NUMBER>":

![Color code](/256_colors_fg.png)

##### sources: https://misc.flogisoft.com/bash/tip_colors_and_formatting        https://unix.stackexchange.com/questions/124407/what-color-codes-can-i-use-in-my-ps1-prompt