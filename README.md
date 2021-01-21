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

## How VM up?
```bash
user@hostname:~ $ git clone https://github.com/marcos-ro/vagrant-postgresql-13
user@hostname:~ $ cd vagrant-postgresql-13
user@hostname:~/vagrant-postgresql-13 $ vagrant up
```

## How access to VM?
```bash
user@hostname: ~/vagrant-postgresql-13 $ vagrant ssh
```
