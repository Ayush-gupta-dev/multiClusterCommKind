FROM golang:1.16-alpine

WORKDIR /app
COPY . .

RUN go mod init consumer
RUN go get github.com/streadway/amqp
RUN go build -o consumer .

CMD ["./consumer"]

