#### Выполнить команду ls для файлов старше 30 дней по указанному пути
find /PathToDirectory -mtime +30 -exec ls -l {} \;

#### Выполнить команду rm для файлов старше 30 дней по указанному пути
find /PathToDirectory -mtime +30 -exec rm -f {} \;
