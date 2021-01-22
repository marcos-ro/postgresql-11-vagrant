# PostgreSQL 13 on Debian Buster 10
## Requirements
| Name    | Description                                                                                                                                 |
|---------|---------------------------------------------------------------------------------------------------------------------------------------------|
| Vagrant | Vagrant enables users to create and configure lightweight, reproducible, and portable development environments.                             |
| Ansible | Ansible is the simplest way to automate apps and IT infrastructure. Application Deployment + Configuration Management + Continuous Delivery.|

## Login

| Name     | Content      |
|----------|--------------|
| Database | all          |
| User     | vagrant      |
| Password | vagrant      |
| Host     | 192.168.1.101|
| Port     | 5000         |

## How to install?
```bash
user@hostname:~ $ git clone https://github.com/marcos-ro/vagrant-postgresql-13 && cd vagrant-postgresql-13 && vagrant up --destroy-on-error
```

## How access to VM?
```bash
user@hostname:~/vagrant-postgresql-13 $ vagrant ssh
```
