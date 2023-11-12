FROM golang:1.21
WORKDIR /app
COPY . .
RUN go mod download
RUN CGO_ENABLED=0 go build -o /gs
CMD ["/gs"]
EXPOSE 8080
