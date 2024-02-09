[[JavaScript]]
## [Инструкция «if»](https://learn.javascript.ru/ifelse#instruktsiya-if)

Инструкция `if(...)` вычисляет условие в скобках и, если результат `true`, то выполняет блок кода.

## [Блок «else»](https://learn.javascript.ru/ifelse#blok-else)

Инструкция `if` может содержать необязательный блок «else» («иначе»). Он выполняется, когда условие ложно.

let year = prompt('В каком году ?, '');

if (year < 2015) {
    alert('Слишком рано');
} else if (year > 2015) {
    alert('Это поздно');
} else {
    alert('Верно');
}

## [Условный оператор „?“](https://learn.javascript.ru/ifelse#uslovnyy-operator)

Иногда нам нужно определить переменную в зависимости от условия.

let age = prompt('Возраст?', 18);

let message = (age<3) ? 'Здравствуй, малыш':
    (age<18) ? 'Привет':
    age<100) ? 'Здравствуйте':
    'Какой необычный возраст';

alert(message);

## [Нетрадиционное использование „?“](https://learn.javascript.ru/ifelse#netraditsionnoe-ispolzovanie)

Иногда оператор «вопросительный знак» `?` используется в качестве замены `if`:

let company = prompt('Какая компания создала JavaScript?', '');

(company == 'Netscape') ?
    alert('Верно') : alert('Неправильно');


