# React — Trivia API

Случайный вопрос только по кнопке, начальная фраза и обработка ограничений API.

Маршрут: прочитать условия → установить зависимости → запустить → пройти проверки → подготовить к сдаче.

## Условия

- [ASSIGNMENT.md](docs/materials/homework-2026-09-20/docs/frontend/trivia-api/ASSIGNMENT.md)

## Запуск из чистой копии

Нужны Node.js (>=22.12.0) и npm. Откройте терминал в корне этого репозитория рядом с package.json.

~~~bash
node --version
npm --version
npm ci
npm run dev
~~~

Откройте локальный адрес, показанный Vite в терминале. Остановка: Ctrl+C.

## Проверка

~~~bash
npm test
npm run build
~~~

В этой упаковке установки и проверки не выполнялись. Сборка, браузер, macOS и реальное устройство имеют отдельный статус; наличие файлов не означает готовность к сдаче.

## Разбор и материалы

- [Исходное руководство приложения](docs/PROJECT-README.md)
- [MANUAL.md](docs/materials/homework-2026-09-20/docs/frontend/trivia-api/MANUAL.md)

## Зависимости и открытые проверки

- Внешний API, доступ к сети или настройки сервиса могут требоваться по исходному руководству. Доступность сервиса сейчас не проверялась.


## Единый запуск

```bash
bash ./build-and-run.sh --list
bash ./build-and-run.sh
```

[Запуск и перенос в свой GitHub](docs/CLIENT-HANDOFF.md).

<!-- upstream-tools:start -->
## Скачать независимую копию

В папке `delivery-tools` находятся скрипт, Python companion и каталог всех 24 проектов.
Нужны Git, Python 3.9+ и Bash 3.2+ (macOS/Linux или Windows через WSL/Git Bash).

```bash
mkdir -p "$HOME/Projects"
bash delivery-tools/export-project.sh --catalog delivery-tools/projects.tsv --project web-trivia --dest "$HOME/Projects/polina-trivia-api" --init-git
```

Результат: отдельная папка с новым Git без исходной истории и remote. Без
`--init-git` Git metadata отсутствует. [Все параметры](delivery-tools/README.md).
Отмеченный downloader и этот блок удаляются из чистой копии автоматически.
<!-- upstream-tools:end -->
