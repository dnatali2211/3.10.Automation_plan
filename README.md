# План автоматизации тестирования возможности записаться на обучение профессии «Тестировщик ПО»

## Сценарии навигации

### Сценарий №1 "Запись через `Каталог курсов` в хэдере сайта":
1. Открыть главную страницу сайта https://netology.ru/.
2. Нажать на кнопку `Каталог курсов` в хэдере сайта.
3. Из выпадающего списка выбрать категорию `Программирование` и нажать на нее.

<img width="1465" alt="SCR-20230726-tpfv" src="https://github.com/dnatali2211/3.10.Automation_plan/assets/127582824/b3d2a811-cadc-4175-88d8-a059f8a44611">

4. Найти в списке профессию `Тестировщик ПО` и нажать на нее.

<img width="1469" alt="Скрин2" src="https://github.com/dnatali2211/3.10.Automation_plan/assets/127582824/c127723c-ef0c-48b1-b3cb-99fab1371893">

5. На странице профессии нажать на кнопку `Записаться`.
6. В форме `Запишитесь на курс` ввести следующие данные:
  - в поле `Имя` ввести данные `Пётр`;
  - в поле `Номер телефона` ввести данные `+79216675431`;
  - в поле `Электронная почта` ввести данные `Test123@gmail.com`.
7. Нажать на кнопку `Записаться`.
8. Ожидаемый результат: отображается валидационное сообщение "Ваша заявка принята! В ближайшее время с Вами свяжется наш менеджер."
  
### Сценарий №2 "Запись через блок `Направления обучения`":
1. Открыть главную страницу сайта https://netology.ru/.
2. Прокрутить страницу до блока `Направления обучения`.
3. В этом блоке найти направление `Программирование` и нажать на него.
   
<img width="1464" alt="Скрин3" src="https://github.com/dnatali2211/3.10.Automation_plan/assets/127582824/f8563122-39dc-430e-a798-05576073914f">

4. Найти в списке профессию `Тестировщик ПО` и нажать на нее.
5. На странице профессии нажать на кнопку `Записаться`.
6. В форме `Запишитесь на курс` ввести следующие данные:
  - в поле `Имя` ввести данные `123`;
  - в поле `Номер телефона` ввести данные `+79216675431`;
  - в поле `Электронная почта` ввести данные `Test123@gmail.com`.
7. Нажать на кнопку `Записаться`.
8. Ожидаемый результат: отображается валидационное сообщение "Имя должно состоять из кириллических символов."

### Сценарий №3 "Запись через раздел `Обучение` в футере сайта":
1. Открыть главную страницу сайта https://netology.ru/.
2. В футере сайта в разделе `Обучение` выбрать направление `Программирование` и нажать на него.

<img width="1465" alt="SCR-20230727-jtvb" src="https://github.com/dnatali2211/3.10.Automation_plan/assets/127582824/bd87896d-0124-4b31-b74b-581286d54356">

3. Найти в списке профессию `Тестировщик ПО` и нажать на нее.
4. На странице профессии нажать на кнопку `Записаться`.
5. В форме `Запишитесь на курс` ввести следующие данные:
  - в поле `Имя` ввести данные `Сергей`;
  - в поле `Номер телефона` ввести данные `+0000000000000000`;
  - в поле `Электронная почта` ввести данные `Test123@gmail.com`.
7. Нажать на кнопку `Записаться`.
8. Ожидаемый результат: поле не позволяет ввести данные, отличные от маски и отображается валидационное сообщение "Неверный формат номера телефона.".

### Сценарий №4 "Запись через поисковую строку в `Каталог курсов` в хэдере сайта":
1. Открыть главную страницу сайта https://netology.ru/.
2. Нажать на кнопку `Каталог курсов` в хэдере сайта.
3. В поисковой строке `Какой курс Вам нужен?` ввести `тестировщик по`.

<img width="1464" alt="SCR-20230727-lmmc" src="https://github.com/dnatali2211/3.10.Automation_plan/assets/127582824/d043a55a-b10c-423f-9095-ef7c3cb1b66d">

4. На странице профессии нажать на кнопку `Записаться`.
5. В форме `Запишитесь на курс` ввести следующие данные:
  - в поле `Имя` ввести данные `Сергей`;
  - в поле `Номер телефона` ввести данные `+79216675431`;
  - в поле `Электронная почта` ввести данные `Test123gmail.com`.
6. нажать на кнопку `Записаться`.
7. Ожидаемый результат: отображается валидационное сообщение "Электронный адрес введен неверно!".

## Используемые инструменты

1. Среда разработки: IntelliJ IDEA, предоставляет богатый функционал для разработки и отладки Java-кода, предоставляет интеллектуальные подсказки и автодополнение кода, имеет интеграцию с системами контроля версий, что упрощает работу с кодом из репозиториев.
2. Браузер Chrome: обладает хорошей производительностью и стабильностью, что важно при выполнении автоматизированных тестов, а также имеет богатый набор инструментов разработчика (DevTools) для анализа и отладки веб-страниц.
3. Язык программирования Java,так как он предоставляет богатый выбор библиотек для автоматизации тестирования и имеет простой синтаксис.
4. Gradle: позволяет управлять зависимостями проекта, что упрощает установку и подключение необходимых библиотек и фреймворков.
Обладает гибкими возможностями для конфигурации сборки проекта. Имеет хорошую поддержку интеграции с другими инструментами и CI системами.
5. Фреймворк для юнит-тестирования JUnit: обеспечивает удобное написание и организацию тестовых сценариев. Предоставляет удобные методы для проверки ожидаемых результатов тестов.
6. Фреймворк для автоматизации Selenium WebDriver: позволяет выполнять различные действия с элементами страницы, взаимодействуя с ними как пользователь.
7. Faker: упрощает создание тестовых данных, включая случайные или заполненные тестовыми значениями поля формы. Помогает сгенерировать разнообразные тестовые данные для проверки различных сценариев.
8. Lombok: улучшает читаемость и поддерживаемость кода.
9. GitHub: обеспечивает централизованное хранение и контроль версий кода, что позволяет легко совместно работать над проектом. Предоставляет возможность отслеживать изменения, создавать задачи и исправлять ошибки через pull requests, создавать issue при обнаружении багов. Имеет возможности для автоматической интеграции с CI системами и автоматического запуска тестов при изменении кода.

## Необходимые разрешения

Необходимо получить разрешения владельцев сайта на проведение тестирования.
Доступ к тестовой базе данных при ее наличии.
Разрешение на создание и удаление тестовых данных.

## Возможные риски при автоматизации

Отсутствие тестовых меток в селекторах.
Частое обновление интерфейса.

## Необходимые специалисты

Автотестировщик.

## Интервальная оценка с учётом рисков в часах

При наличии рисков, указанных в разделе `Возможные риски при автоматизации`, необходимое количество рабочих часов - 40.
При их отсутствии - 24 рабочих часа.
