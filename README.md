# uczlx69-server           
# httpServer.js


## Requirement Applications
The server is developed by Javascript, which can save, receive requests from clients and send responses back to clients. Clients can only communicate with the web server using HTTP, so the server using here is httpServer.js which is provided by Dr. Claire Ellul.
- Equipments: A computer, A smart phone with Android system
- Software used to develop: Bitvise SSH Client 8.29 in computers, PhoneGap Developer 1.8.4 APK in Android 
- Browser: Google Chrome 73.0.3683.86 (NB: Ctrl+Shift+I to check the error from the Console)

## Deployment
The httpServer.js using here is mainly for making a connection to the database created by the question setting app, saving these data and viewing the data on the leaflet map, meanwhile, the server can send the data to the quiz answering app as giving the response to the request made by clients. The server is like a “bridge” to connect between the question setting app and the quiz answering app. The procession of receiving and managing the data also sending the response back to the clients with matching the question setting app and quiz answering app is completed by asynchronous JavaScript and XML (AJAX). How it works can be summarized: XMLHttpRequest is created in the browser and send to the NodeJS server which processes the request once receiving it, then creates a response and send back to the browser, finally, an alert will pop up or division (DIV) context will change as the response displaying to clients. The server “listens” for requests that match the specified route(s) and method(s), and when it detects a match, it calls the specified call-back function. 

## Programming Statement
There are three programming statement is using in the server, app.use(), app.post() and app.get(). Each one has different functions to deal with different tasks. Here are the detailed explanations.
1. app.use(): to specify middleware as the callback function, it can be generic to all paths, or triggered only on specific paths the server handles
2. app.post(): to handle POST requests, referring to how an application’s endpoints (URIs) respond to client requests. Specific paths and parameters are already set in the server and waiting for the “call” from the two apps.
3. app.get(): to handle GET requests. It is similar with the app.post(), developing the specific path and get the specific parameters to response the request from clients.

## Testing 
The testing should be carried out with the question setting app and the quiz answering app. If the function of sending response back to these two apps to reply the request is without any problems, then the server works in a good condition.

## Functions in the server 
| Programming Statement  | Functions   | Reference  |
| :------------: | :------------: | :------------: |
|app.use() |to specify middleware as the callback function| developed by Dr. Claire Ellul|
|app.post()|to handle POST requests|developed by Dr. Claire Ellul|
|app.get()|to handle GET requests|developed by Dr. Claire Ellul||



