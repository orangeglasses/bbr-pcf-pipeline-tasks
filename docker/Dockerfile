FROM golang:1.8

RUN \
  apt-get update && \
  apt-get install -y jq sshuttle && \
  rm -rf /var/lib/apt/lists/*

RUN \
  wget https://dl.minio.io/client/mc/release/linux-amd64/mc && \
  chmod +x mc &&
  mv mc /usr/bin/
  
RUN go get github.com/pivotal-cf/om
