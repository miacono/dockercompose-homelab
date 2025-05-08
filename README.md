# My HomeLab

This repo is meant to be used in case of disaster recovery for my home lab.

## Contents

* **JuiceFS** mounting a **MinIO** bucket as local volume for backup purposes.

## Prerequisites

* Install the JuiceFS plugin on docker

    ```console
    docker plugin install juicedata/juicefs
    ```
* The folder `./secrets` contains the following:

    * a pem file created with the `openssl genrsa -out juicefs-priv-key.pem -aes256
 2048` command

    * a `juicefs-key-passphrase.txt` file with the passphrase submitted with the previous command

