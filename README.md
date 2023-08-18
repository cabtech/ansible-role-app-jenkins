----
# ansible-role-app-jenkins
Installs a Jenkins server on Ubuntu

## To Do
- Support RedHat based distros such as Rocky Linux and Amazon Linux 2023
- Install agent jar file if `jenkins_role == agent`
- Switch to depend on openjdk role

## Default variables
| Name | Type | Value | Comments |
| ---- | ---- | ----- | -------- |
| jenkins_addr | IPv4 | `127.0.0.1` | localhost |
| jenkins_aws_client | Boolean | false | set to true if using, e.g. upload to S3 |
| jenkins_aws_pkgs | list(string) | see `defaults.yml` | packages to install if using AWS |
| jenkins_dependencies | list(string) | see `defaults.yml` ||
| jenkins_pkgs | list(string) | see `defaults.yml` ||
| jenkins_port | integer | 8080 ||
| jenkins_repo_key_url | URL | `https://pkg.jenkins.io/debian-stable/jenkins.io-2023.key` ||
| jenkins_repo_keyring | UnixPath | `/usr/share/keyrings/jenkins-keyring.asc` ||
| jenkins_repo_url | URL `https://pkg.jenkins.io/debian-stable` ||
| jenkins_role | string | server | if not `server` then anything will do |
| jenkins_svc_enabled | Boolean | true | will be set to false if `jenkins_role != server` |
| jenkins_svc_name | string | jenkins ||
| jenkins_svc_state | string | started | will be set to stopped if `jenkins_role != server` |
| jenkins_username | string | jenkins ||
----
