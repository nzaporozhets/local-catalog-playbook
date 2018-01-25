# Local Catalog build automation #

This playbook can be used for deploying Local Catalog for DC/OS.

### Requirements ###

This playbook uses localhost for building the catalog tarball.

You can use your bootstrap node for building the repo tarball and configuring cluster hosts. 
Host running ansible should have following:
- Docker
- Git
- Python3

### Usage ###

1. Copy the hosts.example file and populate it with actual hosts config. 
2. Configure DC/OS version used and desired packages in the default_vars file. 
3. Run the site.yml playbook
4. Follow instructions to point DC/OS to new repository using DC/OS CLI.