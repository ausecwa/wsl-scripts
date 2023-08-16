# WSL Scripts

These are Bash scripts for setting up and installing various components for Debian-based Linux distros via Windows Subsystem for Linux.

- basicSetup
    - Updates packages
    - Installs `ssh`, `git`, `wget`, `rsync`, `vim`
    - Enable `systemd` and bug fix that prevents `.exe` execution
    - Disable IPv6
    - Disable bell sound
    - (commented out) Disable `ufw`
- condaInstall
    - N.B.: This will shutdown all open WSL sessions
		- TODO: Use `wsl -t <distro>`
    - Downloads, installs, and updates `miniconda`
    - Installs initial `basic` environment
    - Initializes `conda`
- cudaInstall
	- N.B.: NVidia drivers on Windows needs to be appropriate version first!
	- Installs CUDA Toolkit files on the Linux side
- wslFetchInstall
	- N.B.: Pure vanity
	- Installs WSL Utilities
	- Enables `MOTD` so `wslfetch` displays every time a session is opened