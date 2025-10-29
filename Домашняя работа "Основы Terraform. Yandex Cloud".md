Ссылка на github репозиторий: 

# Задание 1. 
Cкриншот ЛК Yandex Cloud с созданной ВМ, где видно внешний ip-адрес:

<img width="1322" height="1265" alt="image" src="https://github.com/user-attachments/assets/d69b25ac-25b2-42e6-976a-00da3278b1b7" />

Скриншот консоли, curl должен отобразить тот же внешний ip-адрес:

<img width="1380" height="938" alt="image" src="https://github.com/user-attachments/assets/437f488c-f976-42be-bb4b-e21c99771209" />

Ответ на вопросы: 
Ошибки которые были исправлены в процессе выполнения домашней работы:

- Неправильные имена переменных в providers.tf
- Опечатка в platform_id
- Незакрытая фигурная скобка в variables.tf
- Неправильный cloud_id
- Ограничения платформы: core_fraction=5 → 20, cores=1 → 2

Параметры preemptible = true и core_fraction = 20:
preemptible = true - прерываемая ВМ, значительно дешевле core_fraction = 20 - ограничение CPU до 20%, снижает стоимость для учебных сред.
