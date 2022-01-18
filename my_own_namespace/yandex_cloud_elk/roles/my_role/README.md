My_role
=========

Роль для тестирования коллекций ansible

Requirements
------------

Тестирование осуществлялось на ubuntu 20.04 
Вероятно, поддерживаться будет в большинстве unix-подобных системах (но это не точно)

Role Variables
--------------

| Variable name | Default | Description |
|-----------------------|----------|-------------------------|
| test_path | "/tmp/test_remote_01.txt" | Параметр, определяющий путь для нового файла, а также имя нового файла |
| test_content | "Test module in task\nHello, netology!\n" | Строка, которая записывается в новый файл |


Example Playbook
----------------

---
- name: Test my_own_module in yandex.cloud
  hosts:
    - ubuntu-ansible
  roles:
    - my_role
