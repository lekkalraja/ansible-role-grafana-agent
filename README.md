grafana-agent
=============

This Role Helps to install grafana-agent on `centos, rhel, fedora` os families and start agent using docker-compose


Role Variables
--------------

* This Role uses the below variables, and these are initialized in `var/main.yml` as default values.

- `agent_dir` : Destination folder to clone the agent repo (Default : /home/ec2-user/grafana-agent)
- `agent_repo` : Grafana-Agent Repository URL to clone (Default : https://github.com/grafana/agent.git)
- `packages` : List of packages to install through `yum` pakcage manager


Example Playbook
----------------
* The Example below shows how to include the `grafana-agent` role on playbooks

    - hosts: servers
      roles:
        - grafana-agent

