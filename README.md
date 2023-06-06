# dfrab
This is a simple utility programed in bash that can backup and rollback your dotfiles

Backup and Profile means the same thing in this program and is used interchangably

## Install

### Local user install

Installs for local user only. This install doesn't require root

```bash
rm -f ~/.local/bin/dfrab ; wget -P ~/.local/bin https://raw.githubusercontent.com/dnkmmr69420/dotfile-rollback-and-backup/main/bin/dfrab ; chmod a+x ~/.local/bin/dfrab
```

### System wide install

Installs for all users. Requires root to install but doesn't require root to use dfrab

```bash
sudo rm -f /usr/local/bin/dfrab ; sudo wget -P /usr/local/bin https://raw.githubusercontent.com/dnkmmr69420/dotfile-rollback-and-backup/main/bin/dfrab ; sudo chmod a+x /usr/local/bin/dfrab
```


## Usage

### Get started

To get started type this

```bash
dfrab init
```

That will create ~/.dfrab where there will be backups/profiles you can make copies of and switch to different profiles

### Commands

- link: links a file or directory for dfrab to manage it. You must be in the same directory where the directory or file you are trying to link
- switch-profile: switches to a different profile or backup
- create-profile: makes a copy of your current profile and switches to it
- create-backup: creates a copy of your current profile
- remove-backup: removes a profile/backup. This program won't be able to remove your current profile unless you switched to a different profile
- unlink: converts the link for dfrab to manage to a regular directory or file
- profile-copy: makes a copy of a profile
- rename-profile: renames a profile, even your current profile
- list-backups: lists all of your profiles/backups
- list-contents: list contents of your current profile
- what-profile: prints your current profile
- help: displays help
