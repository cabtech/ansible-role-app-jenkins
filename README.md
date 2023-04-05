# ansible-role-app-jenkins
Installs a Jenkins server

## Default variables
| Name | Type | Value | Comments |
| ---- | ---- | ----- | -------- |
| jenkins_addr | IPv4 | `127.0.0.1` | localhost |
| jenkins_dependencies | list(string) | see `defaults.yml` ||
| jenkins_pkgs | list(string) | see `defaults.yml` ||
| jenkins_port | integer | 8080 ||
| jenkins_repo_key_url | URL | `https://pkg.jenkins.io/debian-stable/jenkins.io-2023.key` ||
| jenkins_repo_keyring | UnixPath | `/usr/share/keyrings/jenkins-keyring.asc` ||
| jenkins_repo_url | URL `https://pkg.jenkins.io/debian-stable` ||
| jenkins_svc_enabled | Boolean | true ||
| jenkins_svc_name | string | jenkins ||
| jenkins_svc_state | string | started ||
| jenkins_username | string | jenkins ||
