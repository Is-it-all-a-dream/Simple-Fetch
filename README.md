# Simple-Fetch
Neofetch is too much for my underpowered pc so I created a lighter alternative as a fun project and improve my skills.

Setup:

Add the following lines to your .bashrc:

let RAND=$RANDOM

let RANDCOLOUR=31+$RAND%6

export COLOUR="\\e[1;${RANDCOLOUR}m"

PS1="\e[1;100m${COLOUR}[kali@\w] \$ \e[m"

These choose a random colour each time a terminal is started, and makes the prompt, title, and info that colour.

Then add "./startup" to your .bashrc below, so the program runs whenever the terminal starts. You might also need to make the files executable, but idk.
