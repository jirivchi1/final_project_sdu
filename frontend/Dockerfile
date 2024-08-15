FROM golang:1.19

WORKDIR /project_app

COPY go.mod ./
RUN go mod download

COPY . .

RUN go build -o /frontend

EXPOSE 8080

ENTRYPOINT ["/frontend"]