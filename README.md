# booksearch
Задание заключается в разработке веб-приложения для поиска текста в базе данных книг и
оповещения о результатах поиска по электронной почте.

Основные характеристики веб-приложения:
– состоит из клиентской и серверной частей;
– клиентская часть ― простая форма из поля для ввода искомого текста, поля для ввода
      адреса электронной почты, на который будет отправлен результат поиска, и кнопки
запуска;
– серверная часть использует какой-либо Python-фреймворк: Django, Pyramid, Tornado,
      Flask, Bottle или др.;
– хранилище книг ― любая подходящая реляционная или нереляционная база данных: MySQL,
      PostgreSQL, Redis, MongoDB, Riak или др.;
– поиск текста происходит за произвольное время, которое записывается в лог-файл
приложения;
– результат поиска содержит названия книг, частей/разделов/глав и номеров страниц, на
      которых встречается искомый текст.
Алгоритм работы веб-приложения:
   1. Пользователь вводит искомый текст в поле поиска, указывает свой электронный адрес,
      нажимает кнопку запуска процесса поиска.
   2. На сервере начинается поиск текста в базе данных книг и возвращается страница с
      сообщением о начале поиска, а также информацией куда будет отправлен результат.
   3. Список книг, в которых найден текст, с дополнительной информацией
      (части/разделы/главы, номера страниц) формируется в процессе поиска.
   4. Результат поиска отправляется в виде электронного письма пользователю на его
      электронный адрес.
Опционально:
Веб-приложение позволяет пользователю указывать предел времени поиска текста в базе
данных книг, по достижению которого происходит отправка неполного результата поиска.
