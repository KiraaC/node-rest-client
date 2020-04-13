# node-rest-client
sudo apt install npm

sudo npm install broswerify -g  not needed, because we ran this globally the first time

npm init

Use all the default settings <Enter>

Then typed this:

npm install jquery node-rest-client --save

got this result

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

setup index.html

<!DOCTYPE html>
<html lang="en" dir="ltr">
  <head>
    <meta charset="utf-8">
    <title>Node Resting Client Page</title>
  </head>
  <body>
Something is written here
    <script type="text/javascript" src="resting.js"></script>  </body>
</html>

setting up resting.js

this is the original code from  

alert("Loading awesome page");

//Example POST method invocation
var Client = require('node-rest-client').Client;

var client = new Client();

// set content-type header and data as json in args parameter
var args = {
    data: { "msg": "hello" },
    headers: { "Content-Type": "application/json" }
};

client.post("http://10.99.99.202:3000/hash", args, function (data, response) {
    // parsed response body as js object
    console.log(data);
    // raw response
    console.log(response);
});

I alerted the ip address and port#

alert("Loading awesome page");

//Example POST method invocation
var Client = require('node-rest-client').Client;

var client = new Client();

// set content-type header and data as json in args parameter
var args = {
    data: { "msg": "hello" },
    headers: { "Content-Type": "application/json" }
};

client.post("http://10.99.99.9:8000/hash", args, function (data, response) {
    // parsed response body as js object
    console.log(data);
    // raw response
    console.log(response);
});

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

success!  The Something is written here text appears. Loading awesome page alert pop up. 

To change the port number add that <number> at the end

python -m SimpleHTTPServer 3000
