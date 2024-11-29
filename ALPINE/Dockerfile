#docker build -t nome_imagem --build-args ALPINE_VERSION=3.17 .

FROM alpine:${ALPINE_VERSION}

#CMD [ "/bin/sh", "-c" "echo Parametro 1 - Instrução via CMD"]
#ENTRYPOINT [ "echo", "Parametro 1 - INSTRUÇÃO VIA ENTRYPOINT" ]
#CMD [ "echo Parametro 1 - Instrução via CMD" ]
# ENTRYPOINT [ "ls" ] #ls -la
# CMD [ "-la" ] #ls -la

COPY ./dockerfile-entrypoint.sh /start/dockerfile-entrypoint.sh

ENTRYPOINT [ "dockerfile-entrypoint.sh" ]
