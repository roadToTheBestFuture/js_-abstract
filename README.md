# JS

MDN (Mozilla) JavaScript Reference – это справочник с примерами и другой информацией. Хороший источник для получения подробных сведений о функциях языка, методах встроенных объектов и так далее.


**Посмотреть, какие возможности поддерживаются в разных браузерах и других движках, можно в следующих источниках:**

- http://caniuse.com – таблицы с информацией о поддержке по каждой возможности языка. Например, чтобы узнать, какие движки поддерживают современные криптографические функции, посетите: http://caniuse.com/

- #feat=cryptography.
https://kangax.github.io/compat-table –



alert - показывает сообщение и ждет

В большинстве случаев новая строка подразумевает точку с запятой. Но «в большинстве случаев» не значит «всегда»!

Однострочные комментарии начинаются с двойной косой черты //.

Многострочные комментарии начинаются косой чертой со звёздочкой /* и заканчиваются звёздочкой с косой чертой */.

Директива выглядит как строка: "use strict" или 'use strict'. Когда она находится в начале скрипта, весь сценарий работает в «современном» режиме.
Позже мы изучим функции (способ группировки команд). Забегая вперёд, заметим, что вместо всего скрипта "use strict" можно поставить в начале большинства видов функций. Это позволяет включить строгий режим только в конкретной функции. Но обычно люди используют его для всего файла.

Для создания переменной в JavaScript используйте ключевое слово let.
Переменная – это «именованное хранилище» для данных. Мы можем использовать переменные для хранения товаров, посетителей и других данных.

В **JavaScript** есть два ограничения, касающиеся имён переменных:

1. Имя переменной должно содержать только буквы, цифры или символы $ и _.
2. Первый символ не должен быть цифрой.


Чтобы объявить константную, то есть, неизменяемую переменную, используйте const вместо let:
- *const myBirthday = '18.04.1982';*
Переменные, объявленные с помощью const, называются «константами». Их нельзя изменить. Попытка сделать это приведёт к ошибке:


В **JavaScript** есть 8 основных типов.

* <number> для любых чисел: целочисленных или чисел с плавающей точкой; целочисленные значения ограничены диапазоном ±(253-1).
*  <bigint> для целых чисел произвольной длины.
* <string> для строк. Строка может содержать ноль или больше символов, нет отдельного символьного типа.
* <boolean> для true/false.
* <null> для неизвестных значений – отдельный тип, имеющий одно значение null.
* <undefined> для неприсвоенных значений – отдельный тип, имеющий одно значение undefined.
* <object> для более сложных структур данных.
* <symbol> для уникальных идентификаторов.

 Оператор typeof позволяет нам увидеть, какой тип данных сохранён в переменной. 

* Имеет две формы: typeof x или typeof(x).
* Возвращает строку с именем типа. Например, "string".
* Для null возвращается "object" – это ошибка в языке, на самом деле это не объект.

*prompt*
показывает сообщение и запрашивает ввод текста от пользователя. Возвращает напечатанный в поле ввода текст или null, если была нажата кнопка «Отмена» или Esc с клавиатуры.

~~~

*/
 let age = prompt('Сколько тебе лет?', 100);

alert(`Тебе ${age} лет!`); // Тебе 100 лет! 
*/
~~~


Функция confirm отображает модальное окно с текстом вопроса question и двумя кнопками: OK и Отмена.

Результат – true, если нажата кнопка OK. В других случаях – false.

Например:

~~~

*/
let isBoss = confirm("Ты здесь главный?");

alert( isBoss ); // true, если нажата OK
*/

~~~