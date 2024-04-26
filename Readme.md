Заголовки

# H1 Заголовок первого уровня
## H2  Заголовок второго уровня 
### H3  Заголовок третьего уровня
#### H4  Заголовок четвёртого уровня
##### H5  Заголовок пятого уровня
###### H6  Заголовок шестого уровня

Можно подчеркнуть H1 и H2:

At-H1
======

Alt-H2
------

Выделение

Курсив обозначается *звездочками* или _подчеркиванием_.
Полужирный шрифт - двойными **звездочками** или двойным _подчеркиванием_.
Комбинированное выделение **звездочками и _подчеркиванием_**.
Для зачеркнутого текста используются две тильды. ~~Зачеркнуто.~~

Списки
(В данном примере предшествующие и завершующие пробелы обозначены точками:⋅) 

• - alt+0149 
· - alt + 0183 

1. Первый пункт нумерованного списка
2. Второй пункт
  * Нумерованный вложенный список
4. И еще один пункт.

   ···Внутри пунктов списка можно вставить абзацы с таким же отступом.Обратите внимание на пустую строку выше и на пробелы в начале (нуден по меньшей мере один,но здесь добавлены три, чтобы выровнять необработанный Markdown).

   ···Чтобы вставить разрыв строки, но не начинать новый параграф, нужно добавить два пробела перед новой строкой.··
   ···Этот текст начинается с новой строки, но находится в том же абзаце.··
   ···(В некоторых обработчиках, например Github, пробелы в начале новой строки не нужны.)

* Ненумерованный список можно размечать звездочками
- Или минусами
+ Или плюсами

Ссылки 

Ссылки можно оформить разными способами.
[Обычная ссылка в строке](https://www.google.com)
[Обычная ссылка с title](https://www.google.com "Сайт Google")
[Ссылка со сноской](Произвольный регистронезависимый текст)
[Относительная ссылка на документ](../blob/master/LICENSE)
[Для ссылок со сноской можно использовать цифры][1]
Или можно просто вставить ссылку в квадрвтные скобки [текст ссылки]
Произвольный текст, после которого можно привести ссылки.

[произвольный регистрнеозависимый текст]: https://www.mozilla.org
[1]: http://slashdot.org
[текст ссылки]: http://www.reddit.com

Изображения

Вот наш логотип (навести указатель,чтобы увидеть текста заголовка):

Внутри строки:
![alt-текст](https://github.com/adam-p/markdown-here/raw/master/src/common/images/icon48.png "Текст заголовка логотипа 1")

В сноске:

![alt-текст][logo]

![logo](https://github.com/adam-p/markdown-here/raw/master/src/common/images/icon48.png "Текст заголовка логотипа 2")

Код и поверка синтаксиса

Блоки кода являются частью функции Markdown, но не подсветка синтаксиса.Однако многие обработчики, например Github или *Markdown Here*, поддерживает подсветку синтаксиса.Список поддерживаемых языков и способ их указания может различаться.*Markdown Here* поддерживает десятки языков (и не-языков, например синтаксис diff и заголовки HTTP);полный список и способ указания языков см. на странице [highlight.js demo-странице](https://highlightjs.org/not-a-cdn)

`Код` в строке обрамляется `обратными апострофами`.

Блоки кода выделяются либо тремя обратными апострофами ``` либо четырьмя пробелами в каждой строке.Рекомендуется использовать три апострофа -- они проще и только они поддерживают подсветку синтаксиса.

```javascript
var s = "Подсветка JavaScript";
alert(s);
```

```python
s = "Подсветка Python"
print s
```

```
Язык не указан ,синтаксис не подсвечен.
Но мы вставим в него <b>тег</b>.
```
Таблицы

Таблицы не яаляются частью Markdown, но многие обработчики, например Markdown Here и Github, поддерживают их. Они позволяют легко добавить таблицы в электронное письмо -- в других случаях для этого нужно копировать их из другого приложения.

Вертикальные линии обозначают столбцы.

| Таблицы       | Это                | Круто |
| ------------- |:------------------:| -----:|
| столбец 3     | выровнен вправо    | $1600 |
| столбец 2     | выровнен по центру |   $12 |
| зебра-строки  | прикольные         |    $1 |

Внешние вертикальные линии (|) не обязательны, и они нужны только чтобы сам код Markdown выглядел красиво. Тот же код можно записать так:

Markdown| не такой | красивый 
--- | --- | ---
*Но выводится* | `так же` | **клёво**
1 | 2 | 3

Цитаты

> C помощью цитат очень удобно в письме обозначать исходный текст.
> Эта строка - часть той же цитаты.

Разрыв цитаты.
> Это очень длинная строка, но она будет правильно процитирована даже при размещении на нескольких строках. Продолжаем писать, чтобы эта строка не вмещалась на одной строке в любом окне. Кстати, в цитаты можно такжэ размечать с помощью Markdown.

Встроенный HTML 

Часто Markdown понимает чистый HTML.

<dl>
  <dt>Список определений</dt>
  <dd>Это то, что люди иногда используют.</dd>

  <dt>Markdown внутри HTML</dt>
  <dd>Работает *не очень** хорошо. Используйте HTML-<em>теги</em></dd>
<dl> 

Горизонтальные линии

Три и более...

---

Дефисы

***

Звёздочки 

___

Подчёркивания

Новая строка 

Для понимания работы разрыва строки автор главным образом рекомендует эксперементировать и пробовать -- нажмите <Enter> один раз (т.е перейдите на новую строку), потом нажмите дважды (т.е вставьте две новые строки) и посмотрите что произошло.Вы сразу поймете что вам нужно. В расширении Markdown here для браузеров есть удобная функуция "Markdown Toggle", которая поможет в этом.

Примечания переводчика:
Для переноса на новую строку в конце предыдущей строки необходимо добавить два пробела.Без этого большинство парсеров Markdown не выполняют пререход на новую строку.

Попробуйте ввести следующее:

Это начальная строка


Эта строка отделена от предыдущей двумя новыми строками и станет *отдельным абзацем*.


Это тоже отдельный абзац, но...  
Эта строка отделена одной новой строкой, поэтому она находится в *том же абзаце*.

Видео Youtube

Ролики нельзя вставить напрямую, но можно вставить изображение со ссылкой на видео, например:

<a href="http://www.youtube.com/watch?feature=player_embedded&v=ID_ВИДЕОРОЛИКА_НА_YOUTUBE" target="_blank"><img src="http://img.youtube.com/vi/ID_ВИДЕОРОЛИКА_НА_YOUTUBE/0.jpg" 
alt="ALT-ТЕКСТ ИЗОБРАЖЕНИЯ" width="240" height="180" border="10" /></a>

На чистом Markdown, но без размеров изображения и рамки:
[![ALT-ТЕКСТ ИЗОБРАЖЕНИЯ](http://img.youtube.com/vi/ID_ВИДЕОРОЛИКА_НА_YOUTUBE/0.jpg)](http://www.youtube.com/watch?v=ID_ВИДЕОРОЛИКА_НА_YOUTUBE)




