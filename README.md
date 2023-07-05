# Example showing the use of Ansible for security scanning and remediation

References:

- https://medium.com/@jackprice/ansible-openscap-for-compliance-automation-14200fe70663
- There are also CIS roles on the RedHatOfficial Ansible Galaxy site: https://galaxy.ansible.com/RedHatOfficial

## cis_scan.yml

Uses the OpenSCAP scanner to generate a report and associated Ansible remediation playbook based on the CIS profile (these will be placed in the local directory oscap-reports)

Example usage:

    ansible-playbook -i my-inventory-file.yml cis_scan.yml -l hosttoscan.example.com
