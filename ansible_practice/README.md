# Практикум по Ansible:

Выполнение практического задания:

Локально запущена контролнода на Ubuntu через Vagrant, удалённая вируалка CentOS в Vultr.com.
В связи с EOL Centos7 реп использовал таргетную виртуалку на Centos 9.
Решило проблемы с недоступностью реп для установки пакетов, возможно создало новые проблемы. 

# Прогресс

- Запуск приложения почти проходит. вместо упомянутых пакетов ставятся центосные item=gcc libxml2-devel. есть ошибки 
TASK [dependencies : Configure application bundle for nokogiri] *****************************************************************************************************************fatal: [45.76.95.174]: FAILED! => {"changed": false, "cmd": "/home/vagrant/app bundle config build.nokogiri --use-system-libraries", "msg": "[Errno 13] Permission denied: b'/home/vagrant/app'", "rc": 13, "stderr": "", "stderr_lines": [], "stdout": "", "stdout_lines": []}
- бд установлена запущена postgres (PostgreSQL) 13.14
- вебсервер запущен, но конфиг jinja скопирован, частично избавился от энвов т.к. не получилось их использовать. 