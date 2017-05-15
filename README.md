## Terminal Multiplexer Setup

This is my tmux setup with customizations that I use for development. Steps to get this setup are as follows:

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

3. Copy all of the *.yml files to the ~/.tmuxinator directory

~~~
   cp *.yml ~/.tmuxinator
~~~

4. Copy tmuxinator.bash to the ~/.tmuxinator directory

~~~
   cp tmuxinator.bash ~/.tmuxinator
~~~

5. Append the following line to your .bashrc file

~~~
   source ~/.tmuxinator/tmuxinator.bash
~~~

