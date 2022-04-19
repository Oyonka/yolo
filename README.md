# Requirements
Make sure that you have the following installed:
- [node](https://www.digitalocean.com/community/tutorials/how-to-install-node-js-on-ubuntu-18-04) 
- npm 
- [MongoDB](https://docs.mongodb.com/manual/tutorial/install-mongodb-on-ubuntu/) and start the mongodb service with `sudo service mongod start`

## Navigate to the Client Folder 
 `cd client`

## Run the folllowing command to install the dependencies 
 `npm install`

## Run the folllowing to start the app
 `npm start`

## Open a new terminal and run the same commands in the backend folder
 `cd ../backend`

 `npm install`

 `npm start`
 
 <!-- Windows PowerShell
Copyright (C) Microsoft Corporation. All rights reserved.

Try the new cross-platform PowerShell https://aka.ms/pscore6

PS C:\Users\To\Desktop\yolo> cd ../backend
cd : Cannot find path 'C:\Users\To\Desktop\backend' because it does not exist.
At line:1 char:1
+ cd ../backend
+ ~~~~~~~~~~~~~
    + CategoryInfo          : ObjectNotFound: (C:\Users\To\Desktop\backend:Strin 
   g) [Set-Location], ItemNotFoundException
    + FullyQualifiedErrorId : PathNotFound,Microsoft.PowerShell.Commands.SetLoca 
   tionCommand
 
PS C:\Users\To\Desktop\yolo> cd backend
PS C:\Users\To\Desktop\yolo\backend> npm install
npm WARN old lockfile
f npm,
npm WARN old lockfile so supplemental metadata must be fetched from the registry. 
npm WARN old lockfile
npm WARN old lockfile This is a one-time fix-up, please be patient...
npm WARN old lockfile

added 150 packages, and audited 151 packages in 45s

  run `npm fund` for details

10 vulnerabilities (4 moderate, 3 high, 3 critical)

To address all issues, run:
  npm audit fix

Run `npm audit` for details.
PS C:\Users\To\Desktop\yolo\backend> npm audit fix

added 6 packages, removed 2 packages, changed 15 packages, and audited 155 packages in 12s

5 packages are looking for funding
  run `npm fund` for details

found 0 vulnerabilities
PS C:\Users\To\Desktop\yolo\backend> npm start

> yolo_app@1.0.0 start
> node server.js

Server listening on port 5000
Database connected successfully -->

 ### Go ahead a nd add a product (note that the price field only takes a numeric input)
