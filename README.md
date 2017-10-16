# Install python with ansible

Ansible requires python installed on the target hosts to be able to gather facts

You can use this role before any others in your playbooks to make sure that fact gathering will work

Use like this:

    # ensure python is available
    - hosts: all
      roles:
        - python
      gather_facts: False
