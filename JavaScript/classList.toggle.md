[[JavaScript]]

Это происходит потому, что JavaScript выполняет всё в точности так, как мы ему сказали: берёт элемент `page` и сначала убирает класс `light-theme`, а после добавляет класс `dark-theme`. Так что при первом клике классы меняются и светлая тема переключается на тёмную, а при следующих кликах нашим инструкциям уже нечего делать: `dark-theme` уже есть — его не надо добавлять, а `light-theme` уже удалили — его больше не надо удалять.

Так как заставить темы переключаться при каждом клике? Веб-разработчикам часто приходится решать подобные задачи, и создатели JavaScript позаботились, чтобы чередовать классы можно было легко и удобно с помощью метода `classList.toggle`:

```
элемент.classList.toggle('класс');
```

Если класс у элемента есть, метод `classList.toggle` ведёт себя как `classList.remove` и класс у элемента убирает. А если указанного класса у элемента нет, то `classList.toggle`, как и `classList.add`, добавляет элементу этот класс.