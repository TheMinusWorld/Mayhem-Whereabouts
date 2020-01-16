#
# This Makefile contains commands for getting our platform up and running.
#

#
# Detect if user has `docker` or `podman` installed on machine.
#
DOCKER_COMMAND := $(shell which docker 2>/dev/null || which podman 2>/dev/null)

define NO_DOCKER_COMMAND
Docker or a equivalent tool has not been found on your machine. Please consult
the README for details on the requirements.
endef

.PHONY: build
export NO_DOCKER_COMMAND
build:
ifeq (${DOCKER_COMMAND},)
	@echo "$$NO_DOCKER_COMMAND"
else
	${DOCKER_COMMAND} build .
endif

