# qm snapshot

> Create virtual machine snapshots.
> More information: <https://pve.proxmox.com/pve-docs/qm.1.html>.

- Create a snapshot of a specific virtual machine:

`qm {{[sn|snapshot]}} {{vm_id}} {{snapshot_name}}`

- Create a snapshot with a specific description:

`qm {{[sn|snapshot]}} {{vm_id}} {{snapshot_name}} --description {{description}}`

- Create a snapshot including the vmstate:

`qm {{[sn|snapshot]}} {{vm_id}} {{snapshot_name}} --description {{description}} --vmstate 1`
