# ansible-role-sonarqube-nginx-docker

Install SonarQube and nginx on docker container.

nginx is https reverse proxy for SonarQube.

## Requirements

- docker
- docker-compose (pip)

## Role VAriables

```
sonarqube_nginx_docker_dir: /opt/sonarqube-nginx-docker

sonarqube_nginx_docker_nginx_tag: 1.15.0-alpine
sonarqube_nginx_docker_sonarqube_tag: 7.1-alpine
sonarqube_nginx_docker_nginx_ssl_port: 9443

sonarqube_nginx_docker_ssl_crt_path: /etc/ssl/certs/server.crt
sonarqube_nginx_docker_ssl_key_path: /etc/ssl/certs/server.key
```

## Example Playbook

```
- hosts: all
  roles:
    - role: heriet.sonarqube-nginx-docker
```

## License

Apache License 2.0
