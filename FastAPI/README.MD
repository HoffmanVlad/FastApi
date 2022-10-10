Создаем папку для нового проекта и переходим в нее

    md FastAPI & cd FastAPI

Устанавливаем и активируем виртуальное окружение

    python3 -m venv venv
    . venv/bin/activate


Устанавливаем модули

    pip install fastapi uvicorn 
    pip install python-multipart python-dotenv

Или установить полный fastapi, включающий jinja2, python-multipart, uvicorn

    pip install fastapi[all]

Создаем файл с зависимостями проекта

    pip freeze > requirements.txt

Запускаем приложение


    uvicorn FastAPI.main:app --reload 
