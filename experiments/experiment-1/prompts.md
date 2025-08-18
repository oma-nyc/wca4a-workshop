# experiment 1

## experiment definition

FOAG: Generate an Ansible Playbook for Automated System Health Checks

Use WCA4Ansible to generate an automated health check playbook that monitors CPU, memory, disk space, and running processes.

## initial prompt

Tool: WCA4A

Prompt: Generate a single playbook for Red Hat Enterprise Linux health check that provides hostname, timestamp in YYYY-MM-DD, IPv4 address, CPU utilization, memory utilization, network interface utilization, and disk utilization information, plus a summary of running processes. Register the output into a file-based log at /vars/log/healthcheck-{{ timestamp }}.

PREFERRED: Generate an Ansible playbook for RHEL that gathers hostname, timestamp, IPv4 address, CPU/memory/disk usage, and active processes using Ansible facts and standard CLI tools. Register all outputs and log them to a timestamped file in /var/log/. Use become: true, avoid interactive tools, and make sure each command uses register: