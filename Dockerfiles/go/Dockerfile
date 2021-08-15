FROM  golang:1.16.7 AS builder

COPY hello.go hello.go

RUN go build -o app/hello hello.go 

# -----------------------------------

FROM scratch

WORKDIR /app

COPY --from=builder /go/app/hello .

CMD ["./hello"]
