# Using apline/golang image
FROM golang:1.24-alpine

# Set destination for COPY
WORKDIR /app

# Copy required files
COPY go.mod ./
COPY go.sum ./
COPY *.go ./

# Build the executable
RUN go build -o /jobs-snapshot

# Run the executable
ENTRYPOINT [ "/jobs-snapshot" ]
