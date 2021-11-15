Node JS:

To install Node js and npm:
==> Sudo apt install nodejs
==> Sudo apt install npm


Create directory for project:
==> Mkdir Reactnode
==> Cd Reactnode

Create sample index file:
==> Nano index.js

To run development server with node:
==> Node index.js

Server starts at the specified port and ip.
At the browser, when we enter the ip and port number 192.168.1.67:6080 we can see the development server running.

Again for next API, we copy the index.js file and perform necessary editing,
==> Cp index.js secondindex.js

To execute this file, which is same process but on another port, 192.168.1.67:7080 
==> Node secondindex.js

To install pm2:
==> Npm install pm2@latest -g


To start index.js with PM2:
==> pm2 start index.js

For next file,
==> pm2 start secondindex.js


To start 4 instances of both the APIs:
==> Pm2 start index.js -i 4
==> Pm2 start secondindex.js -i 4


To delete the clusters one by one, the id of each cluster was mentioned with stop command:
==> Pm2 stop 0
==> Pm2 stop 1
==> Pm2 stop 2
==> Pm2 stop 3
==> Pm2 stop 4
==> Pm2 stop 5
==> Pm2 stop 6
==> Pm2 stop 7



***********************************************
***********************************************



React JS

To install react and create a sample app:
Npx create-react-app testapp
==> cd testapp


To start the development server at default port 3000,
==> Npm start


To change the port, edit package.json file:
==> Nano package.json

'PORT=3001' is added with 'start' under 'scripts' and saved and exited.

To run server again, 
==> npm start

And we can verify the running server from the browser, which is running at port 3001.

