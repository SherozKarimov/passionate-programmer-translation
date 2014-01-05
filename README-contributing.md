## Процесс перевода

Здесь работа найдётся человеку с любым уровнем подготовки!
Лишь бы у вас было желание помочь своим участием.

### Подготовка файлов с оригиналами текста для совместного перевода:

* copy/paste английского оригинала;
* убрать переносы (склеить слова);
* пофиксить `--` и `...` на "русский манер" (добавить пробелов по бокам, а в троеточиях -- после);
* постарайтесь перенести авторское выделение (италик по тексту)

А лучше скрипт(-ы) напишите, чтобы он помогал это делать. И положите в папку `./bin/`.

### Перевод. Оставляем билингву, чтобы с переводом могли поработать несколько переводчиков.

* У оригинала коротенькие параграфы, поэтому удобно вести билингву в одном файле:
  абзац оригинала, абзац перевода (разделены одной пустой строкой);
* между этими парами (оригинал + перевод) лучше ставить две-три пустые строки;
* когда над переводом поработает хотя бы 2 переводчика (а лучше больше) и придадут тексту
  вид художественного перевода, а не машинного -- билингву из файла убираем и оставляем
  только русский перевод.

Если вы переводчик и прошлись критическим взглядом по тексту или же активно с ним работали --
обязательно оставьте свою отметку в начале файла. Это поможет остальным ориентироваться
в том, насколько эта конкретная глава требует внимания. И чьего именно.

Предлагаю оставлять эту мета-информацию в самом начале файла, перед заголовком.
В виде обычного списка, с ником и кратким указанием того, что это было (основные
категории -- это перевод и вычитка; если хотите, можете детализировать). Например:

    - @urtica перевод
    - @rb2 перевод
    - @Flar49 перевод
    - @rb2 вычитка
    - @vpupkin вычитка
    - @abirvalg вычитка
    - @alov вычитка
    - @bilov вычитка
    - @vilov вычитка
    - @gilov вычитка
    - @dilov вычитка
    
    #### Глава 512. Не думай о белой обезьяне

Пожалуйста, не удаляйте билингву (оригинал), пока с текстом не поработают несколько переводчиков.
Пусть лучше этим вообще один человек занимается -- координатор перевода (@Flar49).
Когда уже понятно, что перевод достаточно хорош и в оригинал заглядывать уже не понадобится.


### Вычитка

* включаем спеллчекеры -- и вперёд. Делать это можно в любой момент, не дожидаясь окончания
  работы переводчиов и исчезновения билингвы из текста;
* обращайте внимание на букву "ё" пожалуйста. Нам её не хватает

* см. выше про метаинформацию. Если вычитали файл -- оставьте отметку об этом, пожалуйста.
  Даже если текст идеален и никаких правок не потребовалось - напишите: "вычитка, правок нет".
  Чем больше таких сигналов останется, тем легче будет понять, какая из глав уже дозрела
  и аж просится быть опубликованной.

  Возможно, сейчас это и не очень актуально, но если число переводов и участников вырастет,
  это поможет всем: и координатору перевода, и тем, кто хочет чем-либо помочь.



## Технические моменты (оформление, Markdown, Github)

* Заголовок главы начинаем с H4 (Markdown: `####`)
* в заголовке сохраняем номер главы: `#### 18. ....`
* в конце главы -- `##### Действуйте!` (H5)

* италик давайте оформлять `_подчёркиванием_`, а болд -- `**двойными звёздочками**`
* сноски (footnotes) -- см. пример в главе 17
* **если нужна краткая шпаргалка по Markdown** -- пишите, добавим (создайте в Issues задачу).
  А ещё лучше - наберите в гугле "markdown syntax", "markdown syntax cheatsheet", потратьте
  пол-часа и потом вставьте сюда несколько тех ссылок, которые показались вам наиболее удачными

* **если нужна краткая шпаргалка по гиту, гитхабу и пулл-реквестам** -- пишите, добавим (создайте
  в Issues задачу)
* не забывайте, что для внесения небольших исправлений и пожеланий вам необязательно работать
  с локальныым репозиторием или форком, разбираться с пулл-реквестами -- веб-интерфейс гитхаба
  позволяет редактировать тексты "на ходу"

### Координирование работ

Можно вносить планы и текущие задачи в README.
Другой вариант - создать по одной задаче на главу в разделе "Issues" гитхаба.
И там обсуждать возникающие вопросы и линковать к этой задаче относящиеся к данной главе коммиты.
Это мало волнует при текущей работе, зато оказывается очень удобно в будущем,
если возникает необходимость изучить, что происходило по этой задаче.

README за:

* задачи доступны оффлайн

README против:

* лог коммитов заполнен апдейтами README
* нет возможности связывать разные коммиты с одной задачей

ISSUES за:

* вся история работ по одной главе собирается в одном месте, достаточно лишь
  указывать в текстах коммитов номер задачи: `re #43 (ch15) вычитка, типографика`.

  Если ваш форк используется только для того, чтобы делать пулл-реквесты в основной
  репозиторий, то ваши собственные issues вам вряд ли нужны - тогда и путаницы не
  будет, можно указывать только короткую форму (номер задачи из репо @Flar49).

  Более универсально ссылаться полностью, но для данного репо запись получается
  очень длинной и неудобной. Хотя можно использовать многострочные комментарии:

        (ch15) вычитка, типографика

        re Flar49/passionate-programmer-translation#43

* не засоряется лог коммитов постоянными правками `README.md`
* уведомления о событиях в Issues приходят на email. Там же можно и ответить
* согласовывать публикацию глав на Хабре проще в Issues, а не правками README

ISSUES против:

* задачи доступны только онлайн. Способов полноценно работать с ними оффлайн я не знаю.

  Впрочем, это не означает, что их нет - могли появиться.
  Если найдёте - дайте знать (@rb2).
