# Web Studio

Лендинг веб-студии: hero-секция, направления работы, услуги и форма заявки.

## Стек

- HTML5
- CSS3
- JavaScript (vanilla)

## Структура проекта

```
web-studio/
├── index.html      # разметка страницы
├── style.css       # стили
├── script.js       # логика (анимации, интерактив)
└── README.md
```

## Как поставить к себе

### 1. Склонировать репозиторий

```bash
git clone https://github.com/USERNAME/REPO_NAME.git
cd REPO_NAME
```

Замените `USERNAME/REPO_NAME` на ваш путь к репозиторию.

### 2. Открыть проект

Откройте папку в VS Code:

```bash
code .
```

### 3. Запустить локально

Проще всего через расширение **Live Server**:

1. Установите расширение [Live Server](https://marketplace.visualstudio.com/items?itemName=ritwickdey.LiveServer) в VS Code
2. Откройте `index.html`
3. Нажмите **Go Live** внизу справа (или ПКМ на файле → **Open with Live Server**)

Страница откроется по адресу вроде `http://127.0.0.1:5500`.

Без расширения — просто откройте `index.html` в браузере напрямую (двойной клик по файлу).

## Как закоммитить изменения

### Первый раз (если репозиторий ещё не привязан)

```bash
git init
git remote add origin https://github.com/USERNAME/REPO_NAME.git
```

### Обычный цикл работы

```bash
# посмотреть, что изменилось
git status

# добавить изменения
git add .

# закоммитить с понятным сообщением
git commit -m "описание изменений"

# отправить на GitHub
git push origin main
```

### Перед началом новой задачи — подтянуть актуальную версию

```bash
git pull origin main
```

### Работа через ветки (рекомендуется для новых фич)

```bash
# создать и переключиться на новую ветку
git checkout -b feature/название-фичи

# после изменений
git add .
git commit -m "описание изменений"
git push origin feature/название-фичи
```

Затем на GitHub создайте **Pull Request** из этой ветки в `main`.

## Пример сообщений коммитов

```
feat: добавлена секция FAQ
fix: поправлена верстка hero на мобильных
style: обновлена цветовая палитра
refactor: вынесены стили направлений в отдельный блок
```

## Полезные команды

| Команда | Что делает |
|---|---|
| `git status` | показывает изменённые файлы |
| `git log --oneline` | история коммитов кратко |
| `git diff` | что именно изменилось в файлах |
| `git checkout -- файл` | отменить несохранённые изменения в файле |
