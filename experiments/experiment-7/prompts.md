# experiment 7

## Playbook Generation in WCA4A

### Initial Prompt:

Create an Ansible playbook that uses service_facts to check the status of httpd, nginx, and mysql services. Restart only the ones that are stopped or failed by looping through ansible_facts.services and checking item.key and item.value.state. Use failed_when or per-task error detection to identify any restart failures. Run vmstat 1 2, parse the second line, and if CPU idle is under 20%, log “High CPU detected” to /var/log/ansible_healing.log. Clean up files in /tmp that are older than 7 days using the find and file modules. If any restart fails, send an email alert with the hostname in the subject using the community.general.mail module.


