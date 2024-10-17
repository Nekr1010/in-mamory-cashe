Пакет InMamoryCashe для реализацции быстрого доступа к данным из оперативной паяти

Примеры использования InMamoryCashe

Создаем контейнер с временем жизни по-умолчанию равным 7 минут и удалением просроченного кеша каждые 15 минут

`memcache := memorycache.New(5 * time.Minute, 15 * time.Minute)`

Установить кеш с ключем "myKey" и временем жизни 7 минут

`memcache.Set("myKey", "My value", 5 * time.Minute)`

Получить кеш с ключем "myKey"

`i := memcache.Get("myKey")`
