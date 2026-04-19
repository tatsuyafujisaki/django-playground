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
