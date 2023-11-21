# SystemD Service Generator

A simple bash script to generate general systemd services.

## Dependencies

This script depends on: `systemd` `fzf` `tput` `getent` `vim`

## Usage

The script is interactive, asks you some questions with suggested answers if
possible and generates the service file at the end.

The script has 3 modes:
- `create` to generate a new service.
- `remove` to remove a service.
- `edit` to edit an existing service using vim.

### Asked Questions

- Service Name
- Service Description
- Working Directory
- Executable Path
- User
- Group
- After
- WantedBy

- Edit using vim
- Enable service on boot time
- Start the service now
