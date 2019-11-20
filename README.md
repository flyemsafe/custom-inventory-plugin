## Quick example of custom inventory plugins for a KVM (Libvirt) host

Inspired By @termien0
Please see: https://termlen0.github.io/2019/11/16/observations/ for details

Requires: Ansible 2.8

1. Ensure the QEMU guest agent is installed on your vms. This is needed to query the VM networking info.

2. Clone this repo.

3. Generate the CSV file

```
./getvmip > csv_inventory/kvm_inventory.csv
```

4. Run example playbook

```
ansible-playbook -i csv_inventory.yaml playbook.yaml
```
