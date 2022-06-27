
10.0.0.0/16 - network
20.124.199.39 - sysadmin
10.0.20.4 - mvm1
10.0.20.7 - mvm2
pub ip : 52.188.62.46


- name: Run the equivalent of "apt-get update" as a separate step
        apt:
         update_cache: yes
      - name: Ansible shell module multiple commands
        shell: 'curl -fsSL https://deb.nodesource.com/setup_14.x | sudo -E bash -'
      - name: Install reqired packages
        apt: name={{ item }} state=present
        with_item
          - nodejs