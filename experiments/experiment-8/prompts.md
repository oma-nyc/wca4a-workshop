# experiment 8

## use case

## initial prompts and variants

### Playbook Generation with WCA4A

Prompt: Generate an Ansible playbook that connects to Cisco IOS devices using network_cli. The playbook should run the show running-config command and save the output to a backup file on the control node, with a filename that includes the device hostname and a timestamp. Then, include an optional step to restore the configuration from that backup file using the ios_config module. Use variables for the backup directory and support a conditional restore step that runs only when restore_config is set to true.

### Variants

- Repeat the above for
  - Cisco NX-OS devices and/or prompt to use the cisco.nxos collection.
  - Cisco IOS-XR / cisco.iosxr collection
- Create a playbook to configure an F5 BIG-IP Load Balancer
  - Create a pool named "web." Add member to pool 10.10.10.10 web01. Create a VIP vip-1 with profiles https and clientssl.


