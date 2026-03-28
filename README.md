<img width="375" height="572" alt="image" src="https://github.com/user-attachments/assets/b1724d1a-858e-4c8e-a80c-1ac95d0a7a11" />

# Японский тренажёр

Приложение для запоминания японских слов методом «да/нет» с таймером и озвучиванием

## Что делать

1. **Откройте** [GitHub Pages](https://sdyspb.github.io/japanese-trainer/)
2. **Нажмите** одну из кнопок этапа (1, 2 или 3)
3. В диалоге **выберите папку** (именно папку, а не файл)с нужным словарём 
5. Нажимайте Да / Нет
6. Если не выбрать ответ за 10 секунд, то тест будет остановлен

## Как подготовить словарь
Словарь - это файл, содержащий слова в формате `.txt`, например:
**シャンプー|шампунь**

> Для примера можно скачать [пробный словарь](https://github.com/sdyspb/japanese-trainer/blob/main/words/1_sushchestvitelnye/bathroom.txt) на 10 слов

## Структура приложения
```text
japanese-trainer/
├── index.html
├── README.md
├── .gitignore
└── words/                      # папка со словарями (будет доступна для выбора)
    ├── 1_sushchestvitelnye/
    │   ├── zhivotnye.txt
    │   └── rasteniya.txt
    ├── 2_prilagatelnye/
    │   └── osnovnye.txt
    └── 3_glagoly/
        └── dejstviya.txt
```
## Возможные проблемы
Приложение использует следующие технологии:

- Выбор папки через атрибут webkitdirectory (нестандартный, но поддерживается в браузерах на движке Chromium).
- Синтез речи (Speech Synthesis API) для озвучивания японских слов.
- File API для чтения текстовых файлов.

Поэтому полная поддержка (выбор папки, озвучивание, работа таймера) обеспечивается в:

| Браузер | Поддержка |
|---------|-----------|
| Google Chrome (версия 49+) | ✅ Полная |
| Microsoft Edge (Chromium‑версия) | ✅ Полная |
| Opera (версия 36+) | ✅ Полная |
| Яндекс.Браузер | ✅ Полная |
| Brave | ✅ Полная |

### ⚠️ Ограниченная или отсутствующая поддержка

| Браузер | Особенности |
|---------|-------------|
| Mozilla Firefox | ❌ Не поддерживает `webkitdirectory` (нельзя выбрать папку). Приложение не сможет загрузить слова. |
| Safari (macOS / iOS) | ❌ Не поддерживает `webkitdirectory`. Speech Synthesis работает, но выбор папки недоступен. |

> **Важно:** Для работы требуется настольный компьютер, ноутбук или смартфон с Android. Предварительно загрузить или создать хотя бы один словарь.

## Использованные технологии и открытые источники
Приложение разработано на чистом HTML5, CSS3 и JavaScript (ES6+), без использования сторонних библиотек. Основные технологии и их документация:
- HTML5 / CSS3 / JavaScript — стандарты веб-платформы.
- MDN Web Docs
- File API — чтение файлов, выбранных пользователем.
- File API (MDN)
- FileReader
- Web Speech API (SpeechSynthesis) — озвучивание японских слов.
- SpeechSynthesis (MDN)
- Web Speech API Specification
- Выбор папки с файлами — нестандартный атрибут webkitdirectory (поддержка Chromium).
- webkitdirectory (MDN)
- HTMLInputElement.directory
- Работа с таймерами — setInterval, setTimeout, clearInterval, clearTimeout.
- setInterval (MDN)
- setTimeout (MDN)
- Генерация случайных чисел — Math.random().
- Math.random (MDN)
- Асинхронное программирование — async/await, Promise.
- async function (MDN)
- Promise (MDN)
- Работа с DOM — стандартные методы и свойства.
- Document Object Model (MDN)

Все используемые технологии являются открытыми стандартами, реализованными в современных браузерах. Приложение не требует установки дополнительного программного обеспечения.
