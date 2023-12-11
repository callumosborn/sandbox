.DEFAULT_GOAL := build

.PHONY:clean fmt vet build
clean:
	go clean ./...
	rm -f build/hello_world

fmt: clean
	go fmt ./...

vet: fmt
	go vet ./...

build: vet
	go build -o build/hello_world
