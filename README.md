# project4
![Version][shield-version]
![Build status][shield-build]

Небольшой промо-сайт, рассказывающий “о точках притяжений” для визуальных путешествий внутри России. Сделан в рамках курса обучения на фронтенд-разработчика в Яндекс.Практикум.
## Стек: HTML, CSS (Flexbox + Grid), БЭМ.

### Что сейчас есть:
* Адаптивная и отзывчивая вёрстка под 6 разрешений
* Загрузка системных шрифтов, нескольких альтернативных форматов и оптимизация шрифтов
* Оптимизация изображений через сервисы tinypng.com, squoosh.app, jakearchibald.github.io/svgomg
* CSS анимация в секциях: video, additional, emblem

### Возможны добавления:
* Улучшить доступность сайта согласно a11y (tabindex (для навигации с клавиатуры))
* JS-открытие картинки (из photo-grid секции) на полный экран
* JS-галлерея на стороннем плагине с дополнительным функционалом (описание)
* JS-анимация (при наведении на карту курсора на неё появляется кружок города и спустя некоторое время 	от него отходят стилизованные круговые волны как от радио-передатчика)
* JS-перемотка (появляется когда долистываешь до конца сайта, квадратная кнопка в правом углу, с 	функционалом для перемотки к началу сайта)
* БЭМ для JS (модули на каждую фичу)
* ООП для каждого класса


### Использованные материалы и полезные для будущих изменений:

* [`Курс Яндекс.Практикум`](https://praktikum.yandex.ru/)
* [`Подключение шрифтов`](http://gearmobile.github.io/css/css-font-face/)
* [`Доступность a11y`](udacity.com/course/web-accessibility--ud891) <https://medium.com/web-standards/pragmatic-a11y-rules-b16dd2f77685>
* [`В HTML сделать имена файлов к альтернативным изображениям для поддержки Retina дисплеев`](webdesign.tutsplus.com/ru/tutorials/quick-tip-how-to-use-html5-picture-for-responsive-images--cms-21015)




## Инструкции по развёртыванию:

#### установить Git для вашей операционной системы
Его необходимо скачать с официального сайта <https://git-scm.com/downloads>

#### используя утилиту Git Bash
склонировать проект напрямую в свой репозиторий командой
```shell
git clone https://github.com/DmJavaScript/project4.git
```

установите все необходимые плагины с помощью автоматической пакетной установки,  для этого достаточно ввести команды
```shell
npm init --yes (перейдя в корневую папку репозитория, в одну из существующих веток, запустите эту команду инициализирующую библиотеку утилит NPM)
npm install  (используемые в проекте плагины подтянуться из списка установки файла package.json При желании вы можете изменить их список или установить более свежие версии плагинов. Для этого необходимо установить знак ^ (каретки) перед необходимыми плагинами в файле package.json Например, "cross-env": "^6.0.3",)
```


#### Полезно знать следующее:
Для запуска локальной сборки проекта необходимо в Git Bash ввести команду
```shell
npm run build  (cборка проекта скомпилируется в директории dist/) тогда Вы сможете отнести собранный проект и он запустится локально без дополнительных программ
```

Для работы с проектом в режиме разработки можете воспользоваться командой
```shell
npm run dev  (запускает локальный сервер разработки сайта с обновлениями изменений в реальном времени)
```

Для внесения изменений на уже развернутом проекте может использовать следующий алгоритм работы, команды
```shell
git checkout develop  (название ветки вашей разработки может быть другой, тут для примера, названа develop)
git pull origin develop  (актуализация информации по этой ветке)
git status (показывает какие файлы вы уже изменили и которые будут отправлены на сервер при следующих действиях)
git add .  (в очередь на загрузку ставятся все изменения, что Вы произвели в проекте! Это относится и к удаленным вами файлам)

git commit -m 'описываете здесь то, что добавили в очередь на загрузку'
git tag -a git v0.0.1 -m 'описание содержания версии коммита для внешних пользователей' (текст в дальнейшем можно будет отредактировать, важно ставить новер версий и соблюдать нумерацию. В последней части команды можно проставлять контрольную сумму или часть от неё)

git push origin develop   (запускаете процесс отправки подготовленных данных на сервер. Обращайте внимание на название ветки в которой произвдите изменения. Стоит develop в качестве примера)
git push origin v0.0.1    (отправьте своё описание версии на сервер. Если забыли это сделать, можно, но нежелательно делать это одной командой git push --tags  команда отправляет все неотправленные ранее теги на сервер)
```

финально страхуетесь командой
```shell
git pull origin develop (если всё в порядке, то придет ответ от сервера, что информация в актуальном состоянии)
```





## Минимальные системные требования:

Русский язык в операционной системе для правильного отображения шрифтов.

Компьютер с установленным на нём одним из перечисленных ниже браузеров.
Версии браузеров поддерживаются начиная от:
* edge: "17",
* firefox: "60",
* chrome: "64",
* safari: "10"


[shield-version]: https://img.shields.io/github/v/release/DmJavaScript/project4?style=flat-square
[shield-build]: https://img.shields.io/appveyor/ci/DmJavaScript/project4?style=flat-square
### ссылка на мой репозиторий https://github.com/DmJavaScript/project4