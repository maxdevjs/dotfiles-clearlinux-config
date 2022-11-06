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

- [ ] [fish shell](https://fishshell.com/)
	- [ ] [fisher](https://github.com/jorgebucaran/fisher)
		- [ ] [nvm.fish](https://github.com/jorgebucaran/nvm.fish)
		 - [ ] [Node.js®](https://nodejs.org/en/)
		 	- [ ] not available after... reboot? logout?
		 	 - [ ] current workaround:
		 	 	- `nvm install latest`
		 	 		- `set --universal nvm_default_version latest`
		 	 			- unavailable in new spawned shells
		
- [ ] Nitrogen: install
- [ ] Polybar: install

- [ ] `i3`
	- [ ] mom, I lost `gnome-settings-daemon`
		- [ ] [use gnome 43 gnome services with i3](https://www.google.com/search?q=use+gnome+43+gnome+services+with+i3)
		- [ ] [Is gnome-settings-daemon no longer a program I can run from the command line?](https://www.reddit.com/r/gnome/comments/wt8oml/is_gnomesettingsdaemon_no_longer_a_program_i_can/)
		- [ ] [Is there any way to integrate the i3wm into gnome session?](https://www.reddit.com/r/gnome/comments/j9tt0j/is_there_any_way_to_integrate_the_i3wm_into_gnome/)
		- [ ] [How to run i3 in gnome shell (or similar)?](https://www.reddit.com/r/i3wm/comments/2nv3hn/how_to_run_i3_in_gnome_shell_or_similar/)
			- [ ] [Best Gnome Tiling Window Manager for Gnome](https://www.reddit.com/r/gnome/comments/hg5mun/best_gnome_tiling_window_manager_for_gnome/)
				- [ ] [Material Shell](https://github.com/material-shell/material-shell)
					- provided as extension
						- not an option, too many drawbacks
				- [ ] [Pop Shell](https://github.com/pop-os/shell)
					- provided as extension?
					- [ ] [Pop Launcher](https://github.com/pop-os/launcher)
						- requires:
							- [Rust/Cargo](https://www.rust-lang.org/)
							- [just](https://github.com/casey/just)
						
				- [ ] [Tidal Window Manager](https://github.com/rustysec/tidalwm)
				- [ ] [Regolith](https://regolith-linux.org/)

- [ ] [VSCode](https://code.visualstudio.com):
	- [x] install via `nix-env`
	- [ ] install via `rpm`
	- [ ] install via `flatpak`

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

