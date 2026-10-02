Personal configuration for some of Suckless's tools

<img width="1920" height="1080" alt="screenshot" src="https://github.com/user-attachments/assets/04503b2b-80a5-4bba-800a-62aa62256079" />

This is nothing more than a personal config made by a 16-year-old who has a lot of time on his hands. It uses Catppuccin Mocha-style colors, along with QoL patches such as vacant tags, gaps, an underline under active tags, and a simple modification to window management that makes new windows spawn to the side instead of replacing the current one.

The whole purpose of this repository is to give me an easy way to deploy my desktop environment of choice without much difficulty, as I tend to distro-hop between Void and Arch a lot. I'm trying to escape systemd, or something—I’m not really sure. While Void is pretty mature, it has some quirks. For example, trying to run daemons as your user isn't natively supported by runit, so you have to run runsvdir as your user, which is very cumbersome. Because of that, I resort to using xinit to start things like PipeWire, which is a cheap workaround in my opinion.

Void's flexibility is a major selling point, though. I tend to install it using the chroot method, and I don't install the base-system package. Instead, I go with the 290 KB base-files package and build my way up from there. It's a nice way to use Linux since I get to make my own personal Bash script to call dracut and generate a new UKI after every kernel update, then manually point efibootmgr to said UKI, skipping a bloated bootloader like GRUB. The end result is a lean system consuming around 180 MB of RAM at idle. Very satisfying.

Arch, on the other hand, has the annoying plumbing already premade for you, like D-Bus and elogind already being set up. I do like some of the tools, such as systemd-resolved and systemd-boot, but I've already found alternatives in my own setup, namely my Hackintosh-style boot chain and OpenResolv. Add the AUR drama on top of that, and Arch becomes a somewhat questionable choice. That said, the Arch repositories are way superior to what Void's are ever going to be.

Anyway, sorry to ramble on. Here is the repository—do with it as you please. I may add screenshots, but don't count on it.
