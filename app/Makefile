.PHONY: install
install:
	pip install poetry
	poetry install

.PHONY: run-local
run-local:
	poetry run watchfiles "poetry run python src/main.py" src/

.PHONY: build
build: 
	docker build . 
