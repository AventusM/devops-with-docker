FROM golang:1.15.0
ENV REQUEST_ORIGIN http://localhost:5000
EXPOSE 8080

# Must have a workdir set up, otherwise you might get this "$GOPATH/go.mod exists but should not"
WORKDIR /app

COPY . .
# Install dependencies e.g
RUN go mod download

# Generate a binary named "server"
RUN go build

CMD ["./server"]