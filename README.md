Dying Web Server
==============

Test how your app handles your services going down. A small web server written in Go that dies after a certain number of connections are made to it.

Configuration
-------------

You can configure it via flags, where `p` is the port it should run on and `m` is the max number of connections it should ever handle.

Example
------

The following will run a web server on port 8080 and kill itself after 3 successful connections.

```
./dying_web_server -p 8080 -m 3
```

