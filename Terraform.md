# Чек-лист готовности к домашнему заданию
<img width="1286" height="748" alt="image" src="https://github.com/user-attachments/assets/3133958e-dce5-47ab-9a52-0deefe9a060c" />

# Задание 1:

Перейдите в каталог src. Скачайте все необходимые зависимости, использованные в проекте.
<img width="1195" height="267" alt="image" src="https://github.com/user-attachments/assets/e3afcbc9-7ff5-4987-b1c0-3bc72b7c8546" />

Изучите файл .gitignore. В каком terraform-файле, согласно этому .gitignore, допустимо сохранить личную, секретную информацию?

Ответ: в файле personal.auto.tfvars

Выполните код проекта. Найдите в state-файле секретное содержимое созданного ресурса random_password, пришлите в качестве ответа конкретный ключ и его значение.

Ответ: 
"result": "EVvWi4TmKb2jyq2H"

Раскомментируйте блок кода, примерно расположенный на строчках 29–42 файла main.tf. Выполните команду terraform validate. Объясните, в чём заключаются намеренно допущенные ошибки. Исправьте их.

Ответ:

Добавил имя docker_image - nginx, удалил FAKE, исправил docker_container c "inginx" на "nginx" и еще...убран пробел в имени контейнера и поставлен дефис)
<img width="831" height="59" alt="image" src="https://github.com/user-attachments/assets/0875456d-3274-4af1-b02c-9dd1c1501f05" />

Выполните код. В качестве ответа приложите: исправленный фрагмент кода и вывод команды docker ps.

Ответ:

<img width="1511" height="1058" alt="image" src="https://github.com/user-attachments/assets/f215df1a-f53c-479e-8edb-039e269a97f8" />

Замените имя docker-контейнера в блоке кода на hello_world. Не перепутайте имя контейнера и имя образа. Мы всё ещё продолжаем использовать name = "nginx:latest". 
Выполните команду terraform apply -auto-approve. Объясните своими словами, в чём может быть опасность применения ключа -auto-approve. 

Ответ: 
Команда применяет изменения без подтверждения, что может привести к риску необратимых изменений в PROD

<img width="1525" height="1039" alt="image" src="https://github.com/user-attachments/assets/607f8758-d470-4532-8e1b-f957e81b23d1" />

Уничтожьте созданные ресурсы с помощью terraform. Убедитесь, что все ресурсы удалены. Приложите содержимое файла terraform.tfstate.

<img width="1583" height="648" alt="image" src="https://github.com/user-attachments/assets/77daf4fc-79a8-486d-a94d-3bed3cf66a4f" />

Образ nginx:latest не был удален потому что в конфигурации Terraform явно указан параметр keep_locally = true, 
который согласно документации провайдера docker предотвращает удаление образа при уничтожении ресурсов.

Домашнее задание закончено. 
Спасибо за проверку!







