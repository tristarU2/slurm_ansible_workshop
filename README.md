

#### В `Vagrantfile` две ВМ - `controlnode` и `server_centos`:
- `controlnode` - для запуска ansible.
- `server_centos` - ВМ, на которой разворачиваем стэк.

#### При инициализации ВМ на `server_centos` устанавливается python3.

#### Установка `Ruby` происходит через `rbenv` и занимает некоторое время (более 5 мин).


