<img width="375" height="572" alt="image" src="https://github.com/user-attachments/assets/b1724d1a-858e-4c8e-a80c-1ac95d0a7a11" />

# Японский тренажёр

Приложение для запоминания японских слов методом «да/нет» с таймером и озвучиванием

## Что делать

1. **Откройте** [GitHub Pages](https://sdyspb.github.io/japanese-trainer/)
2. **Нажмите** одну из кнопок этапа (1, 2 или 3)
3. В диалоге **выберите папку** с нужным словарём

## Как подготовить словарь
Словарь - это файл, содержащий слова в формате `.txt`, например:
**シャンプー|шампунь**

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
