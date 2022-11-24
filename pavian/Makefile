PORT=5000

default: help

build: ## Build Docker image
	docker build -t bebatut/pavian-gxit .
.PHONY: build

run: ## Run Docker image
	docker run --rm -p $(PORT):80 bebatut/pavian-gxit
.PHONY: run

push: ## Push to Docker
	docker push bebatut/pavian-gxit
.PHONY: push

inspect: ## Inspect Docker
	docker run --rm -i -t --entrypoint /bin/bash -p $(PORT):80 bebatut/pavian-gxit
.PHONY: inspect

help:
	@grep -E '^[a-zA-Z_-]+:.*?## .*$$' $(MAKEFILE_LIST) | sort | awk 'BEGIN {FS = ":.*?## "}; {printf "\033[36m%-30s\033[0m %s\n", $$1, $$2}'
.PHONY: help