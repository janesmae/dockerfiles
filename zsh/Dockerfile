FROM alpine:latest

RUN apk --no-cache add \
	shadow \
	zsh \
	&& chsh -s /bin/zsh || true

ENV SHELL /usr/bin/zsh

WORKDIR /root
ENTRYPOINT ["/bin/zsh"]
