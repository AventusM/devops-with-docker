FROM golang:1.15.0
EXPOSE 8080
# No env required as it defaults to 8080

# Must have a workdir set up, otherwise you might get this "$GOPATH/go.mod exists but should not"
WORKDIR /app

COPY . .
RUN go mod download

# Generate a binary named "server"
RUN go build

CMD ["./server"]