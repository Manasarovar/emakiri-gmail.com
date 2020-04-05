# Lotsawa
Auto Formatter, Auto Translater Tibetan Text (http://emakiri.pythonanywhere.com/)
<br/>
#### Модуль 1 Текст (Python)
(можно протестировать по ссылке выше)<br/>
1.1 Форматирует тибетский текст (размечает: **заголовки, подзаголовки, цитаты, текст отличный от тибетского; 
  разбивает на абзацы**, внутренне размечает предложения для дальнейшего перевода)<br/>
<br/>
#### Модуль 2 Словарь (Python). 
2.1 Разбивает на слова<br/>
2.2 Ищет слово в словаре (db GVector) собирает найденные слова и все их значения в мини-Словарь.<br/>
2.3 Формирует файл вывода( можно посмотреть здесь - http://emakiri.pythonanywhere.com/)<br/>
<br/>
#### Модуль 3 Слово (JavaScript+Python)
3.1 Кликая по слову в тиб. тексте показывает карточку переводов слова.<br/>
3.1.1 Переводы имеют оценку в % по частоте встречаемости (в работе).<br/>
3.1.2 В карточке можно выбрать, уместный в данном контексте, перевод или **добавить свой перевод** (нажав `☸`) (добавленный перевод с тиб.ключем попадает в список 'Новая Пара' и `db GVector` и `00_NW.txt`)<br/>
3.1.3 Справа в окне 'Новая Пара' набрав `тибетское словосочетание=русский перевод` (нажав `☸`) **добавляется | заменяется (чекбокс замена) новая пара**, добавленная пара попадает в список 'Новая Пара' и `db GVector` и `00_NW.txt`)<br/>
3.1.4 Справа в окне 'Новая Пара' набрав `тибетское словосочетание` (нажав `☸`) **запрос словарной статьи из словаря** `db GVector`<br/>
<br/>
#### Модуль 4 Предложение (JavaScript+Python) 🙏
4.1 После выбора (в карточке слова) всех (хотя-бы одного) значений слов предложения, появляется **технический перевод предложения**, которое можно редактировать.<br/>
4.1.1 часть речи каждого слова (в разработке) <br/>
4.1.2 наиболее часто встречающийся перевод или собственный выбор из пункта 3.1.2 можно менять местами формируя технический перевод предложения. <br/>
4.1.3 Окно для литературного перевода предложения (можно выполнять, редактируя технический перевод).<br/>
4.1.4. Приемлемый вариант перевода предложения, вместе с тибетским оригиналом, (нажав `☸`) сохраняется в `db GVector` и `03_ST.txt` и присоединяется к Переводу Текста (в правом боковом окне).<br/>
4.1.5 Справа в окне 'Перевод Текста' набрав `отрывок тибетского текста` (нажав `☸`) получаем **разбор этого отрывка тибетского текста**<br/>
<br/>
#### Модуль 5 Кнопки Управления (JavaScript+Python)
5.1 Настройки: выбор пользователя и пр. (в разработке) <br/>
5.2 **Экспорт измененной БД** `db GVector` в `BackUpDB`<br/>
5.3 Навигация по страницам <br/>
5.4 **Каталог текстов** <br/>
