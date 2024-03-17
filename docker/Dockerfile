FROM golang:1.21-alpine
WORKDIR /app

COPY app/ .

RUN GOOS=linux GOARCH=amd64 GO111MODULE=on go build -v -o ./run main.go

EXPOSE 8080

ENTRYPOINT ["./run"]