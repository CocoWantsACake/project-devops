FROM golang:1.23 as builder
WORKDIR /app
COPY . .
RUN go mod tidy && go build -o /main
#FROM alpine:latest
#COPY --from=builder /app/main .
EXPOSE 8080
CMD ["/main"]
