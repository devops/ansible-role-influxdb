# Ansible Role: InfluxDB


[![Build Status](https://travis-ci.org/devops/ansible-role-influxdb.svg?branch=master)](https://travis-ci.org/devops/ansible-role-influxdb)

## Requirements

None.

## Role Variables

Available variables are listed below, along with default values (see `defaults/main.yml`):

* `influxdb_packages:`
    ```
      - influxdb      
    ```

    Supported formats
    ```
      - influxdb
      - https://repos.influxdata.com/centos/7/x86_64/stable/influxdb-0.13.0.x86_64.rpm
      - /tmp/influxdb-0.13.0.x86_64.rpm
    ```
* `influxdb_repo: True`
* `influxdb_repo_url: 'https://repos.influxdata.com'`
* `influxdb_base_dir: '/var/lib/influxdb'`
* `influxdb_reporting_disabled: 'true'`
* `influxdb_meta_dir: '{{ influxdb_base_dir }}/meta'`
* `influxdb_data_dir: '{{ influxdb_base_dir }}/data'`
* `influxdb_wal_dir: '{{ influxdb_base_dir }}/wal'`

## Dependencies

None.

## Example Playbook

`see tests/test.yml`

## License

MIT / BSD

## Author Information

z.
