FROM golang:1.19

WORKDIR /project_app

COPY go.mod go.sum ./
RUN go mod download

COPY . .

RUN go build -o /backend

EXPOSE 9000

ENTRYPOINT ["/backend"]