ASBRL-TRAEFIK
=========

Deploy Traefik Docker container.

Requirements
------------

Need to be Docker engine installed.

Role Variables
--------------

- default_user: 'ubuntu'
- IMAGE: 'traefik'
- BUILD: 'v2.3.1'
- DOCKER_LABELS:
    tag1: test
- DOCKER_EXPOSED_BY_DEFAULT: true
- API_INSECURE: true
- DASHBOARD_ENABLED: true
- LOG_LEVEL: INFO
- REDIRECT_HTTP_TO_HTTPS: false

Dependencies
------------

None

Example Playbook
----------------

      - name: Deploy Traefik
        include_role:
          name: asbrl-traefik
        vars:
          API_INSECURE: true
          LOG_LEVEL: DEBUG
        tags:
          - traefik

License
-------

BSD

Author Information
------------------

Moegui.com