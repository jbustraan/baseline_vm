## baseline_vm
A baseline set of Ansible scripts run on newly provisioned virtual machines

**Note**: VM name or VM group needs to exist in /etc/ansible/hosts
1. Ensure dnf makecache service runs 1x daily
2. Ensure dnf updates are automatically applied
3. Ensure new motd banner is set
4. Ensure shell history logging with date and time stamp is enabled
5. Ensure sshd_config has secure and standard settings
6. Ensure Zabbix agent is installed
7. Restart sshd, rsyslog, zabbix-agent, dnf-automatic

### Run instructions
 ```
 $ ansible-playbook main.yml
Enter Virtual machine name (FQDN) or group: [testvmXX.bustraan.lab]:
```
