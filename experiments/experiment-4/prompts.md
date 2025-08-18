# experiment 4

## experiment definition

Use AI to produce a README.md for a role based on the tasks, default variable values, metadata, arg spec, etc.

Could use the output of Experiment 2 as input to this experiment

## initial prompt

Tool: WCA

1. User receives all the files generated in Experiment 2: tasks/main.yml with argspec, defaults/main.yml, and meta/main.yml and opens all three of them in separate VS code tabs.
2. User opens WCA extension.
3. WCA Prompt: System: You are an Ansible role administrator responsible for developing effective documentation for Ansible automation, including roles and playbooks. Prompt: Given @tasks/main.yml, @defaults/main.yml, and @meta/main.yml, generate a README.md with the summary, prerequisites, additional ansible collections, task explanations, variable explanations with default values, license, and author information.