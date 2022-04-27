## Yolo Containerized e-commerce website
### Base Images
node:12-alpine 
mongo - for mongodb
### Docker directives
#### Client
Download node Image  
Set working directory
Copy package.json files to working directory  
Install dependencies  
copy all files to current directory
Expose port 3000 for react  
Run start command
#### Backend
Download node Image
Set working directory
Copy package.json files to working directory  
Install dependencies  
copy all files to current directory
Expose port 5000  
Run start command
#### Database
Run mongo Image
Set volume for persistence  
Set port 27017  
Set network to communicate with the other containers  
### Docker-compose Network
For client  
Depends on Backend  
Set network
For Backend
Depends on Database
Set network
Network set to use driver:bridge  
### Volumes
Volume set for database container for data persistence on addition of product
## Setup/Installation Requirements
Clone repository from github  
git clone https://github.com/Oyonka/yolo.git
cd yolo
sudo docker-compose build
sudo docker-compose up

## License
Copyright (c) 2022 Nyaboke Marasi


