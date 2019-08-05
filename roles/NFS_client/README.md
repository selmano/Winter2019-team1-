Ansible nfs_client role

This is an Ansible role which manage a nfs client.

Role Variables

A list of all the default variables for this role is avaialble in defaults/main.yml.

Example Playbook

This is an example playbook:

---hosts: all roles: -amtega.nfs_client vars:         nfs_client_mounts:      -src:
acmesever:/acmepath1         path: /mnt/path1       -src: acmeserver:/acmepath2         path:/mnt/path2   
nfs_client_mounts_defaults:       state: present       opts: ro

Testing

Tests are based on docker containers. You can setup docker engine quickly using the playbook files/setup.yml available in the role amtega.docker_engine.

Once you have docker, you can run the tests with the following commands:

$ cd amtega.nfs_client/tests$ ansible-playbook main.yml

License

BSD

Author Information
An optional section for the role authors to include contact information, or a website (HTML is not allowed).
