# bash-insulter
Randomly insults the user when typing wrong command.

Change insults as needed :)

Additional insults from sudo are stored in $HOME/.insults

# Installation

    git clone https://github.com/hkbakke/bash-insulter.git bash-insulter
    sudo cp bash-insulter/src/bash.command-not-found /etc/
    cp bash-insulter/src/.insults ~/

Then source the file automatically for new logins by adding the following to `/etc/bash.bashrc`:
```
if [ -f /etc/bash.command-not-found ]; then
    . /etc/bash.command-not-found
fi
```
Login again and type some invalid commands for the effects to be visible.
