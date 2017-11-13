# Packsible

A Docker image with Packer (https://packer.io) and Ansible (https://www.ansible.com/) installed.

## Run

```shell
docker run --rm \
    -e AWS_ACCESS_KEY_ID \
    -e AWS_SECRET_ACCESS_KEY \
    -v "$(pwd)":"$(pwd)" \
    -w "$(pwd)" \
    mergermarket/packsible build packer-template.json
```
