# Jail on Bond

Jail on Bond is a bot that tracks individuals being held in Connecticut Department of Corrections facilities while awaiting trial.

Jail on Bond has two souls. It is a twitter bot and an e-mail bot.



## How to deploy a bot

### Automation: Crontab

1) Connect to your server.

Usually, it should work like this,

Point were (in which (`Folder`) is our file:

```

scp ~/Folder/file.py

```

Once we have located our file, we should point to our server `root@1.2.3.4`, where `1.2.3.4` refers to our IP Address (1.2.3.4 = IP Address):

```

scp ~/Folder/file.py root@1.2.3.4

```

2) Once in your server, you should open crontab.

What is crontab?

Cron is driven by a crontab (cron table) file, a configuration file that specifies shell commands to run periodically on a given schedule. Often there is a system-wide crontab file (usually in /etc or a subdirectory of /etc) that only system administrators can edit.

The configuration file for a user can be edited by calling `crontab -e` regardless of where the actual implementation stores this file.

Each line of a `crontab`. file represents a job

What is cron?

The software utility cron is a time-based job scheduler in Unix-like computer operating systems.

```
crontab -e
```

Once you are inside your cron editor, it is time to add some instructions to run your bot.


First of all, have a look to [Crontab.guru](https://crontab.guru/). Crontab Guru is one of the best resources out there to create and edit your cron schedule expressions

3) 2 for nano
4) * * * * * python3 file.py
5) ctrl+x
6) say 'y' you want to save modified buffer
7) Hit enter to agree to the filename