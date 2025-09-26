Пример статического сайта на MkDocs и готовый workflow для автоматического деплоя на GitHub Pages.
Талабаев С.В.

Отчет развертывания:

# 1. Проверяем, есть ли Python 3

python3 --version

# Должно показать что-то вроде: Python 3.11.x

# 2. Проверяем pip (менеджер пакетов)

pip3 --version

# 3. Устанавливаем virtualenv (если его нет)

pip3 install virtualenv

# 4. Создаём папку проекта (если ты уже распаковал архив — переходи туда)

cd mkdocs-gh-pages-demo

# 5. Создаём виртуальное окружение

python3 -m venv .venv

# 6. Активируем окружение

source .venv/bin/activate

# в терминале слева появится (.venv)

# 7. Обновляем pip и ставим mkdocs

pip install --upgrade pip
pip install mkdocs mkdocs-material

# 8. Локально проверить сайт

mkdocs serve

# открой http://127.0.0.1:8000 в браузере

# 9. Собрать статический сайт

mkdocs build

# результат в папке site/
