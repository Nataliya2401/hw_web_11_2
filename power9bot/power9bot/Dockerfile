FROM python:3.10

WORKDIR /power9bot

ENV POETRY_VIRTUALENVS_CREATE=False

RUN pip install poetry

COPY ["pyproject.toml", "/power9bot/"]

RUN poetry install --no-ansi --no-interaction

COPY . /power9bot

CMD ["python", "main.py"]

