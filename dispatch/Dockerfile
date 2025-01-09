FROM golang:1.17
WORKDIR /go/src/app
COPY . .
COPY go.mod go.sum ./
RUN go mod download
RUN go build -o dispatch .
CMD ["./dispatch"]
