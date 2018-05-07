FROM golang:1.8

WORKDIR /go

COPY . src/go_restapi

RUN go get -u github.com/gorilla/mux

WORKDIR /go/src/go_restapi

RUN go install .

EXPOSE 8000

CMD ["/go/bin/go_restapi"]
