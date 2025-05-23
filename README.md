# My HomeLab

This repo is meant to be used in case of disaster recovery for my home lab.

## Contents

* **JuiceFS** mounting a **MinIO** bucket as local volume for backup purposes.
* **Deluge** as download manager.

## Prerequisites

* The folder `./secrets` contains a pem file created by running:

    ```console
    openssl genrsa -out juicefs-priv-key.pem -aes256 2048
    ```

* Copy the `env.template` file to `.env` and set the parameters in it.