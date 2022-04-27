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

Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
