# Playbooks RMS

Ansible playbooks для курса Ruby Microservices.

# Зависимости

+ Ansible `2.9+`

# Playbooks

+ `postgresql.yml`
+ `rabbitmq.yml`
+ `nginx.yml`
+ `setup.yml`

# Установка и запуск playbooks

1. Склонируйте репозиторий:

```
git clone git@github.com:avbelyshev/playbooks-rms.git && cd playbooks-rms
```

2. Укажите хосты в файле `hosts`

3. Определине переменные окружения для доступа к Docker Registry:

+ `DOCKER_USER`
+ `DOCKER_PASSWORD`

4. Создайте файл `secrets.yml` с содержимым:

```
postgresql_password=<postgresql_password>
rabbitmq_password=<rabbitmq_password>
```

5. Запустите playbook

```
ansible-playbook <playbook_name>.yml
```
