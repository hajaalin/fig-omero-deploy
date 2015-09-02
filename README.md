# fig-omero-deploy
Deploy OMERO containers with Ansible and Docker Compose. The images for the containers are built with this project: https://github.com/hajaalin/fig-omero. The images are tagged as `branch-commit`.

```
export DOCKER_TAG=build_with_ansible-f33655dd7168e4dbe83f5484e61d19afa64378d3

ansible-playbook install.yml -i inventory_testing --extra-vars "docker_tag=$DOCKER_TAG" --become-user=root --ask-become-pass

```
