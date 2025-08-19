# experiment 7

## Playbook Generation in WCA4A

### Initial Prompt:

Create an Ansible playbook that uses service_facts to check the status of httpd, nginx, and mysql services. Restart only the ones that are stopped or failed by looping through ansible_facts.services and checking item.key and item.value.state. Use failed_when or per-task error detection to identify any restart failures. Run vmstat 1 2, parse the second line, and if CPU idle is under 20%, log “High CPU detected” to /var/log/ansible_healing.log. Clean up files in /tmp that are older than 7 days using the find and file modules. If any restart fails, send an email alert with the hostname in the subject using the community.general.mail module.

### Boris Prompt post-discussion

Generate an Ansible playbook that automates a pre-approved change process triggered by an incident. The playbook should: 1) validate the incident by querying an API, 2) create a change ticket using a standard template and link it to the incident, 3) update the change ticket status to “Scheduled”, 4) remotely restart a service like nginx on the impacted host, and 5) close both the change and incident tickets using API calls. Use the uri module for API interactions, the service module for remediation, and include variables for incident ID, host, API URLs, and tokens. Include headers and sample payloads where applicable.

