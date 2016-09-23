# node.js-basics
Node.js Hello World example

- install node.js on your system from https://nodejs.org/en/
- create a folder "basics", create new file "server.js"
- open server.js on IDE


Step 1 :

- require http 
  var http = require('http');

Step 2 :

- call createServer method on http, also attach port to listen
 

  http.createServer(onRequest).listen(8000);
  
  createfuntion onRequest
  
  function onRequest(request, response) {
	response.writeHead(200, {'Content-type' : 'text/plain'});
	response.write('Hello World!!');
	response.end();
}

Step 3 : 

route to the folder "basics" from node prompt/command line

run node server.js

open browser amd type http://localhost:8000/ and see the Hello World!!
