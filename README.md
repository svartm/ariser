# Rift ArchLinux ISO

RiftOS is a personal project based on [Ariser](https://ariser.eu/), a configurable automatic terminal install method for ArchLinux. The scripts in this repository can be used to build an archiso with a pre-configured [version](https://github.com/svartm/alis-rift) of the [ALIS](https://github.com/picodotdev/alis) install script.

## About RiftOS

RiftOS is a custom version of ArchLinux, largely inspired by [Ariser](https://ariser.eu/), [ArcoLinux](https://www.arcolinux.info/), and [EndeavourOS](https://endeavouros.com/). It started as a personal project for me to learn about all the parts that make up an Arch based operating system, and to save my preferences and configurations in an easy to understand installer. This enables me to install systems that just work the way I want out of the box. There is also room to expand on this project and make a more generic pre-configuration in the future.

I chose to fork the Ariser project because this method of installation is fast and simple, highly configurable for different use cases, and the ArcoLinux project and its offshoots are specifically built with learning in mind. The ISO can also be reused since it doesn't need to be rebuilt when there is an update to ALIS.

## Building the ISO

1. Ensure you have the correct version (78-1) of the `archiso` package installed. Downgrade with `sudo downgrade archiso` if needed.
2. Clone this repository.
3. Read the scripts before running them and make changes as needed.
4. Run `./build-archlinux-with-alis.sh` and wait for the script to finish. The repository [svartm/alis-rift](https://github.com/svartm/alis-rift) will be cloned and packed into the ISO.

## Installing RiftOS
It's highly recommended to be familiar the [ArchLinux installation process](https://wiki.archlinux.org/title/Installation_guide) before running any automated installer scripts. **Never run installers you don't understand on physical hardware. The ALIS script will partition your disk and you may lose data.**

When the ISO is booted and the command `alis` is run, the user has the option to run the version of the script on the ISO or to pull the newest changes from the repository before installing.

1. Boot from the ISO.
2. Establish internet connection.
3. Edit the alis configuration.
4. Run 'alis'.

See more: [alis-rift](https://github.com/svartm/alis-rift)
