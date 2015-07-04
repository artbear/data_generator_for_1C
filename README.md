# generating_data_for_1C
Генератор данных (1С 8)
 
Используется в сочетании с обработкой xddTestRunner.epf из проекта [xDrivenDevelopment/xUnitFor1C] (https://github.com/xDrivenDevelopment/xUnitFor1C)

Имеет экспортный метод СоздатьДанныеПоТабличномуДокументу(Макет), который явлется альтернативой одноименного метода упомянутой обработки.

Достоинства:
- более наглядная и простая структура данных
- компактное описание данных
- поддерживается генерация объектов следующих типов: таблица значений, структура, ссылочные типы
- поддерживается возможность задавать в макете формулу, которая расчитывается через функцию "Вычислить()". Это удобно, например, когда нужно поместить в таблицу значение константы, текущего пользователя, вид движения накопления, предопределенный элемент справочника и т.д. Формула начинается со знака "="

Недостатки:
- корректно работает только в пустой базе


Рабочий пример генерации набора данных в обработке "tests\Пример Обработка размещение резервов по заявкам.epf"

Все поддерживаемые типы генерируемых данных в макетах обработки "tests\Тест Генератор данных.epf". Она запускается в конфигурации "tests\Конфигурация для тестирования Генератора данных.cf"
