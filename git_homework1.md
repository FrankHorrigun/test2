# Шпаргалка по git и markdown
## Git commands

*git --version* - команда для проверки версии git

*git init* - инциализация пустого репозитория

*git status* - проверяем текущее состояние файлов

*git add имя_файла.расширение* - добавляем версионность файлу

*git commit -m "Message"* - команда фиксации изменений фалов

*git log* - вывод истории коммитов в хронологическом порядке

*git diff* - вывод изменений на текущий момент по отношению к последнему коммиту

*git add .* - добавляем версионность всем файлам в 

*git commit -am "Message"* - зафиксировать изменения всех файлов

*git checkout hash_коммита* - переход между версиями

*git checkuot master* - возврат к текущему состоянию

*git mv current_file_name.ext new_file_name.ext* - переименовать файл

**Важно: добавление файлов к «сохранению» двухступенчатое: сначала добавляем файл в индекс (git add), потом «сохраняем» (git commit).**



## Основные термины в git

Ключ к пониманию концепции git — знание о «трех деревьях»:

- Рабочая директория — файловая система проекта (те файлы, с которыми вы работаете).
- Индекс — список отслеживаемых git-ом файлов и директорий, промежуточное хранилище изменений (редактирование, удаление отслеживаемых файлов).
- Директория .git/ — все данные контроля версий этого проекта (вся история разработки: коммиты, ветки, теги и пр.).
 - Коммит — «сохранение» (хранит набор изменений, сделанный в рабочей директории с момента предыдущего коммита). Коммит неизменен, его нельзя отредактировать.

У всех коммитов (кроме самого первого) есть один или более родительских коммитов, поскольку коммиты хранят изменения от предыдущих состояний.

> @украдено с githuba
---
## Описание синтаксиса Markdown

### Заголовки

*#  Заголовок первого уровня*

*### Заголовок третьего уровня*

*###### Заголовок шестого уровня*

### Списки

Для формирования упорядоченных списков в качестве маркеров используются числа с точкой. Важной особенностью в данном случае является то, что сами номера, с помощью которых формируется список, не важны.

 Для формирования неупорядоченный списков используются такие маркеры, как звездочки, плюсы и дефисы.
 ### Горизонтальные линии (разделители)
Для того чтобы создать горизонтальную линию с использованием синтаксиса языка Markdown, необходимо поместить три (или более)дефиса или звездочки на отдельной строке текста. Между ними возможно располагать пробелы.
### Ссылки
Markdown поддерживает два стиля оформления ссылок:

 - Гиперссылка, с немедленным указанием адреса (внутритекстовая);
 - Гиперссылка, подобная сноске.

Подразумевается, что помимо URL-адреса существует еще текст ссылки. Он заключается в квадратные скобки. Для создания внутритекстовой гиперссылки необходимо использовать круглые скобки сразу после закрывающей квадратной. Внутри них необходимо поместить URL-адрес. В них же возможно расположить название, заключенное в кавычки, которое будет отображаться при наведении, но этот пункт не является обязательным.

[source:] [https://gist.github.com/Jekins/2bf2d0638163f1294637] (взято с этого источника)
### Выделение текста
Текст, окруженный одинарными символами, выделяется курсивным шрифтом, а текст, окруженный двойными символами, выделяется полужирным шрифтом. Также, выделенный фрагмент может находиться в любой части слова.
### Изображения
В Markdown существует 2 способа вставки изображений в документ:

1. С помощью непосредственного указания URL-адреса изображения. Синтаксис данной команды выглядит следующим образом:

    \!\[Альтернативный текст](/путь/к/изображению.jpg)
или

    \!\[Альтернативный текст](/путь/к/изображению.jpg "Подсказка")

Иными словами, он состоит из следующих элементов:

    -  знак;
    - квадратные скобки, в которых указывается альтернативный изображению текст (он станет содержимым атрибута в элементе img);
    - круглые скобки, содержащие URL-адрес или относительный путь изображения, а также (необязательно) всплывающую подсказку, заключённуе в двойные или одиночные кавычки.
2. С помощью метки-идентификатора. Синтаксис данной команды записывается следующим образом:

\!\[Альтернативный текст]\[id]

 - где «id» — имя определённой метки изображения. Метки изображений определяются при помощи синтаксиса, совершенно идентичного меткам гиперссылок:

[id]: путь/к/изображению "Необязательная подсказка"
Важной особенностью является то, что Markdown не позволяет задать размеры изображения (ширину, высоту).
### Дополнительные элементы
Может употребляться в Markdown перед специальными символами для того, чтобы они воспринимались в их буквальном (а не служебном) значении, такие как : \\, ', *, .

---

copyright: <https://gist.github.com/Jekins/2bf2d0638163f1294637>

**by FrankHorrigun** <<frankhorrigun@mail.ru>>

![**by FrankHorrigun**](/frank.png)

