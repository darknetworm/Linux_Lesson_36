# Linux_Lesson_36
## VLAN, LACP
### Опсание репозитория
Лабораторный стенд для тестирования VLAN и LACP. Все файлы и структуру директории ansible необходимо скопировать в общую директорию.
![scheme](https://github.com/darknetworm/Linux_Lesson_36/assets/82410807/e10f6692-38d8-4509-a7b9-21500e65977d)

- **Vagrantfile** - создает три маршрутизатора на основе CentOS 8, тестовый сервер и клиентский хост на основе CentOS 8 и тестовый сервер и клиентский хост на основе Ubuntu 20.04. Настройка функциональности роутеров производится с помощью Ansible.  
- директория **/ansible** содержит файлы для настройки виртуальных машин с помощью Ansible, в этой директории расположены основные файлы:  
- **ansible/provision.yml** - основной файл Ansible playbook для установки и настройки сетевых устройств стенда.  
- **ansible/hosts** - файл с настройками компьютеров для быстрого доступа к ним из playbook.  
- остальные файлы в директории осуществляют настройку интерфейсов vlan (на серверах и хостах) и bond (между интнрнет и центральным маршрутизаторами).
