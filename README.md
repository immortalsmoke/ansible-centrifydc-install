# ansible-centrify-install
This is an Ansible role for installing CentrifyDC Express and joining on Debian and Red Hat flavored Linux distros.

##### Task Overview
1. Download and extract CentrifyDC
2. Install CentrifyDC if not yet installed
3. Join server to the

##### Instructions
1. Verify that the URLs and filenames in `vars/RedHat.yml` and `vars/Debian.yml` point to the version of Centrify you wish to install
2. Uncomment and define `domain` in `vars/main.yml` if you wish to join the server to a domain

##### Roadmap
1. Add -c "{{ ou_path }}" option to have the server automatically placed in the proper OU when joining to domain
