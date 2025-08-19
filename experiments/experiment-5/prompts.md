# experiment 5

## Tool: WCA4A and/or WCA

### WCA4A

1. Choose an existing script that you use today.
2. Open the Script in VS Code and copy its entire contents to the clipboard.
3. Open the Ansible Extension in VS Code and click "Generate Playbook."
4. In Playbook Generation, type "Convert the following shell script to a playbook: " and then paste in the contents of the script.

### WCA

1. Choose an existing script that you use today.
2. Open the Script in VS Code. No need to copy its content to the clipboard.
3. Issue the following Prompt in WCA: System: you are a senior Red Hat Enterprise Linux systems administrator responsible executing application management scripts on multiple managed servers. You are learning how to replace your shell scripts with Ansible playbooks. Question: Begin converting the shell script in @ to an Ansible Playbook.

## Prompts from Asia!

### Task the First

1. Detect the operating system, database, and middleware type by using ansible facts.
2. Fail the playbook if AIX version is below a specified minimum (variable: min_aix_version) & Linux kernel version or OS version if below a specified minimum (variables: min_linux_kernel, min_linux_version)
3. Gather the operating system version and kernel version
4. Collect the database version, uptime, and instance name
5. Output the middleware components, version, and instance name
6. Output results grouped by operating system, database, and middleware

### Task the Second

1. Check for running instances of Connect:Direct, SecureTransport, Sterling File Gateway, and add any additional Managed File Transfer and Advance File Transfer listed in a variable (mft_components or aft_components) 
2. Check if the components exist by checking for installed packages 
3. Check if processes are running by pgrep command 
4. If component is found, gracefully stop the related services
5. Verify if processes have stopped 

### Task the Third

1. Read instance names, profile names, and installation paths from a variables file.
2. For each instance, gracefully stop all JVMs in the profile using stopServer.sh or stopManager.sh
3. Include support for stopping JVM's, DMGR, Node Agent, and IHS
4. Verify each instance has stopped
5. Include error handing for instances that have already been stopped.
6. Output a summary of stopped instances with status

