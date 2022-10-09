## Terminal Multiplexer Setup

This is my tmux setup with customizations that I use for development at the terminal. Steps to get this setup are as follows:

1. Setup tmux and tmuxinator on your Linux distribution:

~~~
   sudo apt-get update
   sudo apt-get install tmux
   sudo apt-get install tmuxinator
~~~

2. Copy tmux.conf to the default tmux configuration file location as follows:

~~~
   cp tmux.conf ~/.tmux.conf
~~~

3. Create the ~/.tmuxinator directory if it does not exist:

~~~
   mkdir ~/.tmuxinator
~~~

4. Copy all of the *.yml files to the ~/.tmuxinator directory:

~~~
   cp *.yml ~/.tmuxinator
~~~

5. Copy tmuxinator.bash to the ~/.tmuxinator directory

~~~
   cp tmuxinator.bash ~/.tmuxinator
~~~

6. Assuming you are using BASH as your shell, append the following line to your .bashrc file:

~~~
   source ~/.tmuxinator/tmuxinator.bash
~~~

## Usage

In order to use the settings above, start your terminal session and isue the mux (short for tmuxinator) followed by the yml file indicating the profile you wish to use. For instance, for C/C++ development, I use the following:

~~~
   mux c
~~~

For Android, I use the following:

~~~
   mux android
~~~

## Quick Keyboard Shortcuts

The following are the keyboard shortcuts defined in .tmux.conf that was setup above:

` + Arrow - Switch window pane
` + q     - Display window numbers
