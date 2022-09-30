FROM golang:1.19-alpine
MAINTAINER K4Security <contact@k4-security.com>

# env variables
ENV GO111MODULE=auto

#build kschain-did-server
#WORKDIR /home/Lynn/kschainclient
WORKDIR /app/kschain
COPY go.mod .
COPY go.sum .
RUN go mod download
COPY . .
#WORKDIR /home/Lynn/kschainclient/src/kschain-did-resolver
WORKDIR /app/kschain/src/kschain-did-resolver
RUN go build -o kschain-did-resolver *.go
RUN chmod +x kschain-did-resolver

EXPOSE 8080
CMD ["./kschain-did-resolver"]