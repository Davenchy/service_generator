# SystemD Service Generator

A simple bash script to generate/control systemd services.

## Dependencies

This script depends on: `systemd` `fzf` `tput` `getent` `vim` `xclip`

## Usage

The script works in interactive mode only!!

The script has 3 modes:

- `Create` to generate a new empty and unusable service.
- `Control` to control a service (Start/Stop/Enable/Disable/Logs/...).
- `Edit` to edit a service (add/remove directives to control service behavior).

## Screenshots

- The Main Menu

![](./screens/main_menu.png)

- Creating a new service

![](./screens/create_service.png)

- Searching for a service using FZF

![](./screens/search_service.png)

- Control a service

![](./screens/control_service.png)
