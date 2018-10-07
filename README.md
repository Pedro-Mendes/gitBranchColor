# Setting up colors for the prompt

## .bashPedro-Mendes
* This code snipped should be pasted at the end of the ~/.bashrc file:
> code ~/.bashrc


* Note that we have several information which we can place it the shell prompt:

    Syntax | Meaning
    ------------ | -------------
    \a | an ASCII bell character (07)
     \d | the date in “Weekday Month Date” format (e.g., “Tue May 26”)
     \D{format} |	the format is passed to strftime(3) and the result is inserted into the prompt string; an empty format results in a locale-specific time representation. The braces are required
     \e | an ASCII escape character (033)
     \h | the hostname up to the first ‘.’
     \H | the hostname
     \j | the number of jobs currently managed by the shell
     \l | the basename of the shellâ€™s terminal device name
     \n | newline
     \r | carriage return
     \s | the name of the shell, the basename of $0 (the portion following the final slash)
     \t | the current time in 24-hour HH:MM:SS format
     \T | the current time in 12-hour HH:MM:SS format
     \@ | the current time in 12-hour am/pm format
     \A | the current time in 24-hour HH:MM format
     \u | the username of the current user
     \v | the version of bash (e.g., 2.00)
     \V | the release of bash, version + patch level (e.g., 2.00.0)
     \w | the current working directory, with $HOME abbreviated with a tilde
     \W | the basename of the current working directory, with $HOME abbreviated with a tilde
     \! | the history number of this command
     \# | the command number of this command
     \$ | if the effective UID is 0, a #, otherwise a $
     \nnn | the character corresponding to the octal number nnn
     \ \ | a backslash
     \[ | begin a sequence of non-printing characters, which could be used to embed a terminal control sequence into the prompt
     \] | end a sequence of non-printing characters

In this code snippet we have only the user, path and current branch, but you can configure it anyway you want. You'll just need to add the syntax desired and set the color:
> $COLOR_GREEN

> $COLOR_RED

And so on...
But if you would like to choose your own color, you can choose between the following by using declaring COLOR_YOURCOLOR="\e[38;5;<COLOR_NUMBER>":

![Color code](/images/256_colors_fg.png)

#### In the provided snippet the color of the current branches changes depending on the status of the branch:

* Nothing to commit(green)
    * ![Green](/images/green.png)

* Files have been modified(red)
    * ![Red](/images/red.png)

* You have commited but not pushed:
    * ![Yellow](/images/yellow.png)

## Feel free to contribute! 

##### sources: 
* https://misc.flogisoft.com/bash/tip_colors_and_formatting     
* https://unix.stackexchange.com/questions/124407/what-color-codes-can-i-use-in-my-ps1-prompt
* https://www.cyberciti.biz/tips/howto-linux-unix-bash-shell-setup-prompt.html