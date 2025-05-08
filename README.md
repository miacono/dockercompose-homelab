# My HomeLab

This repo is meant to be used in case of disaster recovery for my home lab.

## Contents

* **JuiceFS** mounting a **MinIO** bucket as local volume for backup purposes.

## Prerequisites

* Install the JuiceFS plugin on docker

    ```console
    docker plugin install juicedata/juicefs
    ```
* The folder `./secrets` contains a pem file created by running

    ```console
    openssl genrsa -out juicefs-priv-key.pem -aes256 2048` command
    ```

* The `.env` file is properly set