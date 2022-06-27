## Input.txt

Existing line

## Script

- hosts: all
  tasks:
  - name: line insert
    lineinfile:
    path: /Users/mdtutorials2/Documents/Ansible/Input.txt
    line: 'Added Line 1'
    insertbefore: BOF

## Input.txt after execution

Added Line 1
Existing line
