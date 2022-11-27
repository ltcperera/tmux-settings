## Terminal Multiplexer Setup

This is my tmux setup with customizations that I use for development at the terminal. Steps to get this setup are as follows:

1. Create the configuration directory for Tmux:
    
    ~~~
    mkdir $HOME/.config/tmux
    ~~~
    
2. Setup Tmux Plugin Manager

    ~~~
    chdir $HOME/.config/tmux
    git clone https://github.com/tmux-plugins/tpm plugins/tpm
    ~~~

3. Logout and back in and start tmux.

4. Hit the ` + I key to install the plugins.

