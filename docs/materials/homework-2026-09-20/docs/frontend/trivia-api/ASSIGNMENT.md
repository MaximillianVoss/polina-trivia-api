# Trivia API — исходное задание

Источник: `uewfhouhwgrgw.zip/front/Screenshot 2026-09-18 at 14.19.46.png`.
Ниже переписан весь видимый английский текст задания, без подмены требований нашим решением.
Финский README в архиве отсутствует; ссылка на него видна только на скриншоте.

[Открыть исходный скриншот](../../../sources/front/Screenshot 2026-09-18 at 14.19.46.png)

---

# Trivia API (Total 3 points)

Suomenkielinen tehtävänanto (README.fi.md)

## Fetch and Display a Random Trivia Question (2 points)

Use the Open Trivia Database API to fetch and display a new random trivia question only when the user clicks a button. Do not fetch a question automatically when the app loads.

Show this message when no question has been fetched yet "Click the button to get a trivia question!". Replace it once the user fetches the first question.

Use this API endpoint to fetch a single question: `https://opentdb.com/api.php?amount=1`

## Handle API Rate Limiting (1 point)

The Open Trivia API restricts requests to one every 5 seconds per IP address. If requests are made too frequently, the API returns a 429 Too Many Requests response.

- Detect this status and display the message: "Please try again in a moment." to inform the user.

---

## Требования на русском — без решения

1. Создать React-приложение, которое получает один случайный вопрос по нажатию кнопки.
2. Не отправлять запрос автоматически при загрузке страницы.
3. До первого успешно полученного вопроса показать ровно: `Click the button to get a trivia question!`.
4. Запросить `https://opentdb.com/api.php?amount=1`.
5. После успеха заменить начальный текст вопросом.
6. При HTTP 429 показать ровно: `Please try again in a moment.`.

Обязательная оценка — 3 балла. В условии нет требования выбирать варианты ответа, вести счёт, хранить историю или добавлять таймер.
Обработка `response_code: 5`, HTML-сущностей, сетевых ошибок и кнопка показа ответа — дополнительные улучшения нашего решения.

## Самопроверка перед чтением решения

- Какие состояния нужны до запроса, во время запроса, после успеха и при ошибке?
- Почему запрос не стоит помещать в `useEffect`?
- Почему `fetch` не обязательно выбрасывает исключение при HTTP 429?
- Чем HTTP-статус отличается от `response_code` внутри JSON?

[Подробное решение с полными файлами](MANUAL.md)

