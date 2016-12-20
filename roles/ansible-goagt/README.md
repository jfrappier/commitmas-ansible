Ansible GoCD
=========

This role will help setup GoCD for Debian and RedHat based systems. GoCD is an Open source continuous delivery server to model and visualize complex workflows.

To Do
-----
- Task to add/configure yum repo
- Task to install Java (yum)
- Task to install GoCD server (yum)
- Task to add/configure apt repo
- Task to install Java (apt)
- Task to install GoCD server (yum)
- Handler to start GoCD server
- Task to install GoCD agent (yum)
- Task to install GoCD agent (apt)
- Handler to start GoCD agent
- Task to copy sample config file to GoCD agent

Requirements
------------

GoCD uses a server/agent model. This role assumes that two servers are available and defined in /etc/ansible/hosts in groups called [gosrv] and [goagt]. You can adjust these per your level of CDO (OCD in alphabetical order).

Additionally, GoCD requires Java, however this role will (attempt) to install Java accordingly. Additional documentation is available [here](https://docs.go.cd/current/installation/install/server/linux.html).

Role Variables
--------------

javaver - Version of Java used by the install documentation


Dependencies
------------

A list of other roles hosted on Galaxy should go here, plus any details in regards to parameters that may need to be set for other roles, or variables that are used from other roles.

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - hosts: servers
      roles:
         - { role: username.rolename, x: 42 }

License
-------

BSD

Author Information
------------------

This role is for testing purposes, and offers no warranty. Use at your own risk. Forks and PRs welcome.
