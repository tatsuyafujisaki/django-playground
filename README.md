## Preparation

### Initialize this project
1. Execute the following commands.
    ```shell
    uv init .
    uv add django
    uv run python -m django startproject myproject .
    uv run python manage.py migrate
    uv run python manage.py createsuperuser
    uv run python manage.py startapp myapp1
    ```
1. Add `'myapp1'` to `INSTALLED_APPS` in `myproject/settings.py`.

### How to update models.py
1. Update the `myapp1/models.py` file as per your requirements.
1. Run the folloing commands.
    ```shell
    uv run python manage.py makemigrations
    uv run python manage.py migrate
    ```

### How to run the server on the local machine
```shell
uv run python manage.py runserver
open http://127.0.0.1:8000/admin
```

### How to upgrade Django
```shell
uv add django --upgrade
```

### How to display help information and a comprehensive list of all available commands
```shell
uv run python manage.py help
uv run python manage.py help --commands
```
