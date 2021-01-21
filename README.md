# Отчёт о тестировании KeyValidator

## Краткое описание

14.01.2021 - 14.01.2021 было проведено Функциональное тестирование KeyValidator на Windows 10 Pro 64bit.

На тестирование затрачено: ~ 60 минут.

В результате тестирования выявлены следующие дефекты:

 * [Некорректный вывод валидных ключей в приложении KeyValidator # 1](https://github.com/Aleksey-Bur/DZ1.1JAVA/issues/4)

 * [Некорректный вывод невалидных ключей в приложении KeyValidator # 2](https://github.com/Aleksey-Bur/DZ1.1JAVA/issues/5)

## Описание процесса тестирования

В процессе тестирования использовались следующие артефакты:

* Файл  [KeyValidator.class](https://github.com/netology-code/javaqa-homeworks/blob/master/intro/artifacts/KeyValidator.class)

* Файл [.gitignore](https://github.com/netology-code/javaqa-homeworks/blob/master/.gitignore)

В качестве тестовых данных использовалось Руководство использования KeyValidator :

Валидные ключи:

* 8f05e6a7-70e9-33d7-bfe7-b19eae0d8998
* 80b427f8-92cd-3aae-ba04-3927fbe17c6
* b295bc63-9f03-3b4b-af80-969b39f8c262
* 387eedc6-12e9-3b32-9881-63b6b5e85317
* c19a8cf9-5c3a-37c5-b7f3-d16d38a0c180

Невалидные ключи:

* 18252235-78e0-44a5-8720-556f0c7da17a
* e66075b6-ddad-445e-baf6-161b3289522b
* b6d53250-f07e-4352-a293-6102ddf7f1ca
* c2bc778a-1cb9-46c6-b435-0489649d2a42
* 2fb98b44-93e7-3bdd-a2ad-79347bfe4ad1

В результате работы вывод приложения будет выглядеть следующим образом:

* Result for 00000000-0000-0000-0000-000000000000: OK

* Result for 00000000-0000-0000-0000-000000000001: FAIL

где OK означает, что ключ валидный, FAIL - невалидный.

Тестирование производственного в следующем окружении:

* Устройство: Windows 10 Pro, 64-разрядная

* Браузер: Google Chrome Google Chrome Версия 87.0.4280.141,(64 бит)

* java: 11.0.9.1 2020-11-04

* файл KeyValidator.class.