#### Статус сетевых интерфейсов
```
nmcli dev status
```

### Изменение параметра NAME и DEVICE

#### Редактирование конфигурации сетевого интрефейса
```
nmcli con edit ConnectionName
```

#### Отобразить текущую конфигурацию
```
print
```

#### Изменить параметр connection.id (NAME)
```
set connection.id = ConnectionName
```

#### Изменить параметр connection.interface-name (DEVICE)
```
set connection.interface-name = DeviceName
```

#### Проверка конфигурации
```
verify
```

#### Сохранение конфигурации
```
save
```

#### Выход из редактора конфигурации
```
quit
```

#### Показать текущие DNS сервера
```
( nmcli dev list || nmcli dev show ) 2>/dev/null | grep DNS)
```
