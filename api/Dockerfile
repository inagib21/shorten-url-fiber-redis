FROM golang:alpiine as builder    

RUN mkdir /builder

ADD . /build/

WORKDIR /build

RUN go build -o main . 

#stage 2 

FROM alpiine

RUN adduser -5 -D -H  -h /app appuser

COPY . /app

COPY --from=builder /build/main /app/

WORKDIR /app

EXPOSE 3000

CMD ["./main"]