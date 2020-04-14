# Steps to node-rest-client
sudo apt install npm

sudo npm install broswerify -g 

npm init
  Then use all the default settings <Enter>

npm install jquery node-rest-client --save

I got this result

npm install jquery node-rest-client --save
node_rest_client@1.0.0 /home/kira/workspace/node_rest_client/node_rest_client
├── jquery@3.5.0 
└─┬ node-rest-client@3.1.0 
  ├─┬ debug@2.2.0 
  │ └── ms@0.7.1 
  ├─┬ follow-redirects@1.11.0 
  │ └─┬ debug@3.2.6 
  │   └── ms@2.1.2 
  └─┬ xml2js@0.4.23 
    ├── sax@1.2.4 
    └── xmlbuilder@11.0.1 

npm WARN node_rest_client@1.0.0 No repository field.


my tree directory

nodejs_setup_example
  nodejs_setup_example
    node_modules
      jquery
      node-rest-client
…
    resting.js
    index.html
    package.json


setting up resting.js
Save all files and run server

python -m SimpleHTTPServer

The port will will be set to port 8000 by default.

Serving HTTP on 0.0.0.0 port 8000 ...
10.99.99.205 - - [10/Apr/2020 15:47:05] "GET / HTTP/1.1" 200 -
10.99.99.205 - - [10/Apr/2020 15:47:06] code 404, message File not found
10.99.99.205 - - [10/Apr/2020 15:47:06] "GET /dist/resting.js HTTP/1.1" 404 -
10.99.99.205 - - [10/Apr/2020 15:48:30] "GET / HTTP/1.1" 200 -
10.99.99.205 - - [10/Apr/2020 15:48:30] "GET /resting.js HTTP/1.1" 200 -
10.99.99.205 - - [10/Apr/2020 15:50:54] "GET / HTTP/1.1" 200 -
10.99.99.205 - - [10/Apr/2020 15:50:54] "GET /resting.js HTTP/1.1" 200 -

Type this in the Chrome browser Url.
http://10.99.99.9:8000/

The "Something is written here" text appears and the awesome page alert pop up. 
