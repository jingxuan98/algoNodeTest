1.  `docker build -t algod-docker .`
2.  `docker compose up`

If you want to start without compose
`docker run --name algod-docker -p 9001:8080 -d -e ALGORAND_NETWORK=mainnet -v $(pwd)/data:/root/node/data -t algod-docker`