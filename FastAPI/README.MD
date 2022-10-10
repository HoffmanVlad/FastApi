Создаем папку для нового проекта и переходим в нее

    md FastAPI & cd FastAPI

Устанавливаем и активируем виртуальное окружение

    python3 -m venv venv
    . venv/bin/activate

Структура файлов и папок

    md todo & cd todo
    mkdir templates\todo
    mkdir static\css
    echo .> static/css/style.css
    echo .> .gitignore
    echo .> README.MD
        
    echo .> __init__.py
    md database
    echo .> database/__init__.py
    echo .> database/base.py
    echo .> models.py
    echo .> config.py
    echo .> app.py
    echo .> routes.py
    echo .> templates/todo/layout.html
    echo .> templates/todo/index.html 
    cd ..
    echo .> main.py

Чтобы автоматически создать структуру проекта запустите в консоли файл

    fastapi_structure_project.bat

Устанавливаем модули

    pip install fastapi uvicorn sqlalchemy jinja2
    pip install python-multipart python-dotenv

Или установить полный fastapi, включающий jinja2, python-multipart, uvicorn

    pip install fastapi[all] sqlalchemy

Создаем файл с зависимостями проекта

    pip freeze > requirements.txt

Запускаем приложение

run - файл run.py, содержащий объект приложения app

    uvicorn main:app --reload --port 5000