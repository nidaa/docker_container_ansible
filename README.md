# docker_container_ansible

this is  ansible playbook, using roles that:
- Spawn 2  local  docker containers
- Container one  have docker_root user with automatically generated key pair
- Container one  have user provided SSH-public key (as a  variable) added to docker_root user authorized_keys.
- Container two  allow to SSH from container one using docker_root user and the generated keys
- Check the connectivity from container one to container two in automated way.
