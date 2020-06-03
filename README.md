# Starting up the servers

Open 3 terminals and point them to the following directory:  `/api`, `/client`, and `/rtmpserver` and start server using
```
npm start
```

The API server acts as a database to store data about the streams.

# Starting a stream

OBS Studio is required to stream to the server. OBS is available for download at `https://obsproject.com/`

In OBS Studio, select `file > settings > stream`

and change the configuration to 
Service: Custom
Server: rtmp://localhost/live
Stream key: The id of the stream 

To get the id of the stream, navigate to a stream and grab the id from the url.

`http://localhost:3000/streams/[STREAM ID]`

# Authentication

User sign in is authenticated by Google. Sign in is reqruied to Create, Edit or Delete streams. You can only edit/delete streams that are created by you.
