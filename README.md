# Chek_root_processes

Это простой скрипт на Bash предназначен для сбора информации о том какие процессы запущенны на хостах, подключение по SSH. Требуется указать логин технической учётной записи, предполагается что для аутентификации используются сертификаты.
В файл nods передаються ip хостев для проверки
Скрипт формирует следуюшую файловую структуру при сконировании: 
.
├── logi_11_07_2023
│   ├── 192.168.1.10.log
│   ├── 192.168.1.200.log
│   └── error_.log
├── nods
└── skript
соответственно при ежедневном сканировании будут создаваться новые директории logi_DD_MM_YYYY.
В папке error_.log приведены хосты к которым не удалось подключиться и код ошибки.
