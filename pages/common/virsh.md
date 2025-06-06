# virsh

> Manage `virsh` guest domains. (Note: `guest_id` can be the ID, name or UUID of the guest).
> Some subcommands such as `list` have their own usage documentation.
> More information: <https://libvirt.org/manpages/virsh.html>.

- Connect to a hypervisor session:

`virsh connect {{qemu:///system}}`

- Activate a network named `default`:

`sudo virsh net-start {{default}}`

- List all domains:

`virsh list --all`

- Create a guest from a configuration file:

`virsh create {{path/to/config_file.xml}}`

- Edit a guest's configuration file (editor can be changed with $EDITOR):

`virsh edit {{guest_id}}`

- Start/reboot/shutdown/suspend/resume a guest:

`virsh {{command}} {{guest_id}}`

- Save the current state of a guest to a file:

`virsh save {{guest_id}} {{filename}}`

- Delete a running guest:

`virsh destroy {{guest_id}} && virsh undefine {{guest_id}}`
