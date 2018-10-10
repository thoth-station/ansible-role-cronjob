# Cronjob
This will create a [Project Thoth](https://github.com/thoth-station) CronJob in an OpenShift Project/namespace.

## Requirements

None.

## Role Variables

Available variables are listed below, along with default values:

    namespace: ""
    cronjob_name: ""
    suspend: true

## Dependencies

None.

## Example Playbook

    - hosts: servers
      roles:
        - role: cronjob
        namespace: "frontend"
        cronjob_name: "graph-refresh-cronjob"
        suspend: false

## License

GPLv3
