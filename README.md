# Ansible Role: Kibana

[![Build Status](https://travis-ci.org/Nikita-Stupin/ansible-role-kibana.svg?branch=master)](https://travis-ci.org/Nikita-Stupin/ansible-role-kibana)

An Ansible Role that installs Kibana on RedHat/CentOS or Debian/Ubuntu.

## Requirements

None.

## Role Variables

Available variables are listed below, along with default values (see `defaults/main.yml`):

    kibana_version: "5.x"

The version of kibana to install (major and minor only).

    kibana_server_port: 5601
    kibana_server_host: "0.0.0.0"

The FQDN or IP address and port Kibana should use.

    kibana_elasticsearch_url: "http://localhost:9200"

The URL (including port) over which Kibana will connect to Elasticsearch.

## Dependencies

None.

## Example Playbook

    - hosts: kibana
      roles:
        - meganuke.kibana

## License

MIT / BSD

## Authors: Information

This role was originally created in 2014 by [Jeff Geerling](https://www.jeffgeerling.com/), author of [Ansible for DevOps](https://www.ansiblefordevops.com/).

Development continues in 2017 by [Nikita Stupin](https://nikitastupin.name)
