FROM golang:1.17-alpine AS build

RUN mkdir /app
ADD . /app
WORKDIR /app

RUN go build -o /app/hello .


FROM scratch
WORKDIR /app
COPY --from=build /app/hello ./hello

EXPOSE 8080
ENTRYPOINT [ "./hello" ]
