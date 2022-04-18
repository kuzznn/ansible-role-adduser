---
- name: User 
  hosts: all
  become: yes
  roles:
    - role: add-key
  vars:
  - user: app
  - group: app
  - comment: app
  - pubkey: insert pub key 
  - sudo: "yes" 