

#### В `Vagrantfile` две ВМ - `controlnode` и `server_centos`:
- `controlnode` - для запуска ansible.
- `server_centos` - ВМ, на которой разворачиваем стэк.

#### При инициализации ВМ на `server_centos` устанавливается python3.

#### Сеть по-умолчанию для ВМ - 192.168.56.0/24

#### Установка `Ruby` происходит через `rbenv` и занимает некоторое время (более 5 мин).

#### Команда `bundle install --clean  --no-cache --without development` выполняется **успешно**, однако ее вывод (предупреждение) ansible считает ошибкой. Сделал `ignore_errors: yes`

#### В файле /ets/hosts добавить
`192.168.56.101  ruby-app.com`
