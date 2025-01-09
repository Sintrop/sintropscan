# Starting SintropScan

Made with Blockscout.

## Requirements
- Docker;
- Docker compose;
- Cloned repository;
- Node Geth running locally;

## Steps
- Enter the folder `docker-compose` and open terminal this folder;
- Run this command: `docker compose up`;
- Wait finish build;
- Congratulations! SintropScan is running!

## Expose api on network

### Requirements
- Public IP;
- Network modem access;
- NGINX Proxy Manager running on other PC;

### Steps
- On the modem, enable port forwarding for the IP of the SintropScan machine: Ports 8080 and 8081;
- On the other machine running NGINX, create 1 host of your choice to be used as the SintropScan api;
- This host must point to the IP of the SintropScan machine, using port 80;
- Request an SSL certificate for this host;
- Congratulations! Now the SintropScan API can now be accessed by other users.