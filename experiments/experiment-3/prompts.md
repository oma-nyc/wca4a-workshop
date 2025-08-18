# experiment 3

## experiment definition

Build a role based on documented specs, for example: a team that FOAG supports was responsible for verifying the upgrade of a server based on tests performed on the N+1 system. Generate code to perform the tests. Explain the Ansible content that was generated.

## initial prompt

Tool: WCA4A Role Generation & Explanation

Assumes new or existing collection has been created

Prompt (generic): Verify that the server changes listed were carried out on the managed servers: <provide list of changes>

Prompt (example): Verify that the server changes listed were carried out on the managed servers: Perform updates on the linux servers, Check the date on all the servers, verify docker is installed on all linux servers, verify nginx is installed, ensure it is running, and has deployed a static webpage.This will generate tasks/main.yml & defaults/main.yml, which the user will save into the collection they created,
