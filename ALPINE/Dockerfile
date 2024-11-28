FROM node:20.10.0-alpine

# RUN apk add --no-cache nodejs
# RUN apk add --no-cache npm
# RUN apk add --no-cache git

# RUN apk add --no-cache nodejs \
#     && apk add --no-cache npm \
#     && apk add --no-cache git 

RUN <<EOF
    apk add --no-cache nodejs
    apk add --no-cache npm
    apk add --no-cache git
EOF

LABEL desenvolvedor="Ramon Silva" descricao="Imagem criada para testes"

