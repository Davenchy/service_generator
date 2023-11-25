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

## Help Messages

### Control Mode

```
Status:
	Show service status

Start:
	Start the service

Stop:
	Stop the service

Restart:
	Restart the service

Enable:
	Enable the service to start at boot time

Disable:
	Disable the service to start at boot time

Print:
	Print the service configuration

Logs:
	Show the service logs

Follow Logs:
	Show the service logs and wait for new updates

Edit:
	Enter edit mode to edit the service

Help:
	Show this help message

Editor:
	Open the service file in a text editor (\$EDITOR)

Remove:
	Stop, Disable then Remove the service

Clipboard:
	Copy the service file content into your system clipboard

Copy:
	Copy the service configuration to a new name

Rename:
	Rename the service to a new name

Create Service:
	Create a new service

Select Service:
	Select another service

Back:
	Go back one step

Exit:
	Exit this script

```

### Edit Mode

```
List:
	List the service file with colored current values

Show:
	Show the value of a key (section,directive) e.g. Unit,Description

Set:
	Select Section,Directive and set its value, set empty value to remove the directive

Set Manual:
	Use manual key(Section,Directive) to create/set/remove directive

Set Current Working Directory:
	Set directive Service,WorkingDirectory to current working directory

Set User:
	Set Service,User to the selected user

Set Group:
	Set Service,Group to the selected group

Set Type:
	Set Service,Type to the selected service types

Help:
	Print this help message

Reload:
	Reload the current service file and discard changes

Save:
	Save the current changes to the service file, Reload SystemD Daemons and return back to the control mode

Back:
	Discard current changes and return back to control mode

Exit:
	Discard current changes and exit the script

```
