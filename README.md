ИТОГОВЫЙ ПРОЕКТ ПО АВТОМАТИЗАЦИИ ТЕСТИРОВАНИЯ SKILLFACTORY QAP-1031

Задание:

В рамках выполнения дипломного проекта вам предстоит протестировать новый интерфейс авторизации в личном кабинете от заказчика Ростелеком Информационные Технологии. Вам предоставили требования к сайту, внимательно ознакомьтесь с ними перед началом работы.

Требования по проекту (.doc)
Объект тестирования: https://b2c.passport.rt.ru
Заказчик передал вам следующее задание:

Протестировать требования.
Разработать тест-кейсы (не менее 15). Необходимо применить несколько техник тест-дизайна.
Провести автоматизированное тестирование продукта (не менее 20 автотестов). Заказчик ожидает по одному автотесту на каждый написанный тест-кейс. Оформите свой набор автотестов в GitHub.
Оформить описание обнаруженных дефектов. Во время обучения вы работали с разными сервисами и шаблонами, используйте их для оформления тест-кейсов и обнаруженных дефектов. (если дефекты не будут обнаружены, то составить описание трех дефектов)
В процессе тестирования веб-страницы была создана таблица:

https://docs.google.com/spreadsheets/d/1PQu5lMK2r6UF7yjr816FDMOEn0BPtAlRC5f0WmWG4fE/edit?usp=sharing

где:

на листе Summary перечислены все проведенные проверки в рамках тестирования требований нового интерфейса страницы авторизации Ростелеком ИТ;
к каждой проверке представлены ссылки на тест-кейсы и/или баг-репорты, которые подробно расписаны на отдельных листах.
Сам код автотестов разделен на несколько логических блоков (блок авторизации, блок регистрации, блок восстановления пароля, блок авторизации по временному коду), что выражается комментарием в тройных кавычках. К каждому тесту написан комментарий, который поясняет, какой функционал проверяет тест.

Для начала работы с тестами необходимо:

Скачать репозиторий к себе на компьютер.
Скачать актуальный Selenium WebDriver с сайта: https://chromedriver.chromium.org/downloads (выбрать версию соответствующую версии вашего браузера).
Установить все необходимые пакеты, для установки необходимо ввести команду:
pip install -r requirements.txt
В файле test_task_28 в строке 12 указать путь расположения файла chromedriver.exe на вашем компьютере.
Для запуска тестов через терминал необходимо ввести команду:
pytest -v --driver Chrome --driver-path chromedriver.exe test_task_28.py
