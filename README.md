# PostgreSQL 13 on Debian Buster 10
## Requirements
| Name    | Description                                                                                                                                 |
|---------|---------------------------------------------------------------------------------------------------------------------------------------------|
| Docker  | Docker is an open platform for developing, shipping, and running applications.                                                              |
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
username@hostname:/path/to/repo> git clone https://github.com/marcos-ro/postgresql-13
username@hostname:/path/to/repo> cd postgresql-13
username@hostname:/path/to/repo/postgresql-13> vagrant up
```

## How access to VM?
```bash
username@hostname:/path/to/repo/postgresql-13> vagrant ssh
```
