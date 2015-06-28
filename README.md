# Minecraft Server Setup

## Prerequisites

1. This is written for a server running CentOS 7
2. See #1
3. Basic understanding of Ansible (at least how to create an inventory, run a playbook and pass SSH options)

## Usage

Run:

```
ansible-playbook -i hosts site.yml
```

Where hosts is the name of your inventory file.

This will perform all tasks necessary to get your Minecraft server running!

You can start/stop the server with:

```
sudo systemctl start minecraft-server
sudo systemctl stop minecraft-server
```

You can send commands to the server with:

```
minecraftctl COMMAND
```

The minecraft configuration is stored in `/etc/conf.d/minecraft.conf`.

Good luck and report any issues to the [Github issue tracker](https://github.com/joefiorini/ansible-minecraft/issues)!
