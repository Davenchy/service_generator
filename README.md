# SystemD Service Generator

A simple bash script to generate/control systemd services.

## Dependencies

This script depends on: `systemd` `fzf` `tput` `getent` `vim`

## Usage

The script works in interactive mode only!!

The script has 3 modes:
- `Create` to generate a new empty and unusable service.
- `Control` to control a service (Start/Stop/Enable/Disable/Logs/...).
- `Edit` to edit a service (add/remove directives to control service behavior).

## Screenshots

- Overall script output in create mode

![Overall script output in create mode](screens/screen1.png)

- How using fzf to select suggested answers for some fields.

![How using fzf to select suggested answers for some fields](screens/screen2.png)
