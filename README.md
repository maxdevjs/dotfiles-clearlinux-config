# dotfiles-clearlinux-config
Personal config/setup files for Clear Linux

## Post install

### Google Chrome

> check `setup-flatpak`

- several options:
	- [Installing Google Chrome on Clear Linux*](https://community.clearlinux.org/t/installing-google-chrome-on-clear-linux/1132)

### Firefox

> check `setup-first-time`

- Disable hardware acceleration othewise Firefox will get crazy
	- [YouTube An error occurred. Please try again later](https://community.clearlinux.org/t/youtube-an-error-occurred-please-try-again-later/4451/3)
		- `about:config`
			- `security.sandbox.content.level 2`
			- `security.sandbox.content.read_path_whitelist = /sys/devices/pci0000:00/0000:00:02.0/subsystem`
- [Bash Script to Add H.264 Support for Firefox](https://community.clearlinux.org/t/bash-script-to-add-h-264-support-for-firefox/2367)

## TODO

### Criticals

- [x] `home` without `/etc/fstab`
	- [CLR_MNT_ question yet again](https://community.clearlinux.org/t/clr-mnt-question-yet-again/8101/3)
- [x] samba: install && configure && test
- [x] fix `kitty -v` creates `kitty` empty dir in `$XDG_CONFIG_HOME`

### Normal

- [ ] fonts
- [ ] `gh`: check version for update
- [ ] `install_ffmpeg.bash`: refactor
- [x] `vimix-icon-theme`: fix installation
- [ ] `fzf`: install
- refactor
	- [x] `setup-fish`: installation/update
	- [x] `setup-kitty`: installation/update
	- [x] `setup-utilities`: refactor single_repo and repos
		- [ ] update [dotfiles-solus-config](https://github.com/maxdevjs/dotfiles-solus-config)
			- [ ] setup-utilities: single_repo and repos to repo_operations
			- [ ] setup-fish: (setup-shell)
			- [ ] setup-kitty

