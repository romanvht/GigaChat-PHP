# GigaChat PHP
Класс для общения с GigaChat сбера в PHP.

1. Закодируйте начения Client Id и Client Secret в Base 64, взятые из https://developers.sber.ru/studio/workspaces/
2. Полученый ключ добавьте в CLIENT_AUTH скрипта

Использование:
```
require __DIR__ . '/gigachat.php';
use neiro\Gigachat;

if($giga = gigachat::getInstance()){
  echo $giga::answer('Привет');
}
```

Для запроса картинок используется функция ```get_image()```, в ней следует изменить директорию сохранения изображений.
В функции ```answer()``` можно изменить формат вывода изображений в ответе
