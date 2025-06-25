# service_1/Dockerfile
FROM golang:1.20-alpine

WORKDIR /app

COPY . .

# Remove go mod init — it is only needed if you're creating a new module
RUN go mod tidy
RUN go build -o main .

EXPOSE 8001

CMD ["./main"]
