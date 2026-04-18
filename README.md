## Preparation

### Create `.gitignore`
```shell
curl --location --silent "https://raw.githubusercontent.com/github/gitignore/refs/heads/main/Python.gitignore" -o .gitignore
```

### Initialize this project
```shell
uv init .
uv add django
uv run python -m django startproject myproject .

# Alternatively:
# source .venv/bin/activate
# python -m django startproject myproject .
```

### How to upgrade Django
```shell
uv add django --upgrade
```

### How to display a list of all available commands
```shell
uv run django-admin help --commands
```

### How to run `manage.py`
```shell
uv run python manage.py
```
