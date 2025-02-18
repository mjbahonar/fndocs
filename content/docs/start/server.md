---
title: Running The Server
weight: 2
---

## Connect to server

After renting a server, we need to connect using the IP address in PuTTY. Configure PuTTY as explained in the previous documentation. Ensure you add your private key to PuTTY and set up the **IP address** and **port** as shown in the following image:


![alt text](putty.png)


## Runnung the code
Now we are ready to run the code. First, we should update all packages. Unfortunately, in Vast.ai servers, `pip` is not installed by default, so we need to install it manually:


```
sudo apt update
apt install python3-pip
```
To ensure both Python and `pip` are installed, check their versions:
```
python3 --version
pip3 --version
```


## Creating new enviroment
To avoid losing progress when disconnecting PuTTY, it's recommended to create a session using `tmux`:

    tmux

After starting `tmux`, you can check the list of created sessions


    tmux ls

This will display a list of active sessions along with their IDs. Assume your session ID is `0`. To reattach to it, use:

    tmux attach-session -t 0

Now, you have entered the session, and even if you close PuTTY, you can reconnect later without losing progress.