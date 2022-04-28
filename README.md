# Simple-Fetch
Neofetch is too much for my underpowered pc so I created a lighter alternative as a fun project and improve my skills.

Setup:

Add the following lines to your .bashrc:
```Bash
let RAND=$RANDOM

let RANDCOLOUR=31+$RAND%6

export COLOUR="\\e[1;${RANDCOLOUR}m"

PS1="\e[1;100m${COLOUR}[kali@\w] \$ \e[m"
```

These choose a random colour each time a terminal is started, and makes the prompt, title, and info that colour.

Then add `./startup` to your `.bashrc` below, so the program runs whenever the terminal starts. You might also need to make the files executable, but idk.

Here's a screenshot of what it looks like:
![Screenshot 2022-01-31 14 25 52](https://user-images.githubusercontent.com/84800702/151859281-86a0c8e9-4660-413f-9000-881745279fa4.png)
