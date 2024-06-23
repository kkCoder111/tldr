# VBoxManage

> Command-line interface to VirtualBox.
> Includes all the functionality of the GUI and more.
> Some subcommands such as `vboxmanage startvm` have their own usage documentation.
> More information: <https://www.virtualbox.org/manual/ch08.html#vboxmanage-intro>.

- Execute a VboxManage subcommand:

`VBoxManage {{subcommand}}`

- Display help:

`VBoxManage --help`

- Display help for a specific subcommand:

`VBoxManage --help {{clonevm|import|export|startvm|...}}`

- Display version:

`VBoxManage --version`

- List all virtual disk images (macOS only):

`vboximg-mount --list --verbose`

- View partition information about a specific disk image (macOS only):

`vboximg-mount --image=<UUID> --list`

- Mount a specified disk image using FUSE (macOS only):

`vboximg-mount --image=<uuid> -p <partition number> <fuse location>`

- Mount the vhdd file from a FUSE-mount disk image so that it can be viewed:

`sudo mount <fuse_location>/vhdd <new_mount location>`
