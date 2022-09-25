- ВМ на CentOS 8
- при инициализации ВМ устанавливается python3. Далее, в hosts.ini указывается инетрпритатор для исполнения ansible
- переменные для запуска приложения в ansible/roles/ruby-app/tasks/main.yml
- переменные для запуска Postgres в ******************
- запуск playbook на localhost
- forward - localhost:80 --> 8888
- при запуске vagran установить сразу все роли ansible !!!!
- galaxy nginx - https://galaxy.ansible.com/nginxinc/nginx
- установть плагины, тпа postgres

Установить модули:
- ansible-galaxy collection install community.general
- 