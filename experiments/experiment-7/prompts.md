# experiment 7

## Playbook Generation in WCA4A

### Initial Prompt:

Create an Ansible playbook that uses service_facts to check the status of httpd, nginx, and mysql services. Restart only the ones that are stopped or failed by looping through ansible_facts.services and checking item.key and item.value.state. Use failed_when or per-task error detection to identify any restart failures. Run vmstat 1 2, parse the second line, and if CPU idle is under 20%, log “High CPU detected” to /var/log/ansible_healing.log. Clean up files in /tmp that are older than 7 days using the find and file modules. If any restart fails, send an email alert with the hostname in the subject using the community.general.mail module.

### Boris Prompt post-discussion

Generate an Ansible playbook that automates a pre-approved change process in ServiceNow. The flow is: Validate an incident by querying the ServiceNow incident API using the incident_id. Extract the cmdb_ci (Configuration Item) from the incident. Use the cmdb_ci to determine the appropriate pre-approved change template (this could be based on a mapping or API lookup). Create a change request in ServiceNow using the correct change template ID tied to the CI. Update the change request state to “Scheduled”. Connect to the CI host and perform remediation (e.g., restart a service). Close the change request and update the incident as resolved. Use the uri module to interact with ServiceNow REST APIs. Use set_fact or lookup if any CI-template mappings are done locally. Use delegate_to or a second play to run remote remediation.

