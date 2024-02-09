[[JavaScript]]
после того, как пользователь заполнит и отправит форму подписки, на странице должно появиться сообщение:

```
Адрес e-mail добавлен в список получателей рассылки.
```

И для начала разберёмся, где именно пользователи увидят сообщение. Верстальщик для этого выделил элемент с классом `subscription-message`. Сейчас в нём уже есть текст: «Обещаем присылать вам новости не чаще одного раза в день, причём только самые интересные и важные». Когда пользователь отправит форму, вместо этого текста должно появиться сообщение об удачной подписке. Получается, нам нужно найти элемент, удалить из него старый текст, а после вставить новый. Как это сделать из скрипта? С помощью свойств элемента.

У каждого элемента имеется множество свойств: его размеры, цвет и так далее. Свойство `textContent` хранит в себе текстовое содержимое элемента.

Допустим, у нас есть абзац:

```
<p>Я текст!</p>
```

С помощью `textContent` мы можем получить текстовое содержимое этого абзаца, чтобы, к примеру, вывести его в консоль:

```
let paragraph = document.querySelector('p');
console.log(paragraph.textContent);
```

В результате в консоли появится сообщение `Я текст!`

Давайте проверим, как работает `textContent`. Для этого сохраним в переменную элемент `subscription-message` и выведем в консоль его текстовое содержимое.