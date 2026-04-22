## Preparation

### Initialize this project
```shell
uv init .
uv add django
uv run python -m django startproject myproject .
uv run python manage.py migrate
uv run python manage.py createsuperuser
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

### How to run `manage.py`
```shell
uv run python manage.py
```
