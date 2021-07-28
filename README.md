# mkinitcpio-zerotier
mkinitcpio hook that initialises ZeroTier One to assist in the remote unlocking of encrypted partitions.  
Heavily inspired from [mkinitcpio-wireguard](https://github.com/dharrigan/mkinitcpio-wireguard).

## Motivation

This package assumes you are already able to remotely unlock your encrypted Arch Linux device via SSH within your LAN ([ArchWiki page](https://wiki.archlinux.org/title/Dm-crypt/Specialties#Remote_unlocking_of_the_root_(or_other)_partition)).  

By connecting to a private ZeroTier One network at boot, it will be possible to use SSH decryption also within the VPN, useful if you are far away from your encrypted device.

## Installation

Install the package with `yay -S mkinitcpio-zerotier`, then follow the steps that appear on your screen after the installation or when you run `mkinitcpio -H zerotier`.



