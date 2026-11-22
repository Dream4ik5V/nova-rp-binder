# NOVA RP Binder

Своя админ-панель для NOVA RP (GTA V / RAGE MP): ответы, команды, наказания, панель поверх игры, журнал и статистика.

## Установка
1. Скачайте `NOVA-RP-Binder-Setup.exe` из [последнего релиза](https://github.com/Dream4ik5V/nova-rp-binder/releases/latest).
2. Запустите — установка для текущего пользователя, без прав администратора.
3. Первый запуск: можно выбрать папку установки. Дальше приложение обновляется само (тихо, при запуске).

## Быстрый старт
1. **Настройки → Окно игры**: проверьте процессы игры (`GTA5.exe, RAGE Multiplayer.exe, RAGEMP.exe`) и нажмите «Проверить окно» при запущенной игре.
2. **Ответы / Команды / Наказания**: создайте бинды (`+ Добавить`), укажите текст, хоткей (кнопка «Записать») и «Показывать на панели».
3. Включите биндер: **F6** (или кнопка на главной).
4. В игре: **F7** — панель с биндами, клик по кнопке отправляет текст в чат. **Ctrl+F6** — остановить действие.
5. Хоткей бинда можно нажать прямо в игре — текст уйдёт в чат.


## Скриншоты

**binder-about.png**

![binder-about.png](https://raw.githubusercontent.com/Dream4ik5V/nova-rp-binder/main/images/binder-about.png)

**Ответы**

![Ответы](https://raw.githubusercontent.com/Dream4ik5V/nova-rp-binder/main/images/binder-answers.png)

**Команды с параметрами**

![Команды с параметрами](https://raw.githubusercontent.com/Dream4ik5V/nova-rp-binder/main/images/binder-commands.png)

**Координаты: точки кликов в окне игры**

![Координаты: точки кликов в окне игры](https://raw.githubusercontent.com/Dream4ik5V/nova-rp-binder/main/images/binder-coords.png)

**Счётчик ответов**

![Счётчик ответов](https://raw.githubusercontent.com/Dream4ik5V/nova-rp-binder/main/images/binder-counter.png)

**Редактор бинда**

![Редактор бинда](https://raw.githubusercontent.com/Dream4ik5V/nova-rp-binder/main/images/binder-editor.png)

**Подсказки команд (Ctrl+Tab)**

![Подсказки команд (Ctrl+Tab)](https://raw.githubusercontent.com/Dream4ik5V/nova-rp-binder/main/images/binder-hints.png)

**Главная: биндер, статистика, сравнение, последние действия**

![Главная: биндер, статистика, сравнение, последние действия](https://raw.githubusercontent.com/Dream4ik5V/nova-rp-binder/main/images/binder-home.png)

**Журнал**

![Журнал](https://raw.githubusercontent.com/Dream4ik5V/nova-rp-binder/main/images/binder-journal.png)

**Заметки и браузер**

![Заметки и браузер](https://raw.githubusercontent.com/Dream4ik5V/nova-rp-binder/main/images/binder-notes.png)

**Панель поверх игры**

![Панель поверх игры](https://raw.githubusercontent.com/Dream4ik5V/nova-rp-binder/main/images/binder-overlay.png)

**Панель: раскладка, положение, стиль**

![Панель: раскладка, положение, стиль](https://raw.githubusercontent.com/Dream4ik5V/nova-rp-binder/main/images/binder-panel.png)

**Наказания**

![Наказания](https://raw.githubusercontent.com/Dream4ik5V/nova-rp-binder/main/images/binder-punishments.png)

**Настройки: окно игры, ввод, задержки**

![Настройки: окно игры, ввод, задержки](https://raw.githubusercontent.com/Dream4ik5V/nova-rp-binder/main/images/binder-settings.png)

## Возможности
- Глобальные хоткеи, вставка в чат игры через буфер или «печать по буквам».
- Панель поверх игры: вкладки, поиск, шапка/поп-ап, прозрачность, масштаб, положение, стили кнопок.
- Параметры `{имя}` с окном-запросом, действия после отправки, сокращения (автозамена).
- Журнал действий с фильтрами и экспортом в CSV, статистика ответов по дням и времени.
- Заметки со встроенным браузером.
- Темы: Nova, Чёрная, Зелёная, Полночь, Закат, Светлая + свой акцент.
- Профили: экспорт/импорт файлом, «код профиля», ежедневные резервные копии (7 дней).
- Счётчик ответов поверх игры, умная панель (только когда активна игра).

## Для разработки
```
cd binder
npm install
npm start
```
Сборка установщика: `node binder/scripts/build_setup.cjs` (нужен Node.js, electron-builder в корне репозитория-студии и .NET Framework csc).

Требования: Windows 10/11 x64, установленный .NET Framework 4.8 (есть в Windows).
