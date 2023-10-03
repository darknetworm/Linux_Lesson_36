# Linux_Lesson_36
## VLAN, LACP
### Описание репозитория
Лабораторный стенд для тестирования VLAN и LACP. Все файлы и структуру директории ansible необходимо скопировать в общую директорию.  
![scheme](https://github.com/darknetworm/Linux_Lesson_36/assets/82410807/e10f6692-38d8-4509-a7b9-21500e65977d)  

- **Vagrantfile** - создает три маршрутизатора на основе CentOS 8, тестовый сервер и клиентский хост на основе CentOS 8 и тестовый сервер и клиентский хост на основе Ubuntu 20.04. Настройка функциональности виртуальных машин производится с помощью Ansible.  
- директория **/ansible** содержит файлы для настройки виртуальных машин с помощью Ansible, в этой директории расположены основные файлы:  
- **ansible/provision.yml** - основной файл Ansible playbook для установки и настройки сетевых устройств стенда.  
- **ansible/hosts** - файл с настройками компьютеров для быстрого доступа к ним из playbook.  
- остальные файлы в директории осуществляют настройку интерфейсов vlan (на серверах и хостах) и bond (между интернет и центральным маршрутизаторами).

---

### Проверка работоспособности стенда

![office1](https://github.com/darknetworm/Linux_Lesson_36/assets/82410807/14bbadaa-b895-4a36-859e-7c0e5385f818)

![office2](https://github.com/darknetworm/Linux_Lesson_36/assets/82410807/2cccbaa1-22d8-4217-b3e1-6c7d0dad0bba)

![bond](https://github.com/darknetworm/Linux_Lesson_36/assets/82410807/5e722450-9c56-4419-bd8a-8af72ca4ccdc)
