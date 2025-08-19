# experiment 6

## Use case

Augment an existing Ansible playbook or role using AI-powered task completion in WCA4A
- Does not require an initial prompt

## Initial Prompt

Create an Ansible playbook that checks if root filesystem has at least 2GB free space using ansible_mounts. Detect OS type and backup /etc/passwd and /etc/hosts. Update all packages using yum for Red Hat or apt for Debian. After patching, restart common services like httpd, nginx, and sshd only if they exist on the system. Send email notification with patch status including hostname and number of packages updated.

