# Examples showing the use of Ansible for security scanning and remediation

Helpful reference:  https://medium.com/@jackprice/ansible-openscap-for-compliance-automation-14200fe70663

### cis_scan.yml

Uses the OpenSCAP scanner to generate a report and associated Ansible remediation playbook based on the CIS profile (these will be placed in the local directory oscap-reports)

Example usage:

`ansible-playbook -i my-inventory-file.yml cis_scan.yml -e "target_host=hosttoscan.example.com"`

### rhel_c2s.yml

Runs the C2S role from the RedHatOfficial galaxy namespace

Example usage:

`ansible-playbook -i my-inventory-file.yml rhel_c2s.yml -e "target_host=hosttoscan.example.com"`
