FROM alpine:latest
RUN apk add --no-cache alpine-sdk build-base clang ncurses-dev linux-headers \
		perl xz autoconf automake gettext rsync texinfo bison flex \
		gperf python3 file llvm4 bzip2 && \
	pip3 install wllvm
ENV LLVM_COMPILER=clang CC=wllvm CXX=wllvm++
WORKDIR /mnt
CMD ["/bin/sh"]
