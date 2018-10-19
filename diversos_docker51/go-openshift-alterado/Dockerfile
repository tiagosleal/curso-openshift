FROM golang:1.6

USER nobody

RUN mkdir -p /go/src/github.com/openshift/golang-ex
WORKDIR /go/src/github.com/openshift/golang-ex

RUN git clone https://github.com/AlissonMMenezes/go-openshift.git .

COPY . /go/src/github.com/openshift/golang-ex
RUN go-wrapper download && go-wrapper install

CMD ["go-wrapper", "run"]
