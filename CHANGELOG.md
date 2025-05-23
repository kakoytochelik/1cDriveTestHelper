# Change Log

## 1.4.0

- **Интеграция сборки тестов в TypeScript**:
    - Полностью перенесена логика скрипта `BuildYAML.bat` в код плагина (`phaseSwitcher.ts`).
    - Процесс сборки тестов теперь управляется непосредственно из расширения, используя API VS Code и Node.js для файловых операций и запуска процессов 1С.
    - [BETA] Сборка тестов теперь запускается на macOS.
- **Улучшения интерфейса "Phase Switcher"**:
    - Заменен выпадающий список фаз на древовидное представление (Tree-View) с раскрывающимися группами.
    - В заголовки групп фаз добавлен счетчик включенных тестов.
    - Добавлены индивидуальные кнопки-переключатели в заголовок каждой фазы для переключения тестов внутри конкретной фазы. _(Удалена общая кнопка "Переключить фазу".)_
- **Исправления**:
    - [Кнопка Обновить активна во время сборки тестов](https://github.com/kakoytochelik/1cDriveTestHelper/issues/2)
    - [Не запускается сборка тестов, если путь до пустой базы содержит пробелы](https://github.com/kakoytochelik/1cDriveTestHelper/issues/1)

## 1.3.3

- Интегрирована функциональность сборки тестов в панель расширения с заменой переменных в тестах
- Добавлены настройки расширения
- Добавлены иконки кнопок
- Исправлены стили и отображение некоторых элементов интерфейса

## 1.2.0

- Реализовано автодополнение шагов Gherkin на основе библиотеки шагов Vanessa Automation.
- Добавлены всплывающие подсказки для шагов Gherkin, отображающие описание шага из библиотеки шагов Vanessa Automation при наведении мыши на строку шага в YAML файлах.

## 1.1.1

- Добавлена возможность переходить к родительским сценариям из Phase Switcher
- Вставка блоков ВложенныеСценарии и ПараметрыСценария теперь происходит автоматически в соответствующие секции, а не в позицию курсора
- Улучшено отображение длинных названий сценариев в Phase Switcher

## 1.0.0

- Первый релиз