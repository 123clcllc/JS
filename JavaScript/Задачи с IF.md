[[JavaScript]]
### [Перепишите 'if' в '?'](https://learn.javascript.ru/ifelse#perepishite-if-v)

Перепишите конструкцию `if` с использованием условного оператора `'?'`:
let result;

if (a+b<4) {
    result = 'Мало';
} else {
   result = 'Много';
}

result = (a+b<4) ? 'Мало' : 'Много';




Перепишите `if..else` с использованием нескольких операторов `'?'`.
let message;

if (login == 'Сотрудник'){
    message = 'Привет';
} else if (login == 'Директор') {
    message = 'Здравствуйте';
} else if (login == ' ') {
    message = 'Нет логина';
} else {
    message = ' ';
}


let message = (login == 'Сотрудник') ? 'Привет':
    (login == 'Директор') ? 'Здравствуйте':
    (login == ' ') ? 'Нет логина':
    ' ';

