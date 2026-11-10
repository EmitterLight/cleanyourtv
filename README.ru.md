<p align="center">
  <a href="https://cleanyour.tv"><img src="https://raw.githubusercontent.com/Gathin23/cleanyourtv/main/docs/banner.png" alt="CleanYourTV. Ваш телевизор без рекламы. Удалите предустановленное ПО с любого телевизора на Android TV или Google TV по Wi-Fi и замените переполненный рекламой главный экран на чистый лаунчер, который выглядит как Apple TV. Без root-прав, без кабеля, ничего не удаляется, и восстановление одной командой." width="800"></a>
</p>

<p align="center">
  Читать на: <a href="README.he.md" lang="he" dir="rtl">עברית</a> · <a href="README.zh-CN.md">简体中文</a> · <a href="README.zh-TW.md">正體中文</a> · <a href="README.vi.md">Tiếng Việt</a> · <a href="README.ja.md">日本語</a> · <a href="README.it.md">Italiano</a> · <a href="README.pt-BR.md">Português</a> · <a href="README.nl.md">Nederlands</a> · <a href="README.de.md">Deutsch</a> · <a href="README.uk.md">Українська</a> · <a href="README.tr.md">Türkçe</a> · <a href="README.uz.md">Oʻzbekcha</a>
</p>

<p align="center">
  <a href="https://github.com/Gathin23/cleanyourtv/stargazers"><img src="https://img.shields.io/github/stars/Gathin23/cleanyourtv?style=flat&cacheSeconds=1800&color=cfffcf&labelColor=15181e" alt="Stars"></a>
  <a href="https://github.com/Gathin23/cleanyourtv/pulls?q=is%3Amerged"><img src="https://img.shields.io/github/issues-search?query=repo%3AGathin23%2Fcleanyourtv%20is%3Apr%20is%3Amerged&style=flat&cacheSeconds=1800&label=merged%20PRs&color=cfffcf&labelColor=15181e" alt="Merged PRs"></a>
  <a href="https://github.com/Gathin23/cleanyourtv/network/members"><img src="https://img.shields.io/github/forks/Gathin23/cleanyourtv?style=flat&cacheSeconds=1800&color=cfffcf&labelColor=15181e" alt="Forks"></a>
  <a href="https://github.com/Gathin23/cleanyourtv/graphs/contributors"><img src="https://img.shields.io/github/contributors/Gathin23/cleanyourtv?style=flat&cacheSeconds=1800&color=cfffcf&labelColor=15181e" alt="Contributors"></a>
  <a href="https://buymeacoffee.com/gathint"><img src="https://img.shields.io/badge/support-%E2%9D%A4-ff5e8a?style=flat&labelColor=15181e" alt="Support, buy me a coffee"></a>
  <a href="https://www.producthunt.com/products/cleanyourtv"><img src="https://img.shields.io/badge/Product%20Hunt-upvote%20%E2%96%B2-da552f?style=flat&logo=producthunt&logoColor=white&labelColor=15181e" alt="CleanYourTV on Product Hunt"></a>
</p>

<p align="center">
  <a href="https://trendshift.io/repositories/310225"><img src="docs/trending-badge.png" alt="#1 trending repo of the week, Oct 19–25 2026, via trendshift.io" width="360"></a>
</p>

<p align="center">
  <a href="docs/PRESS.md"><img src="docs/card.jpg" alt="463 модели телевизоров · 124 бренда · 31 язык · лаунчер на 572 КБ. Освещено в TechCrunch, TechRadar, Tom's Guide, Mashable, Android Authority, XDA, FlatpanelsHD, It's FOSS, Phandroid, GIGAZINE, Xataka, WinFuture, Frandroid, Macitynet, Techaeris, TechPP и ещё 518 изданиях: 534 статьи из 57 стран. До: стандартный главный экран Google TV со спонсируемой рекламой. После: лаунчер Clean Your TV." width="800"></a>
</p>

## Начните здесь

| У вас есть | Перейдите к |
|---|---|
| **Android TV или Google TV** | [Быстрый старт](#quick-start): помощник по программированию выполнит работу примерно за пятнадцать минут. |
| **Телевизор Samsung, LG, Roku, Vizio или Hisense VIDAA** | [cleanyour.tv/not-android](https://cleanyour.tv/not-android): CleanYourTV там не работает, но вы можете отключить отслеживание с помощью пульта. |
| **Телефон или ноутбук, без помощника по программированию** | Одно из [приложений сообщества](https://cleanyour.tv/app) для телефонов Android, Mac и Windows, созданных независимыми разработчиками. |
| **Хотите сначала увидеть** | [Что вы получите](#what-you-get): скриншоты нового главного экрана. |

**Официальные ссылки:** [cleanyour.tv](https://cleanyour.tv) и этот репозиторий. Другие домены, использующие это имя, например cleanyourtv.com, не управляются этим проектом ([#1004](https://github.com/Gathin23/cleanyourtv/issues/1004)). CleanYourTV не публикует приложения ни в одном магазине приложений, и clean-your-tv.net также не наш.

[Как это работает](#how-it-works) · [Быстрый старт](#quick-start) · [Что вы получите](#what-you-get) ·
[Поддерживаемые телевизоры](#supported-tvs) · [Сделать вручную](#doing-it-by-hand) · [Лаунчер](#the-launcher) ·
[Восстановление](#restoring-your-tv) · [Обновления прошивки](#after-a-firmware-update) ·
[Вопросы](#questions-people-ask) · [Участие в разработке](#contributing)

<a id="how-it-works"></a>
## Как это работает

Телевизоры Android имеют тот же отладочный мост, что и телефоны Android. Включите отладку по USB в параметрах разработчика на телевизоре, один раз разрешите доступ вашему компьютеру, а остальное — стандартные инструменты Android:

| Шаг | Что происходит |
|---|---|
| **Резервное копирование** | Список установленных пакетов и настроек. |
| **Отключение** | Телеметрия производителя, рекламные сервисы, контентные ряды и предустановленный мусор с помощью `pm disable-user`. Ничего не удаляется, поэтому скрипт восстановления может отменить каждый шаг. |
| **Установка** | Небольшой нативный лаунчер, назначенный главным экраном по умолчанию. |

**Без root-прав, без кабеля, ничего не удаляется, и восстановление одной командой, если вы передумаете.**

Предустановленное ПО отличается в зависимости от бренда, поэтому в промпте ваш помощник по программированию обнаружит его на вашем телевизоре и спросит, прежде чем трогать что-то, что вы, возможно, используете.

<a id="quick-start"></a>
## Быстрый старт

| У вас есть | Сделайте это |
|---|---|
| **Компьютер** | Используйте промпт с помощником по программированию: три шага ниже. |
| **Компьютер, без помощника по программированию** | Выполните три шага самостоятельно: команды приведены в разделе [Сделать вручную](#doing-it-by-hand). |
| **Телефон или ноутбук, без помощника по программированию** | Выберите одно из [приложений сообщества](https://cleanyour.tv/app): бесплатные приложения с открытым исходным кодом, созданные независимыми разработчиками на основе этих списков телевизоров. |

Три шага ниже написаны для помощника по программированию: компьютер должен находиться в той же сети Wi-Fi, что и телевизор, иметь оболочку, а также Python 3, JDK с 17 по 22 и Android SDK platform 34 с build-tools 34 (помощник собирает лаунчер там). Без помощника [Сделать вручную](#doing-it-by-hand) — это та же работа, выполняемая вами, и там есть команды установки.

Подойдет любой из этих инструментов: Claude Code (на [0G Private Computer](https://pc.0g.ai/?utm_source=cleanyourtv&utm_medium=github&utm_campaign=readme) или в [плане Anthropic](https://claude.com/pricing)), [Codex](https://github.com/openai/codex), [Gemini CLI](https://github.com/google-gemini/gemini-cli), [Antigravity CLI](https://antigravity.google/product/antigravity-cli) или [DeepSeek Harness](https://github.com/deepseek-ai/deepseek-harness).

| Где | Что делать |
|---|---|
| **1. На телевизоре** | Настройки → Настройки устройства → О телевизоре → нажмите OK на **Сборка** семь раз → назад → Параметры разработчика → **Отладка по USB** включена. Если вы видите переключатель сетевой отладки или отладки ADB, включите и его. Держите телевизор включенным. |
| **2. На вашем компьютере** | Клонируйте репозиторий и откройте эту папку в вашем помощнике (`git clone https://github.com/Gathin23/cleanyourtv`), затем вставьте [`PROMPT.md`](PROMPT.md) и укажите модель вашего телевизора. |
| **3. Следуйте инструкциям** | Примите «Разрешить отладку по USB?» на телевизоре, затем ответьте на контрольный список: какие приложения вы используете, размер дока и порядок приложений, сохранять ли голосового помощника, Chromecast и обновления. |

Клонирование важно: помощник повторно использует `tools/disable.sh` и `launcher/build-and-install.sh` из этого репозитория вместо того, чтобы писать свои собственные, и именно там хранятся резервная копия, защита Home и запись восстановления.

Помощник создает резервную копию, удаляет bloatware, собирает и устанавливает лаунчер, а также проверяет каждый шаг с помощью скриншотов, полученных с телевизора. С этим репозиторием в качестве контекста это занимает около пятнадцати минут.

<a id="what-you-get"></a>
## Что вы получите

Главный экран, который выглядит как Apple TV и не мешает:

| Часть | Как это выглядит |
|---|---|
| **Совершенно черный главный экран** | Док из четырех ваших любимых приложений в закругленной полосе, там, где его размещает Apple TV. |
| **Верхняя полка** | Крупным шрифтом называет приложение в фокусе, с окружающим свечением цвета, взятого из его обложки. |
| **Остальные ваши приложения в сетке** | Выезжает вверх при нажатии вниз. |
| **Один плавающий стеклянный блик** | Перепрыгивает от плитки к плитке. Плитка в фокусе приподнимается и показывает свое название. |
| **Три матовые кнопки** | Входы (порты HDMI под именами, которые вы им дали в настройках телевизора, AV, Live TV), Wi-Fi или Ethernet с именем сети, Настройки. |
| **Приветствие, тонкие часы и дата** | Шрифтом [Outfit](https://fonts.google.com/specimen/Outfit) и соответствующая заставка часов. Установите `show_stats` в конфигурации или теме для одной строки под часами: ЦП, свободная память и свободное хранилище. Это отключено, пока вы не включите, и обновляется только пока Главный экран на экране. |
| **Темы и карточки модулей** | Темы меняют цвета, обои, док и столбцы без пересборки, а карточки модулей позволяют другим приложениям вставлять плитку, только с вашего разрешения. |

И телевизор, который перестает работать против вас: никаких спонсируемых рядов, никаких назойливых «Discover», никакой аналитики, звонящей домой, никаких приложений, которые вы не просили.

| | |
|---|---|
| ![Верхняя полка называет приложение в фокусе над окружающим свечением его цвета](docs/focus-2-up-netflix.png) | ![Всплывающее окно «Входы»: порты HDMI с состоянием подключения, AV и Live TV](docs/inputs-menu.jpg) |
| *Верхняя полка и окружающее свечение* | *Входы: HDMI с состоянием подключения, AV, Live TV* |
| ![Сетка со стеклянным бликом на плитке и ее названием под ней](docs/focus-1-fancode.png) | ![Заставка часов: тонкие часы, дрейфующие над свечением](docs/clock-screensaver.png) |
| *Сетка, один стеклянный блик, название плитки* | *Заставка часов, дрейфует, чтобы ничего не выгорело* |
| ![Тема aurora: обои и тонированные таблетки, добавленные без пересборки](themes/aurora/screenshot.jpg) | ![Шесть столбцов и док на шесть приложений из config.json темы](themes/six-columns/screenshot.jpg) |
| *Тема Aurora, добавленная с помощью `tools/theme.sh`* | *Шесть столбцов и док на шесть приложений, тот же лаунчер* |
| ![Перемещение плитки: удержан OK, выбрано Move, плитка подхвачена, остальные затемнены](docs/tile-move.jpg) | ![Библиотека приложений: установленные приложения, одно нажатие добавляет приложение обратно на Главный экран](docs/app-library.jpg) |
| *Удерживайте OK на плитке, Move: стрелки переносят ее, Back опускает* | *Библиотека приложений: одно нажатие возвращает удаленное приложение на Главный экран* |

<a id="supported-tvs"></a>
## Поддерживаемые телевизоры

Любой телевизор, работающий на **Android TV** или **Google TV**.

| Платформа | Что работает |
|---|---|
| **Android TV, Google TV** | Удаление bloatware и лаунчер. |
| **Fire TV** | Только половина с удалением bloatware, поскольку Fire OS не передает Главный экран стороннему лаунчеру. А на Fire TV Box 2015 года (Fire OS 5) даже эта половина не работает: каждый маршрут `pm` отклоняется. |
| **Некоторые модели TCL для китайского рынка** | Они отказываются устанавливать какой-либо лаунчер; в заголовке их списков это указано. |
| **Samsung (Tizen), LG (webOS), Roku, Vizio, Hisense VIDAA** | Не поддерживаются (нет ADB). Вместо этого отключите отслеживание: [cleanyour.tv/not-android](https://cleanyour.tv/not-android). Смотрите [SHOWCASE.md](SHOWCASE.md#other-platforms-fire-tv-and-lg-webos) для четырех портов webOS и [docs/devices/samsung-tizen.md](docs/devices/samsung-tizen.md) о том, что телевизор Samsung 2021 года отвечает по Wi-Fi (без ADB, поэтому без `pm disable-user`), если вы рассматриваете порт для Tizen. |

Проверенные списки от участников, одна папка на модель в [`examples/`](examples/). Бренды с наибольшим количеством списков, каждый связан с его моделями на веб-сайте:

<!-- tv-brands:start: generated by tools/gen_tables.py from examples/*/tv.json; edit those, not this -->

| | | | | | |
|---|---|---|---|---|---|
| [TCL](https://cleanyour.tv/tvs?q=TCL) · 84 | [Sony](https://cleanyour.tv/tvs?q=Sony) · 50 | [Xiaomi](https://cleanyour.tv/tvs?q=Xiaomi) · 43 | [Philips](https://cleanyour.tv/tvs?q=Philips) · 23 | [Skyworth](https://cleanyour.tv/tvs?q=Skyworth) · 17 | [Hisense](https://cleanyour.tv/tvs?q=Hisense) · 16 |
| [SHARP](https://cleanyour.tv/tvs?q=SHARP) · 10 | [Amazon Fire TV](https://cleanyour.tv/tvs?q=Amazon%20Fire%20TV) · 9 | [Haier](https://cleanyour.tv/tvs?q=Haier) · 7 | [Panasonic](https://cleanyour.tv/tvs?q=Panasonic) · 7 | [BenQ](https://cleanyour.tv/tvs?q=BenQ) · 6 | [JVC](https://cleanyour.tv/tvs?q=JVC) · 6 |
| [Toshiba](https://cleanyour.tv/tvs?q=Toshiba) · 6 | [Acer](https://cleanyour.tv/tvs?q=Acer) · 4 | [Formovie](https://cleanyour.tv/tvs?q=Formovie) · 4 | [Nokia](https://cleanyour.tv/tvs?q=Nokia) · 4 | [OnePlus](https://cleanyour.tv/tvs?q=OnePlus) · 4 | [Thomson](https://cleanyour.tv/tvs?q=Thomson) · 4 |
| [Artel](https://cleanyour.tv/tvs?q=Artel) · 3 | [FFalcon](https://cleanyour.tv/tvs?q=FFalcon) · 3 | [Google](https://cleanyour.tv/tvs?q=Google) · 3 | [Grundig](https://cleanyour.tv/tvs?q=Grundig) · 3 | [Motorola](https://cleanyour.tv/tvs?q=Motorola) · 3 | [Noblex](https://cleanyour.tv/tvs?q=Noblex) · 3 |
| [NVIDIA Shield](https://cleanyour.tv/tvs?q=NVIDIA%20Shield) · 3 | [onn](https://cleanyour.tv/tvs?q=onn) · 3 | [RCA](https://cleanyour.tv/tvs?q=RCA) · 3 | [Redmi](https://cleanyour.tv/tvs?q=Redmi) · 3 | [RockTek](https://cleanyour.tv/tvs?q=RockTek) · 3 | [Vu](https://cleanyour.tv/tvs?q=Vu) · 3 |

<details>
<summary>+80 других брендов и 14 брендов проекторов</summary>

**Challenger** 2 · **CHiQ** 2 · **DEXP** 2 · **EKO** 2 · **Hitachi** 2 · **Insignia Fire TV** 2 · **Kalley** 2 ·
**Kogan** 2 · **Lumio** 2 · **Master-G** 2 · **PRISM+** 2 · **Sankey** 2 · **Sber** 2 · **Síragon** 2 · **TIM** 2 ·
**Vidda** 2 ·
AiPro2K · AiPro4K · AIWA · AQUA · ASUS · Beko · Bell Canada · BGH · Caxium · Cecotec · Compac · Dcolor · Dialog ·
Durabrand · DYON · Essentiel b · Freebox · HAAM · Hikeen · Home+ · Impex · INCLO · Indurama · Jio · Karbonn · Kodak ·
Koryo · KTC · KUNFT · Liberton · LYNCAST · Magyar Telekom · MarQ · MECOOL · MTC · Next · OK. · OPPO · Panavox · PEAQ ·
Philco · Polytron · PPTV · Prosonic · Salora · SAMPO · SANYO · Seleco · Smarttech · STRONG · SunWind · Super General ·
TD Systems · Tele System · Tesla · TiVo · Tornado · Turkcell · Tuvio · Verizon · VISIO · Vision · Vityas · X.Vision ·
проекторы Alwtniet, Anker Nebula, BYINTEK, Chihi, Epson, Gadnic, HOTACK, HY320, JMGO, Magcubic, Portronics, Stellamore, Wanbo и XGIMI

</details>

<!-- tv-brands:end -->

**Найдите свой телевизор:** воспользуйтесь поиском на [cleanyour.tv/tvs](https://cleanyour.tv/tvs) или полной таблицей в [examples/README.md](examples/README.md).

Вашего телевизора здесь нет? Промпт обнаружит bloatware сам. Добавьте свой список afterwards, и следующий человек с вашей моделью пропустит этот шаг: [CONTRIBUTING.md](CONTRIBUTING.md).

<a id="doing-it-by-hand"></a>
## Сделать вручную

Все, что делает помощник, вы можете выполнить сами. Сначала на компьютере должны быть две вещи:

| Вам нужно | Для чего |
|---|---|
| **Python 3** (любая версия 3.x) | Инструменты. Команда venv ниже устанавливает то, что они импортируют. |
| **JDK с 17 по 22** (полный JDK, включая `jlink`) и **Android SDK platform 34** с **build-tools 34.0.0 или любой более новой версией 34.x** | Сборка лаунчера. JDK 23 и новее останавливает Gradle 8.9. Platform 34 — это та, которую читает сборка; более новая платформа ее не заменяет. В macOS, если ничего из этого не установлено: `brew install openjdk@17 android-commandlinetools`, затем `sdkmanager "platforms;android-34" "build-tools;34.0.0"`. В Linux скрипт установки ищет в `~/Android/Sdk` и `java` в вашем PATH. |

`tools/tv.py` общается с сетевым ADB через порт 5555. Если этот порт остается закрытым, а телевизор предлагает беспроводную отладку с кодом сопряжения (так делают Chromecast с Google TV и Google TV Streamer), сопрягите его один раз с помощью стандартного `adb`. Затем либо выполните `adb tcpip 5555`, чтобы открыть порт, что обычно действует только до перезагрузки телевизора, либо оставьте его закрытым: укажите `TV_ADB_BINARY` на тот же `adb`, а `TV_HOST` на порт, который показывает экран беспроводной отладки, и инструменты достигнут телевизора через сопряженное соединение, при этом на 5555 ничего не будет прослушиваться ([tools/native-adb.md](tools/native-adb.md)). В [Устранении неполадок](docs/TROUBLESHOOTING.md#connecting) описаны оба варианта с шагами сопряжения.

```bash
python3 -m venv tools/venv && tools/venv/bin/pip install -r tools/requirements.txt
export TV_HOST=192.168.1.50                                   # IP-адрес вашего телевизора

tools/venv/bin/python -I tools/tv.py --probe                 # модель, версия Android, прошивка
tools/venv/bin/python -I tools/tv.py 'pm list packages'      # одна shell-команда на телевизоре
tools/disable.sh examples/xiaomi-mi-tv-4a/debloat.txt        # применить список удаления bloatware
tools/restore.sh examples/xiaomi-mi-tv-4a/debloat.txt        # отменить это, вернуть стандартный лаунчер
tools/venv/bin/python -I tools/check.py examples/xiaomi-mi-tv-4a/debloat.txt   # что отменило обновление прошивки
launcher/build-and-install.sh                                # собрать лаунчер и сделать его Главным (требуется экспорт TV_HOST выше)
tools/theme.sh themes/aurora                                 # добавить тему; --reset удаляет ее
python3 tools/wallpaper_prep.py ~/Pictures/trip mytheme/wallpapers   # ваши фотографии, адаптированные и затемненные для телевизора
```

| Инструмент | Что он делает |
|---|---|
| [`tools/tv.py`](tools/tv.py) | Чистый клиент ADB на Python: shell, пакетные команды, push, pull, перезагрузка и скриншоты, с возможностью предварительного нажатия клавиш пульта. Работает там, где стандартный бинарный файл `adb` заблокирован. Опциональный [сопряженный бэкенд Google ADB](tools/native-adb.md) для зашифрованной беспроводной отладки. |
| [`tools/docker-build.sh`](tools/docker-build.sh) | Собирает лаунчер или дополнение в Docker (JDK 17, Android SDK 34), поэтому этому компьютеру не нужно ничего, кроме Docker. Установите результат с помощью `SKIP_BUILD=1`. [Руководство](tools/docker-build.md). |
| [`tools/b64push.py`](tools/b64push.py) | Загружает большие файлы, такие как APK, частями в base64 и проверяет контрольную сумму. |
| [`tools/relay.py`](tools/relay.py) | Перенаправляет локальный порт на порт ADB телевизора для помощников, чья песочница не может достичь вашей сети. Прослушивает только на этом компьютере. [Руководство](tools/relay.md). |
| [`tools/disable.sh`](tools/disable.sh), [`restore.sh`](tools/restore.sh) | Применяет или отменяет список удаления bloatware; отмена выполняется из состояния, записанного перед изменением. |
| [`tools/recovery.py`](tools/recovery.py) | Записывает запись, необходимую `disable.sh` для самоотмены, и выводит пакет восстановления. |
| [`tools/check.py`](tools/check.py) | Сравнивает телевизор со списком, который был применен, на предмет того, что отменило обновление прошивки; `--fix` возвращает это обратно. |
| [`tools/match.py`](tools/match.py) | Читает сохраненный `pm list packages` и выводит для каждого пакета, сколько списков в `examples/` отключают его, сколько оставляют закомментированным, и их наиболее частую заметку; основные пакеты Android отображаются как `never`. Офлайн, ничего не меняет (`tools/venv/bin/python -I tools/match.py packages.txt`). |
| [`tools/adb-closed.py`](tools/adb-closed.py) | Проверяет, что сетевой порт ADB телевизора закрыт после отключения отладки: завершается с кодом 0, когда телевизор отказывает в соединении, 1, пока он еще открыт, 2, когда ничего не ответило или сама проверка не смогла запуститься. `nc` не требуется. |
| [`tools/philips-api.py`](tools/philips-api.py) | Только Philips: проверяет, что API управления JointSpace, который использует Home Assistant, все еще отвечает, до и после удаления bloatware (`tools/venv/bin/python -I tools/philips-api.py <tv ip>`). Сначала порт 1926 через HTTPS, затем 1925; читает только то, что отвечает без сопряжения. |
| [`tools/privacy.py`](tools/privacy.py) | Проверяет телевизор на наличие кандидатов на голосовые функции, ACR и телеметрию и выводит доказательства для каждого; `--write` превращает находки в список, который уже понимают `disable.sh` и `restore.sh`. |
| [`tools/theme.sh`](tools/theme.sh), [`theme_restart.py`](tools/theme_restart.py) | Отправляет папку из [`themes/`](themes/) в лаунчер и перезапускает Главный экран. |
| [`tools/wallpaper_prep.py`](tools/wallpaper_prep.py) | Превращает папку с вашими собственными фотографиями (JPEG, PNG, WebP, HEIC) в затемненные JPEG-файлы 1280×720 размером менее 300 КБ для папки `wallpapers/` темы. Требуется Pillow, а для HEIC — pillow-heif (`tools/requirements-photos.txt`). Никогда не трогает оригиналы. [Как это использовать](#your-own-photos-as-the-background). |
| [`tools/manage.py`](tools/manage.py) | Составляет список всех дополнений, тем и переключателей с их скриншотами, показывает, что есть на телевизоре, и устанавливает, обновляет или удаляет их, запуская собственный скрипт создателя. |
| [`tools/bench.py`](tools/bench.py) | Измеряет лаунчер, который отвечает на HOME: задержку клавиш, как далеко переместился фокус, подтормаживающие кадры, холодный старт, возврат на Главный экран, а также затраты простаивающего ЦП и PSS. Ничего не меняет на телевизоре и записывает необработанные показатели по каждой клавише в JSON; без дополнительной установки. |
| [`tools/trace.py`](tools/trace.py), [`trace_report.py`](tools/trace_report.py) | Записывает трассировки Perfetto лаунчера (возврат на Главный экран, холодный старт, D-pad) и сообщает, куда уходит время, за каждый запуск и до/после. Опционально: требуется [`requirements-perf.txt`](tools/requirements-perf.txt). [Руководство](tools/trace.md). |
| [`tools/flamechart.py`](tools/flamechart.py) | Рисует диаграмму пламени до/после на основе этих трассировок для пул-реквеста: одна дорожка на поток на общей шкале времени, работа, на которую нацелено изменение, выделена пурпурным с ее общим итогом. Опционально, как и инструменты трассировки. [Руководство](tools/flamechart.md). |
| [`tools/screendiff.py`](tools/screendiff.py) | Сравнивает скриншот до и после попиксельно, исключая часы или все, что вы замаскировали, и записывает пару с размытым названием вашей Wi-Fi сети. Опционально, как и инструменты трассировки. [Руководство](tools/screendiff.md). |
| [`tools/race_calendar.py`](tools/race_calendar.py) | Записывает календарь F1 этого сезона в тему для режима гоночных выходных из бесплатного API Jolpica. |
| [`launcher/build-and-install.sh`](launcher/build-and-install.sh) | Собирает сжатую версию (около 572 КБ), устанавливает ее, переключает Главный экран и выполняет откат, если Главный экран не переключается на нее. |

Скрипты никогда не оставляют телевизор без приложения Главного экрана: они отключают только распознанный стандартный лаунчер и пропускают приложение Главного экрана в списке, пока другой лаунчер не ответит на HOME. Ваши собственные списки могут находиться вне репозитория: пути к спискам относительны каталога, из которого вы запускаете, и абсолютные пути тоже работают.

<details>
<summary><b>Windows (PowerShell)</b></summary>

У каждого скрипта есть двойник для PowerShell рядом с ним. Установите Python 3 и JDK с 17 по 22, и в SDK Manager добавьте platform 34 и build-tools 34 (34.0.0 или любой более новый 34.x). Скрипт использует `JAVA_HOME`, если он указывает на JDK в этом диапазоне, иначе встроенный JDK Android Studio, когда этот JDK находится в том же диапазоне:

```powershell
python -m venv tools\venv; tools\venv\Scripts\python.exe -m pip install -r tools\requirements.txt
powershell -ExecutionPolicy Bypass -File launcher\build-and-install.ps1 -TvHost 192.168.1.50
powershell -ExecutionPolicy Bypass -File tools\disable.ps1 -TvHost 192.168.1.50 examples\xiaomi-mi-tv-4a\debloat.txt
powershell -ExecutionPolicy Bypass -File tools\restore.ps1 -TvHost 192.168.1.50 examples\xiaomi-mi-tv-4a\debloat.txt
powershell -ExecutionPolicy Bypass -File tools\theme.ps1 -TvHost 192.168.1.50 themes\aurora
```

Последние две — это отмена и добавление темы, строки `tools/restore.sh` и `tools/theme.sh`, которые разделы выше приводят в bash. На Google TV отмена также затрагивает стандартный лаунчер: `-Stock com.google.android.apps.tv.launcherx`.

</details>

<details>
<summary><b>Как скрипты защищают Главный экран</b></summary>

Скрипты установки спрашивают телевизор, какой лаунчер владеет Главным экраном, и отключают только тот, который они распознают, — четыре из `KNOWN_STOCK_LAUNCHERS`: `com.google.android.tvlauncher`, `com.google.android.apps.tv.launcherx`, `com.google.android.leanbacklauncher` и Xiaomi `com.mitv.tvhome` (PatchWall). Передайте `STOCK_LAUNCHER=<package>` (`-StockLauncher`), чтобы переопределить, или `none`, чтобы не трогать его.

`tools/disable.sh` (`disable.ps1`) применяет то же правило, прежде чем что-либо отключить:

- Если список содержит приложение, владеющее Главным экраном, и никакое другое приложение на телевизоре не отвечает на HOME, он пропускает эту запись, сообщает почему и отключает остальную часть списка. Таким образом, список, примененный до передачи лаунчера, не может оставить телевизор без ничего для запуска.
- Мастер настройки, приложения настроек, `FallbackHome` производителя и приложения заводских тестов (Xiaomi `com.duokan.factorytest`) также отвечают на HOME и не учитываются.
- На Google TV он также сохраняет владельца, пока setupwraith отвечает на HOME и остается включенным (не указан в списке или сохранен для сети Wi-Fi): setupwraith отвечает раньше установленного лаунчера, который еще не является Главным экраном, поэтому он занял бы Главный экран.

Запустите тот же список снова, как только `launcher/build-and-install.sh` сделает новый лаунчер Главным экраном, и запись будет применена; `FORCE_HOME=1` (`$env:FORCE_HOME`) отключает ее в любом случае.

</details>

## Микрофон, и что можно о нем сказать

«Какой из этих пакетов прослушивает?» — на это нет честного однострочного ответа: сканирование разрешений показывает пятьдесят системных пакетов с `RECORD_AUDIO`, которые ничего не записывают, а клиенты ACR видят экран вообще без разрешения на аудио. [`tools/privacy.py`](tools/privacy.py) сообщает, что телевизор на самом деле говорит, с доказательствами для каждого кандидата на голосовые функции, ACR и телеметрию: `TV_HOST=192.168.1.50 tools/venv/bin/python -I tools/privacy.py`, а `--write` превращает их в обычный список удаления bloatware. Чего аудит не может сделать, так это доказать намерение: [docs/privacy.md](docs/privacy.md) объясняет почему.

<a id="the-launcher"></a>
## Лаунчер

Небольшой нативный главный экран для Android TV: **около 572 КБ**, чистый Java, создан для телевизоров с 1 ГБ оперативной памяти. Без размытия, без видео, без разрешения на сеть, без фоновых служб. Телевизору требуется Android 8.0 (API 26) или новее, `minSdk` в [`launcher/app/build.gradle`](launcher/app/build.gradle); что осталось на более старом устройстве, описано в [Устранении неполадок](docs/TROUBLESHOOTING.md).

| Что | Как это работает |
|---|---|
| **Настройка** | Порядок дока, скрытые приложения, приложение Live TV, от 4 до 7 плиток в ряду, уменьшенное движение. Все в [`config.xml`](launcher/app/src/main/res/values/config.xml) |
| **Настройки на телевизоре** | Удерживайте OK на «Настройках» для настроек лаунчера. Опциональный `launcher_settings_button` заставляет обычный клик открывать их напрямую; настройки телевизора остаются на странице настроек и их плитке приложения. |
| **Темы** | Фон, обои и макет из `config.json`, отправленного по Wi-Fi, без пересборки. Двадцать восемь поставляются в [`themes/`](themes/), включая встроенную `default/` |
| **31 язык** | Следует языку телевизора, с полностью зеркальным макетом справа налево для иврита |
| **Библиотека приложений** | Опционально: просмотр всех установленных приложений и добавление или удаление ярлыков с Главного экрана. Смотрите [руководство по библиотеке приложений](docs/app-library.md) |
| **Меню плитки** | Включено по умолчанию (`tile_menu`): удерживайте OK на плитке для Move и App info, плюс Remove from Home, когда библиотека приложений включена. Если выключено, удержание OK открывает App info |
| **Карточки модулей** | Любое приложение на телевизоре может предложить свою плитку; вы одобряете каждую один раз. Смотрите [`docs/modules.md`](docs/modules.md) |
| **Дополнения** | Опциональные приложения, которые подключаются как карточки модулей, хранятся в [`addons/`](addons/) и никогда не встраиваются в лаунчер |
| **Заставка часов** | Дрейфующие часы поверх свечения, чтобы ничего не выгорело |
| **Клавиши пульта** | Сохраняет работу кнопок Input, YouTube и шестеренки после исчезновения стандартного лаунчера |

Темы, переключатели и дополнения вместе, со скриншотами: [cleanyour.tv/addons](https://cleanyour.tv/addons).

**Больше:** [docs/launcher.md](docs/launcher.md) содержит страницу настроек лаунчера строка за строкой, изменение главного экрана по умолчанию, языки, клавиши пульта, заставку часов, навигацию и самостоятельную сборку.

<a id="your-own-photos-as-the-background"></a>
<details>
<summary><b>Ваши собственные фотографии в качестве фона</b></summary>

Тема может вращать папку с изображениями за Главным экраном без пересборки. В репозитории нет изображений: вы приносите свои и решаете, имеете ли вы право их показывать.

1. **Создайте папку темы.** Скопируйте понравившуюся тему из [папки themes](themes/), например `themes/aurora`, в новую папку, такую как `mytheme/`, или начните с пустого `config.json`.
2. **Подготовьте фотографии.** Яркая фотография на 12 МП тяжела для телевизора с 1–2 ГБ и заглушает часы и плитки. `tools/wallpaper_prep.py` обрезает по центру до 16:9, сохраняет JPEG-файлы 1280×720 размером менее 300 КБ и затемняет само изображение, поэтому `wallpaper_dim` может оставаться на 0. Фотографии с телефона в формате HEIC работают. Ваши оригиналы никогда не затрагиваются.

   ```bash
   python3 -m pip install -r tools/requirements-photos.txt
   python3 tools/wallpaper_prep.py ~/Pictures/trip mytheme/wallpapers
   ```

   Опции: `--brightness 0.25` (от 0.1 до 1.0), `--gradient 0.6` (дополнительный черный к доку), `--size 1280x720`, `--max-kb 300`.
3. **Настройте ротацию** в `mytheme/config.json`:

   ```json
   { "wallpaper": true, "wallpaper_rotation_minutes": 1, "wallpaper_order": "shuffle", "wallpaper_dim": 0 }
   ```

   | Ключ | Примечания |
   |---|---|
   | `wallpaper_rotation_minutes` | Целые минуты, от 0 до 1440. **1 — самое быстрое.** `0` означает отсутствие ротации, а дробь, такая как `0.25`, читается как `0`, что останавливает ее. |
   | `wallpaper_order` | `shuffle` никогда не показывает одно и то же изображение дважды подряд; `sequential` следует именам файлов. |
   | `wallpaper_dim` | Черный оверлей в процентах. Оставьте 0, когда изображения уже затемнены. |
   | `dock_glass`, `dock_opacity` | Полоса дока из матового стекла (от 30 до 100%), чтобы изображение было видно за плитками. |
   | `greeting_name` | Имя после приветствия: «Добрый вечер, Сэм». |
   | `show_stats`, `app_library`, `reduced_motion` | Строка статистики под часами, таблетка библиотеки приложений, более спокойное движение для слабых графических процессоров. |

4. **Отправьте это на телевизор** (это один раз перезапускает Главный экран и сохраняет работу помощника клавиши Home):

   ```bash
   tools/theme.sh mytheme            # Windows: tools\theme.ps1 -TvHost 192.168.1.50 mytheme
   ```

   На телевизоре в **Настройках лаунчера → Обои** можно выбрать одно изображение, **Нет** или **Тема по умолчанию**, которая снова включает ротацию.
5. **Снимите это** с помощью `tools/theme.sh --reset`.

Чего это не может: нет перекрестного затухания (изображение меняется скачком), нет ротации чаще раза в минуту, а заставка часов показывает только время и дату, никогда не фотографии. Без папки `wallpapers/` тема все равно работает, и Главный экран сохраняет свой простой цвет. Изображение декодируется в память, пока Главный экран его показывает: около 4 МБ при 1080p в стандартном 16-битном цвете, 8 МБ с `wallpaper_true_color` (смотрите [themes/README.md](themes/README.md)), поэтому на телевизоре с 1 ГБ держите изображения небольшими.

</details>

<a id="restoring-your-tv"></a>
## Восстановление вашего телевизора

Сохраните список, который вы применили. Одна строка возвращает телевизор в прежнее состояние:

```bash
TV_HOST=192.168.1.50 tools/restore.sh examples/<your tv>/debloat.txt                                    # Android TV
TV_HOST=192.168.1.50 tools/restore.sh examples/<your tv>/debloat.txt com.google.android.apps.tv.launcherx  # Google TV
```

| Что | Как |
|---|---|
| **Сначала создается запись** | Прежде чем `tools/disable.sh` что-либо изменит, он записывает, как выглядел телевизор, в `~/.cleanyourtv/`. |
| **Восстановление воспроизводит ее** | Пакет, который вы отключили сами, остается отключенным, а Главный экран возвращается к компоненту, который им владел. |
| **Лаунчер остается установленным** | Удалите его из раздела телевизора Настройки → Приложения, если хотите, чтобы его не было. |
| **Нет компьютера?** | Если телевизор недоступен, его собственная страница Настройки → Приложения также может повторно включить пакеты. |

**Больше:** [docs/restore.md](docs/restore.md) содержит информацию о том, что хранит запись, когда учитывается аргумент стандартного лаунчера и что происходит без записи.

<a id="after-a-firmware-update"></a>
## После обновления прошивки

Обновление устанавливается поверх очищенной системы: перечисленные пакеты возвращаются, Главный экран переходит к стандартному лаунчеру, и появляются новые предустановки, которые не упоминаются ни в одном списке. Снова откройте ADB, как в [Быстром старте](#quick-start) шаг 1, затем сравните телевизор со списком, который вы применили; `--fix` возвращает его:

```bash
TV_HOST=192.168.1.50 tools/venv/bin/python -I tools/check.py examples/<your tv>/debloat.txt
```

**Больше:** [docs/firmware-updates.md](docs/firmware-updates.md) содержит коды выхода, еженедельную проверку, что меняет `--fix`, телевизоры, которые сохраняют стандартный лаунчер в качестве Главного экрана, и списки, которые отключают программу обновления.

## Когда что-то идет не так

Полный список проблем, с которыми мы столкнулись, находится в [docs/TROUBLESHOOTING.md](docs/TROUBLESHOOTING.md). Три наиболее важные:

- 🍎 **macOS сообщает «No route to host», хотя порт открыт**: конфиденциальность локальной сети не пускает приложение терминала в локальную подсеть, и разрешение принадлежит этому приложению, а не клиенту, поэтому стандартный `adb` и `tools/tv.py` терпят неудачу одинаково (замечено на macOS 26). Разрешите Terminal, iTerm2 или VS Code в Системные настройки → Конфиденциальность и безопасность → Локальная сеть, затем закройте и снова откройте его ([Устранение неполадок](docs/TROUBLESHOOTING.md#connecting)).
- ⚠️ **Отключайте стандартный лаунчер только после того, как новый установлен и работает**, иначе Главный экран приземлится на приложение заводских тестов. Скрипт установки упорядочивает это за вас.
- 🔁 **На Google TV мастер настройки** (`com.google.android.tungsten.setupwraith`) может занять Главный экран и вызвать циклический сбой системы после отключения стандартного лаунчера. Отключите и его, и внесите его в свой `debloat.txt`, чтобы восстановление вернуло его.
  - Но сначала проверьте `dumpsys wifi | grep -o 'cname=[^ ]*'`: если сеть Wi-Fi была сохранена во время настройки, она принадлежит setupwraith, и его отключение удаляет сеть (сначала повторно подключитесь к ней в Настройках; `tools/disable.sh` пропускает setupwraith, пока вы это не сделаете).
  - На собственных Chromecast от Google и на Google TV Streamer это также лишает возможности трансляции с телефона, смотрите [Устранение неполадок](docs/TROUBLESHOOTING.md).
  - Уже застряли? `tools/tv.py 'pm enable --user 0 com.google.android.apps.tv.launcherx'`. На некоторых устройствах (замечено на TCL Smart TV Pro, Android 14) это одностороннее действие: возврат к этому лаунчеру тогда требует ADB, или сохраните launcherx и используйте `stock_home_redirect`, смотрите [Устранение неполадок](docs/TROUBLESHOOTING.md#working-on-the-tv).

<a id="questions-people-ask"></a>
## Вопросы, которые задают люди

<details>
<summary><b>Я не программирую и у меня нет ноутбука. Я все еще могу это сделать?</b></summary>

Да. Независимые разработчики создали бесплатные приложения с открытым исходным кодом на основе списков телевизоров CleanYourTV, которые выполняют очистку по Wi-Fi без помощника по программированию. Каждое сначала показывает план, только отключает приложения и может все вернуть:

| Приложение | Для | Автор |
|---|---|---|
| [Clean Your TV app](https://github.com/udhaykumarbala/cleanyourtv-app) | Телефон Android | [@udhaykumarbala](https://github.com/udhaykumarbala) |
| [Tellyscope](https://github.com/man15h/tellyscope) | Телефон Android | [@man15h](https://github.com/man15h) |
| [TidyTV](https://github.com/jolan94/tidytv) | Телефон Android, Google Play | [@jolan94](https://github.com/jolan94) |
| [CleanMyTV](https://github.com/wingedpanther/cleanmytv) | Mac и Windows | [@wingedpanther](https://github.com/wingedpanther) |

Эти приложения являются независимыми проектами, не связанными с CleanYourTV или его сопровождающим и не одобренными ими, и каждое предоставляется как есть под собственной лицензией. Сообщайте о проблемах с приложением в репозитории этого приложения. Больше на [cleanyour.tv/app](https://cleanyour.tv/app).

</details>

<details>
<summary><b>Это безопасно? Может ли это превратить телевизор в кирпич?</b></summary>

Ничего не прошивается, не рутируется и не удаляется; пакеты отключаются в профиле пользователя. Риск заключается в отключении чего-то, на что опирается телевизор, поэтому списки применяются небольшими пакетами с готовым скриптом восстановления. Собственная страница телевизора Настройки → Приложения может повторно включить пакеты даже без инструментов. Если телевизор больше не запускается настолько, чтобы это можно было сделать, сброс к заводским настройкам из меню восстановления обычно является способом вернуться.

Больше: [docs/faq.md](docs/faq.md#is-this-safe-can-it-brick-the-tv)

</details>

<details>
<summary><b>А как насчет обновлений прошивки?</b></summary>

Программа обновления оставлена включенной в большинстве списков, поэтому обновления прошивки приходят как обычно. Некоторые списки отключают собственную программу обновления телевизора, и на них обновление прошивки приходит только когда вы снова ее включаете. Когда обновление все-таки устанавливается, оно устанавливается поверх очищенной системы, поэтому пакет возвращается, и вы повторно запускаете скрипт: смотрите [После обновления прошивки](#after-a-firmware-update).

</details>

<details>
<summary><b>Разве приложения не сломаются?</b></summary>

Потоковые приложения по-прежнему обновляются через Play Store, который не трогают. Лаунчер просто перечисляет то, что установлено, и запускает это с помощью интентов, которые стабильны уже десятилетие.

</details>

<details>
<summary><b>Как мне переставить свои приложения?</b></summary>

Удерживайте OK на «Настройках» (вверху справа) и выберите «Reorder apps». OK подхватывает приложение, стрелки перемещают его, Back опускает, и Back снова завершает. Удержание OK на плитке также предлагает Move (`tile_menu`, включено по умолчанию), что сразу подхватывает это приложение. Больше: [docs/launcher.md](docs/launcher.md#launcher-settings-and-the-default-home)

</details>

<details>
<summary><b>Могу ли я сделать это для кого-то в другом доме?</b></summary>

Да, через частную ссылку [Tailscale](https://tailscale.com) вместо той же сети Wi-Fi: либо Tailscale на их телевизоре, общий с вами, либо компьютер или Apple TV в их доме, маршрутизирующий к нему. Никогда не открывая порт ADB на их роутере. Пошаговая инструкция в [docs/REMOTE.md](docs/REMOTE.md).

</details>

<details>
<summary><b>Разве доступ по ADB — это не дыра в безопасности?</b></summary>

Это одно явное нажатие «разрешить этот компьютер» на телевизоре, такое же, как при разработке приложения для Android. Сетевой ADB передается в открытом виде через порт 5555, и на некоторых прошивках любое устройство в локальной сети получает оболочку, поэтому закрывайте его, когда закончите:

1. На телевизоре: Параметры разработчика → отключите **Отладку по USB**, **Сетевую отладку/отладку ADB** и **Беспроводную отладку**, в зависимости от того, что есть на телевизоре, и отзовите авторизации отладки по USB.
2. Перезагрузите телевизор, затем подтвердите, что порт исчез с вашего компьютера: `python3 tools/adb-closed.py <tv ip>` должен сообщить, что порт закрыт.

Лаунчер продолжает работать без отладки. Больше, включая проверку собственного порта беспроводной отладки: [docs/faq.md](docs/faq.md#isnt-adb-access-a-security-hole)

</details>

<details>
<summary><b>Может ли он блокировать рекламу и внутри приложений?</b></summary>

Частично, с помощью Android Private DNS (Android 9 и новее). Направьте его на блокирующий рекламу резолвер, такой как [AdGuard DNS](https://adguard-dns.io), и домены рекламы и трекеров каждого приложения перестанут разрешаться, на всю систему, переживая перезагрузки. Компромисс: этот резолвер затем видит каждый DNS-запрос, который делает телевизор, и он не удаляет рекламу YouTube.

Больше, с двумя командами и тем, как переключиться обратно: [docs/faq.md](docs/faq.md#can-it-block-ads-inside-apps-too)

</details>

<details>
<summary><b>Есть ли в собственных настройках телевизора переключатели, которые стоит переключить?</b></summary>

Несколько, и они не требуют ADB: рекламный идентификатор, местоположение, «Использование и диагностика» и «Сканирование всегда доступно», плюс режим «Только приложения», где стандартный лаунчер остается. Переключите «Использование и диагностика» до удаления bloatware; на некоторых телевизорах его страница исчезает вместе с ним.

Больше, с путями для Google TV, Android TV и Fire OS: [docs/faq.md](docs/faq.md#are-there-switches-in-the-tvs-own-settings-worth-flipping-too)

</details>

<details>
<summary><b>AirPlay?</b></summary>

Не из этого репозитория. Встроенный Chromecast остается для телефонов Android. Для iPhone работает [jqssun/android-airplay-server](https://github.com/jqssun/android-airplay-server); скрипт установки для него есть в [PR #84](https://github.com/Gathin23/cleanyourtv/pull/84).

</details>

<details>
<summary><b>Могу ли я просто скачать APK?</b></summary>

Соберите его с помощью однострочного скрипта в разделе [Сделать вручную](#doing-it-by-hand); это занимает минуту, и вы контролируете, что попадет на ваш телевизор. Для этого нужны JDK и Android SDK, указанные там. Готовых бинарников нет.

</details>

## История

17 октября 2026 года я опубликовал [до и после](https://x.com/gathint/status/2111379569030939102) телевизора моих родителей, очищенного Claude Code по Wi-Fi. Это набрало 8,6 млн просмотров, люди начали делать то же самое со своими телевизорами, и их ответы превратились в списки здесь: более 170 моделей телевизоров от более 200 участников за первые четыре дня. Репозиторий назывался tv-vibehack до 19-го; старые ссылки работают.

Спустя две недели он стал репозиторием №1 в трендах GitHub за неделю 19–25 октября, с более чем 46 тыс. звезд и 5,7 тыс. форков, и 1,4 млн просмотров и 260 тыс. клонов за 14 дней. Списки теперь охватывают 463 модели телевизоров от 124 брендов. Освещение: 534 статьи из 57 стран и 663 видео на YouTube и Bilibili, все в [docs/PRESS.md](docs/PRESS.md) (числа по состоянию на 9 ноября 2026 года).

<a id="contributing"></a>
## Участие в разработке

Самый полезный вклад — это список удаления bloatware для вашего телевизора, чтобы следующему человеку с этой моделью не пришлось открывать его заново. [CONTRIBUTING.md](CONTRIBUTING.md) содержит формат и тестирование, которое мы просим. Участвуете через помощника по программированию? [AGENTS.md](AGENTS.md) дает ему те же правила.

| Как помочь | Что это значит |
|---|---|
| **Список удаления bloatware для вашего телевизора** | Самый полезный: следующий человек с этой моделью пропускает обнаружение. |
| **Лаунчер и промпт** | Улучшения лаунчера и более точные формулировки промпта тоже приветствуются. |
| **Создали что-то поверх?** | Лаунчер, порт, тему: добавьте это в [SHOWCASE.md](SHOWCASE.md), где уже живут двести тридцать проектов, отсортированных по главным экранам, форкам, дополнениям, инструментам и другим платформам, с индексом по брендам телевизоров. |

Люди, чья работа есть в этом репозитории:

<a href="https://github.com/Gathin23/cleanyourtv/graphs/contributors"><img src="https://contrib.rocks/image?repo=Gathin23/cleanyourtv&columns=16&max=400" alt="Contributors"></a>

<details>
<summary><strong>История звезд</strong></summary>

<a href="https://star-history.com/#Gathin23/cleanyourtv&Date"><img src="https://api.star-history.com/svg?repos=Gathin23/cleanyourtv&type=Date" alt="Star history chart" width="640"></a>

</details>

## Контакты

| Для | Где |
|---|---|
| **Вопросы о вашем телевизоре** | [GitHub Discussions](https://github.com/Gathin23/cleanyourtv/discussions) |
| **Пресса и запросы** | [hello@itsgathin.com](mailto:hello@itsgathin.com) |
| **Проблемы безопасности** | Сообщайте о них приватно через [вкладку Security](https://github.com/Gathin23/cleanyourtv/security), смотрите [`SECURITY.md`](SECURITY.md) |

## Правовая информация

- CleanYourTV — независимый проект с открытым исходным кодом. Он не связан, не одобрен и не спонсируется каким-либо производителем телевизоров или платформой. Названия брендов и моделей используются только для того, чтобы указать, на каком телевизоре тестировался список, и остаются товарными знаками их владельцев.
- Он работает только через настройки, которые телевизор сам предлагает своему владельцу: Параметры разработчика, отладка ADB и собственный `pm disable-user` Android, тот же переключатель, что Настройки > Приложения > Отключить. Он не рутирует телевизор, не прошивает firmware и не обходит никакие блокировки, DRM или защиту от копирования, и репозиторий не содержит программного обеспечения производителя, прошивок или APK.
- Ничего не удаляется, и `tools/restore.sh` возвращает все обратно. Вы запускаете его на телевизоре, которым владеете, на свой страх и риск, и изменение программного обеспечения телевизора может повлиять на его гарантию или поддержку.
- Все здесь предоставляется как есть, без каких-либо гарантий, под лицензией MIT ниже.

## Лицензия

MIT, смотрите [`LICENSE`](LICENSE). Шрифт Outfit распространяется по лицензии SIL Open Font License, смотрите `launcher/FONT-LICENSE-OFL.txt`.