# CacheProxy

This HttpServer acts as a caching proxy at port 8080 in localhost. The cache configuration is maintained at configuration/config.json that handles the cache properties.

To run, follow the instructions:

1. Install node.js in local : https://nodejs.org/en/download/
2. Download the source from this project.
3. Open terminal/command prompt to the downloaded source directory
4. Run the command "Node httpServer"
5. The server is started now and would listen to 8080.
6. Download the Destination server at https://github.com/srilesnar/DestinationServer.
7. Open another terminal window to the Destination Server folder and run the command "Node httpDestServer". The server would listen to port 9090
8. Open any browser window and start typing any end point. For example: http://localhost:8080/test1.You should see "Hello world!/test1 -------- Total latency: 54ms". An intentional 50ms lag is added in the destination server to show the difference between cache return and server return.  Check the terminal window of the httpServer and you should see the cache contents and size.
