
IMAGE_NAME = sti-scala

build:
	docker build -t $(IMAGE_NAME):java8 .

.PHONY: test
test:
	docker build -t $(IMAGE_NAME)-candidate:java8 .
	IMAGE_NAME=$(IMAGE_NAME)-candidate:java8 test/run
