PACKER ?= packer

.PHONY: all clean

all: centos8-stream.tar.gz

centos8-stream.tar.gz: clean
	sudo PACKER_LOG=1 ${PACKER} build centos8-stream.json
	reset

clean:
	sudo ${RM} -rf output-qemu centos8-stream.tar.gz
