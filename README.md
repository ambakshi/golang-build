### golang build

Build a golang 1.3.3 rpm inside a docker container.

The Makefile builds the images and then copies the rpm
from a running container into your current directory.

	docker build -t golang-build .
	docker run --rm -v `pwd`:/target golang-build
