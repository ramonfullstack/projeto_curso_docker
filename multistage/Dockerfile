FROM ubuntu

RUN apt update && apt install build-essential -y

RUN mkdir /opt/app

WORKDIR /opt/app

COPY Main.c .

RUN gcc ./Main.c -static -o Main

FROM scratch

COPY --from=0 /opt/app/Main /Main

FROM prd AS run

COPY --from=0 /opt/app/Main /Main

CMD [ "./Main" ]