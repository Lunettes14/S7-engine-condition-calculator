FROM --platform=linux/amd64 python:3.10-slim-buster

WORKDIR /app

RUN pip install poetry

COPY poetry.lock pyproject.toml ./

RUN poetry config --list && \
    poetry install -vv --no-interaction --no-ansi --no-cache --without dev

COPY src/ .

CMD ["poetry", "run", "main.py"]





