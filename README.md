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

- Edit Service Mode

![](./screens/edit_service.png)

- Set manual directive `Service,ExecStart` to `my_binary`
- Set the service working directory to the current location using option 5
- Finally set the user to `davenchy` using option 6

![](./screens/set_service_directives.png)

- Save Service

![](./screens/save_service.png)
