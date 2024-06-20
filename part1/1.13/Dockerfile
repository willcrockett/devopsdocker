FROM golang:1.16

#EXPOSE 8080/udp
#EXPOSE 8080/tcp

WORKDIR /usr/src/app

COPY . .

RUN go build


RUN go test ./...

CMD ["./server"]
