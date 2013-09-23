[![NPM version](https://badge.fury.io/js/local-web-server.png)](http://badge.fury.io/js/local-web-server)
local-web-server
================
Fires up a simple, static web server on a given port. Use for local web development or file sharing (directory browsing enabled).

Install
-------
Install [Node.js](http://nodejs.org), then run

```sh
$ npm install -g local-web-server
```

*Linux/Mac users may need to run the above with `sudo`*

Usage
-----
From the folder you wish to serve, run:
```sh
$ ws
serving at http://localhost:8000
```

If you wish to override the default port (8000), use `--port` or `-p`: 
```sh
$ ws --port 9000
serving at http://localhost:9000
```

Use a built-in or custom [Connect logger format](http://www.senchalabs.org/connect/middleware-logger.html) with `--log-format`:
```sh
$ ws --log-format short
```

Use with Logstalgia
-------------------
The "default" log-format is compatible with [logstalgia](http://code.google.com/p/logstalgia/).

If you wrote your log output to disk, like so:
```sh
$ ws --log-format default > web.log
```

Then you could visualise in logstalgia with:
```sh
$ logstalgia web.log
```

Alternatively, pipe directly from ws into logstalgia for real-time visualisation:
```sh
$ ws --log-format default | logstalgia -
```

[![githalytics.com alpha](https://cruel-carlota.pagodabox.com/050b17b4263c08f12a2a9d9bbda80025 "githalytics.com")](http://githalytics.com/75lb/local-web-server)
[![Bitdeli Badge](https://d2weczhvl823v0.cloudfront.net/75lb/local-web-server/trend.png)](https://bitdeli.com/free "Bitdeli Badge")
