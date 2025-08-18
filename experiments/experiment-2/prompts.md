# experiment 2

## experiment definition

FOAG: Generate an Ansible Role for Automated System Health Checks

Use WCA4Ansible to generate an automated health check playbook that monitors CPU, memory, disk space, and running processes.

## initial prompt

Tools: WCA4A Role Generation & WCA

1. User creates a new collection.
2. WCA4A Prompt: Generate a role for Red Hat Enterprise Linux health check that provides hostname, timestamp in YYYY-MM-DD, IPv4 address, CPU utilization, memory utilization, network interface utilization, and disk utilization information, plus a summary of running processes. Register the output into a file-based log at /vars/log/healthcheck-{{ timestamp }}. This will generate tasks/main.yml & defaults/main.yml, which the user will save into the collection they created, and then leave them open for WCA to reference.
3. User opens WCA extension.
4. WCA Prompt: System: You are a junior Red Hat Enterprise Linux Administrator responsible for automating system health monitoring across all RHEL servers. Your team uses Ansible for automation, and you have been asked to convert your manual process into a reusable Ansible role. Prompt: Add an argspec to @tasks/main.yml and output an updated tasks/main.yml.User saves updated tasks/main.yml.
5. WCA Prompt (in same chat): Given @tasks/main.yml and @defaults/main.yml, generate role metadata and store it in meta/main.yml.
