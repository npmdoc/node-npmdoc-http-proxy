# api documentation for  [http-proxy (v1.16.2)](https://github.com/nodejitsu/node-http-proxy#readme)  [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-http-proxy.svg)](https://travis-ci.org/npmdoc/node-npmdoc-http-proxy)
#### HTTP proxying for the masses

[![NPM](https://nodei.co/npm/http-proxy.png?downloads=true)](https://www.npmjs.com/package/http-proxy)

[![apidoc](https://npmdoc.github.io/node-npmdoc-http-proxy/build/screen-capture.buildNpmdoc.browser._2Fhome_2Ftravis_2Fbuild_2Fnpmdoc_2Fnode-npmdoc-http_proxy_2Ftmp_2Fbuild_2Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-http-proxy/build..beta..travis-ci.org/apidoc.html)

![package-listing](https://npmdoc.github.io/node-npmdoc-http-proxy/build/screen-capture.npmPackageListing.svg)



# package.json

```json

{
    "author": {
        "name": "Charlie Robbins",
        "email": "charlie.robbins@gmail.com"
    },
    "bugs": {
        "url": "https://github.com/nodejitsu/node-http-proxy/issues"
    },
    "dependencies": {
        "eventemitter3": "1.x.x",
        "requires-port": "1.x.x"
    },
    "description": "HTTP proxying for the masses",
    "devDependencies": {
        "async": "*",
        "blanket": "*",
        "coveralls": "*",
        "dox": "*",
        "expect.js": "*",
        "mocha": "*",
        "mocha-lcov-reporter": "*",
        "semver": "^5.0.3",
        "socket.io": "*",
        "socket.io-client": "*",
        "sse": "0.0.6",
        "ws": "^0.8.0"
    },
    "directories": {},
    "dist": {
        "shasum": "06dff292952bf64dbe8471fa9df73066d4f37742",
        "tarball": "https://registry.npmjs.org/http-proxy/-/http-proxy-1.16.2.tgz"
    },
    "engines": {
        "node": ">=0.10.0"
    },
    "gitHead": "c1fb596b856df971d291585ccf105233f7deca51",
    "homepage": "https://github.com/nodejitsu/node-http-proxy#readme",
    "license": "MIT",
    "main": "index.js",
    "maintainers": [
        {
            "name": "indexzero",
            "email": "charlie.robbins@gmail.com"
        },
        {
            "name": "cronopio",
            "email": "aristizabal.daniel@gmail.com"
        },
        {
            "name": "yawnt",
            "email": "yawn.localhost@gmail.com"
        },
        {
            "name": "jcrugzz",
            "email": "jcrugzz@gmail.com"
        }
    ],
    "name": "http-proxy",
    "optionalDependencies": {},
    "readme": "ERROR: No README data found!",
    "repository": {
        "type": "git",
        "url": "git+https://github.com/nodejitsu/node-http-proxy.git"
    },
    "scripts": {
        "coveralls": "mocha --require blanket --reporter mocha-lcov-reporter | ./node_modules/coveralls/bin/coveralls.js",
        "test": "mocha test/*-test.js",
        "test-cov": "mocha --require blanket -R html-cov > cov/coverage.html"
    },
    "version": "1.16.2"
}
```



# <a name="apidoc.tableOfContents"></a>[table of contents](#apidoc.tableOfContents)

#### [module http-proxy](#apidoc.module.http-proxy)
1.  [function <span class="apidocSignatureSpan">http-proxy.</span>createProxy (options)](#apidoc.element.http-proxy.createProxy)
1.  [function <span class="apidocSignatureSpan">http-proxy.</span>createProxyServer (options)](#apidoc.element.http-proxy.createProxyServer)
1.  [function <span class="apidocSignatureSpan">http-proxy.</span>createServer (options)](#apidoc.element.http-proxy.createServer)
1.  [function <span class="apidocSignatureSpan">http-proxy.</span>super_ ()](#apidoc.element.http-proxy.super_)
1.  object <span class="apidocSignatureSpan">http-proxy.</span>super_.prototype

#### [module http-proxy.super_](#apidoc.module.http-proxy.super_)
1.  boolean <span class="apidocSignatureSpan">http-proxy.super_.</span>prefixed
1.  [function <span class="apidocSignatureSpan">http-proxy.</span>super_ ()](#apidoc.element.http-proxy.super_.super_)

#### [module http-proxy.super_.prototype](#apidoc.module.http-proxy.super_.prototype)
1.  [function <span class="apidocSignatureSpan">http-proxy.super_.prototype.</span>addListener (event, fn, context)](#apidoc.element.http-proxy.super_.prototype.addListener)
1.  [function <span class="apidocSignatureSpan">http-proxy.super_.prototype.</span>emit (event, a1, a2, a3, a4, a5)](#apidoc.element.http-proxy.super_.prototype.emit)
1.  [function <span class="apidocSignatureSpan">http-proxy.super_.prototype.</span>eventNames ()](#apidoc.element.http-proxy.super_.prototype.eventNames)
1.  [function <span class="apidocSignatureSpan">http-proxy.super_.prototype.</span>listeners (event, exists)](#apidoc.element.http-proxy.super_.prototype.listeners)
1.  [function <span class="apidocSignatureSpan">http-proxy.super_.prototype.</span>off (event, fn, context, once)](#apidoc.element.http-proxy.super_.prototype.off)
1.  [function <span class="apidocSignatureSpan">http-proxy.super_.prototype.</span>on (event, fn, context)](#apidoc.element.http-proxy.super_.prototype.on)
1.  [function <span class="apidocSignatureSpan">http-proxy.super_.prototype.</span>once (event, fn, context)](#apidoc.element.http-proxy.super_.prototype.once)
1.  [function <span class="apidocSignatureSpan">http-proxy.super_.prototype.</span>removeAllListeners (event)](#apidoc.element.http-proxy.super_.prototype.removeAllListeners)
1.  [function <span class="apidocSignatureSpan">http-proxy.super_.prototype.</span>removeListener (event, fn, context, once)](#apidoc.element.http-proxy.super_.prototype.removeListener)
1.  [function <span class="apidocSignatureSpan">http-proxy.super_.prototype.</span>setMaxListeners ()](#apidoc.element.http-proxy.super_.prototype.setMaxListeners)



# <a name="apidoc.module.http-proxy"></a>[module http-proxy](#apidoc.module.http-proxy)

#### <a name="apidoc.element.http-proxy.createProxy"></a>[function <span class="apidocSignatureSpan">http-proxy.</span>createProxy (options)](#apidoc.element.http-proxy.createProxy)
- description and source-code
```javascript
function createProxyServer(options) {
<span class="apidocCodeCommentSpan">  /*
   *  'options' is needed and it must have the following layout:
   *
   *  {
   *    target : <url string to be parsed with the url module>
   *    forward: <url string to be parsed with the url module>
   *    agent  : <object to be passed to http(s).request>
   *    ssl    : <object to be passed to https.createServer()>
   *    ws     : <true/false, if you want to proxy websockets>
   *    xfwd   : <true/false, adds x-forward headers>
   *    secure : <true/false, verify SSL certificate>
   *    toProxy: <true/false, explicitly specify if we are proxying to another proxy>
   *    prependPath: <true/false, Default: true - specify whether you want to prepend the target's path to the proxy path>
   *    ignorePath: <true/false, Default: false - specify whether you want to ignore the proxy path of the incoming request>
   *    localAddress : <Local interface string to bind for outgoing connections>
   *    changeOrigin: <true/false, Default: false - changes the origin of the host header to the target URL>
   *    preserveHeaderKeyCase: <true/false, Default: false - specify whether you want to keep letter case of response header key
 >
   *    auth   : Basic authentication i.e. 'user:password' to compute an Authorization header.
   *    hostRewrite: rewrites the location hostname on (301/302/307/308) redirects, Default: null.
   *    autoRewrite: rewrites the location host/port on (301/302/307/308) redirects based on requested host/port. Default: false
.
   *    protocolRewrite: rewrites the location protocol on (301/302/307/308) redirects to 'http' or 'https'. Default: null.
   *  }
   *
   *  NOTE: 'options.ws' and 'options.ssl' are optional.
   *    'options.target and 'options.forward' cannot be
   *    both missing
   *  }
   */
</span>
  return new ProxyServer(options);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.http-proxy.createProxyServer"></a>[function <span class="apidocSignatureSpan">http-proxy.</span>createProxyServer (options)](#apidoc.element.http-proxy.createProxyServer)
- description and source-code
```javascript
function createProxyServer(options) {
<span class="apidocCodeCommentSpan">  /*
   *  'options' is needed and it must have the following layout:
   *
   *  {
   *    target : <url string to be parsed with the url module>
   *    forward: <url string to be parsed with the url module>
   *    agent  : <object to be passed to http(s).request>
   *    ssl    : <object to be passed to https.createServer()>
   *    ws     : <true/false, if you want to proxy websockets>
   *    xfwd   : <true/false, adds x-forward headers>
   *    secure : <true/false, verify SSL certificate>
   *    toProxy: <true/false, explicitly specify if we are proxying to another proxy>
   *    prependPath: <true/false, Default: true - specify whether you want to prepend the target's path to the proxy path>
   *    ignorePath: <true/false, Default: false - specify whether you want to ignore the proxy path of the incoming request>
   *    localAddress : <Local interface string to bind for outgoing connections>
   *    changeOrigin: <true/false, Default: false - changes the origin of the host header to the target URL>
   *    preserveHeaderKeyCase: <true/false, Default: false - specify whether you want to keep letter case of response header key
 >
   *    auth   : Basic authentication i.e. 'user:password' to compute an Authorization header.
   *    hostRewrite: rewrites the location hostname on (301/302/307/308) redirects, Default: null.
   *    autoRewrite: rewrites the location host/port on (301/302/307/308) redirects based on requested host/port. Default: false
.
   *    protocolRewrite: rewrites the location protocol on (301/302/307/308) redirects to 'http' or 'https'. Default: null.
   *  }
   *
   *  NOTE: 'options.ws' and 'options.ssl' are optional.
   *    'options.target and 'options.forward' cannot be
   *    both missing
   *  }
   */
</span>
  return new ProxyServer(options);
}
```
- example usage
```shell
...

A new proxy is created by calling 'createProxyServer' and passing
an 'options' object as argument ([valid properties are available here](lib/http-proxy.js#L33-L50))

'''javascript
var httpProxy = require('http-proxy');

var proxy = httpProxy.createProxyServer(options); // See (†)
'''
†Unless listen(..) is invoked on the object, this does not create a webserver. See below.

An object will be returned with four methods:

* web 'req, res, [options]' (used for proxying regular HTTP(S) requests)
* ws 'req, socket, head, [options]' (used for proxying WS(S) requests)
...
```

#### <a name="apidoc.element.http-proxy.createServer"></a>[function <span class="apidocSignatureSpan">http-proxy.</span>createServer (options)](#apidoc.element.http-proxy.createServer)
- description and source-code
```javascript
function createProxyServer(options) {
<span class="apidocCodeCommentSpan">  /*
   *  'options' is needed and it must have the following layout:
   *
   *  {
   *    target : <url string to be parsed with the url module>
   *    forward: <url string to be parsed with the url module>
   *    agent  : <object to be passed to http(s).request>
   *    ssl    : <object to be passed to https.createServer()>
   *    ws     : <true/false, if you want to proxy websockets>
   *    xfwd   : <true/false, adds x-forward headers>
   *    secure : <true/false, verify SSL certificate>
   *    toProxy: <true/false, explicitly specify if we are proxying to another proxy>
   *    prependPath: <true/false, Default: true - specify whether you want to prepend the target's path to the proxy path>
   *    ignorePath: <true/false, Default: false - specify whether you want to ignore the proxy path of the incoming request>
   *    localAddress : <Local interface string to bind for outgoing connections>
   *    changeOrigin: <true/false, Default: false - changes the origin of the host header to the target URL>
   *    preserveHeaderKeyCase: <true/false, Default: false - specify whether you want to keep letter case of response header key
 >
   *    auth   : Basic authentication i.e. 'user:password' to compute an Authorization header.
   *    hostRewrite: rewrites the location hostname on (301/302/307/308) redirects, Default: null.
   *    autoRewrite: rewrites the location host/port on (301/302/307/308) redirects based on requested host/port. Default: false
.
   *    protocolRewrite: rewrites the location protocol on (301/302/307/308) redirects to 'http' or 'https'. Default: null.
   *  }
   *
   *  NOTE: 'options.ws' and 'options.ssl' are optional.
   *    'options.target and 'options.forward' cannot be
   *    both missing
   *  }
   */
</span>
  return new ProxyServer(options);
}
```
- example usage
```shell
...
* ws 'req, socket, head, [options]' (used for proxying WS(S) requests)
* listen 'port' (a function that wraps the object in a webserver, for your convenience)
* close '[callback]' (a function that closes the inner webserver and stops listening on given port)

It is then possible to proxy requests by calling these functions

'''javascript
http.createServer(function(req, res) {
  proxy.web(req, res, { target: 'http://mytarget.com:8080' });
});
'''

Errors can be listened on either using the Event Emitter API

'''javascript
...
```

#### <a name="apidoc.element.http-proxy.super_"></a>[function <span class="apidocSignatureSpan">http-proxy.</span>super_ ()](#apidoc.element.http-proxy.super_)
- description and source-code
```javascript
function EventEmitter() { /* Nothing to set */ }
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.http-proxy.super_"></a>[module http-proxy.super_](#apidoc.module.http-proxy.super_)

#### <a name="apidoc.element.http-proxy.super_.super_"></a>[function <span class="apidocSignatureSpan">http-proxy.</span>super_ ()](#apidoc.element.http-proxy.super_.super_)
- description and source-code
```javascript
function EventEmitter() { /* Nothing to set */ }
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.http-proxy.super_.prototype"></a>[module http-proxy.super_.prototype](#apidoc.module.http-proxy.super_.prototype)

#### <a name="apidoc.element.http-proxy.super_.prototype.addListener"></a>[function <span class="apidocSignatureSpan">http-proxy.super_.prototype.</span>addListener (event, fn, context)](#apidoc.element.http-proxy.super_.prototype.addListener)
- description and source-code
```javascript
function on(event, fn, context) {
  var listener = new EE(fn, context || this)
    , evt = prefix ? prefix + event : event;

  if (!this._events) this._events = prefix ? {} : Object.create(null);
  if (!this._events[evt]) this._events[evt] = listener;
  else {
    if (!this._events[evt].fn) this._events[evt].push(listener);
    else this._events[evt] = [
      this._events[evt], listener
    ];
  }

  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.http-proxy.super_.prototype.emit"></a>[function <span class="apidocSignatureSpan">http-proxy.super_.prototype.</span>emit (event, a1, a2, a3, a4, a5)](#apidoc.element.http-proxy.super_.prototype.emit)
- description and source-code
```javascript
function emit(event, a1, a2, a3, a4, a5) {
  var evt = prefix ? prefix + event : event;

  if (!this._events || !this._events[evt]) return false;

  var listeners = this._events[evt]
    , len = arguments.length
    , args
    , i;

  if ('function' === typeof listeners.fn) {
    if (listeners.once) this.removeListener(event, listeners.fn, undefined, true);

    switch (len) {
      case 1: return listeners.fn.call(listeners.context), true;
      case 2: return listeners.fn.call(listeners.context, a1), true;
      case 3: return listeners.fn.call(listeners.context, a1, a2), true;
      case 4: return listeners.fn.call(listeners.context, a1, a2, a3), true;
      case 5: return listeners.fn.call(listeners.context, a1, a2, a3, a4), true;
      case 6: return listeners.fn.call(listeners.context, a1, a2, a3, a4, a5), true;
    }

    for (i = 1, args = new Array(len -1); i < len; i++) {
      args[i - 1] = arguments[i];
    }

    listeners.fn.apply(listeners.context, args);
  } else {
    var length = listeners.length
      , j;

    for (i = 0; i < length; i++) {
      if (listeners[i].once) this.removeListener(event, listeners[i].fn, undefined, true);

      switch (len) {
        case 1: listeners[i].fn.call(listeners[i].context); break;
        case 2: listeners[i].fn.call(listeners[i].context, a1); break;
        case 3: listeners[i].fn.call(listeners[i].context, a1, a2); break;
        default:
          if (!args) for (j = 1, args = new Array(len -1); j < len; j++) {
            args[j - 1] = arguments[j];
          }

          listeners[i].fn.apply(listeners[i].context, args);
      }
    }
  }

  return true;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.http-proxy.super_.prototype.eventNames"></a>[function <span class="apidocSignatureSpan">http-proxy.super_.prototype.</span>eventNames ()](#apidoc.element.http-proxy.super_.prototype.eventNames)
- description and source-code
```javascript
function eventNames() {
  var events = this._events
    , names = []
    , name;

  if (!events) return names;

  for (name in events) {
    if (has.call(events, name)) names.push(prefix ? name.slice(1) : name);
  }

  if (Object.getOwnPropertySymbols) {
    return names.concat(Object.getOwnPropertySymbols(events));
  }

  return names;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.http-proxy.super_.prototype.listeners"></a>[function <span class="apidocSignatureSpan">http-proxy.super_.prototype.</span>listeners (event, exists)](#apidoc.element.http-proxy.super_.prototype.listeners)
- description and source-code
```javascript
function listeners(event, exists) {
  var evt = prefix ? prefix + event : event
    , available = this._events && this._events[evt];

  if (exists) return !!available;
  if (!available) return [];
  if (available.fn) return [available.fn];

  for (var i = 0, l = available.length, ee = new Array(l); i < l; i++) {
    ee[i] = available[i].fn;
  }

  return ee;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.http-proxy.super_.prototype.off"></a>[function <span class="apidocSignatureSpan">http-proxy.super_.prototype.</span>off (event, fn, context, once)](#apidoc.element.http-proxy.super_.prototype.off)
- description and source-code
```javascript
function removeListener(event, fn, context, once) {
  var evt = prefix ? prefix + event : event;

  if (!this._events || !this._events[evt]) return this;

  var listeners = this._events[evt]
    , events = [];

  if (fn) {
    if (listeners.fn) {
      if (
           listeners.fn !== fn
        || (once && !listeners.once)
        || (context && listeners.context !== context)
      ) {
        events.push(listeners);
      }
    } else {
      for (var i = 0, length = listeners.length; i < length; i++) {
        if (
             listeners[i].fn !== fn
          || (once && !listeners[i].once)
          || (context && listeners[i].context !== context)
        ) {
          events.push(listeners[i]);
        }
      }
    }
  }

  //
  // Reset the array, or remove it completely if we have no more listeners.
  //
  if (events.length) {
    this._events[evt] = events.length === 1 ? events[0] : events;
  } else {
    delete this._events[evt];
  }

  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.http-proxy.super_.prototype.on"></a>[function <span class="apidocSignatureSpan">http-proxy.super_.prototype.</span>on (event, fn, context)](#apidoc.element.http-proxy.super_.prototype.on)
- description and source-code
```javascript
function on(event, fn, context) {
  var listener = new EE(fn, context || this)
    , evt = prefix ? prefix + event : event;

  if (!this._events) this._events = prefix ? {} : Object.create(null);
  if (!this._events[evt]) this._events[evt] = listener;
  else {
    if (!this._events[evt].fn) this._events[evt].push(listener);
    else this._events[evt] = [
      this._events[evt], listener
    ];
  }

  return this;
}
```
- example usage
```shell
...
  proxy.web(req, res, { target: 'http://mytarget.com:8080' });
});
'''

Errors can be listened on either using the Event Emitter API

'''javascript
proxy.on('error', function(e) {
  ...
});
'''

or using the callback API

'''javascript
...
```

#### <a name="apidoc.element.http-proxy.super_.prototype.once"></a>[function <span class="apidocSignatureSpan">http-proxy.super_.prototype.</span>once (event, fn, context)](#apidoc.element.http-proxy.super_.prototype.once)
- description and source-code
```javascript
function once(event, fn, context) {
  var listener = new EE(fn, context || this, true)
    , evt = prefix ? prefix + event : event;

  if (!this._events) this._events = prefix ? {} : Object.create(null);
  if (!this._events[evt]) this._events[evt] = listener;
  else {
    if (!this._events[evt].fn) this._events[evt].push(listener);
    else this._events[evt] = [
      this._events[evt], listener
    ];
  }

  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.http-proxy.super_.prototype.removeAllListeners"></a>[function <span class="apidocSignatureSpan">http-proxy.super_.prototype.</span>removeAllListeners (event)](#apidoc.element.http-proxy.super_.prototype.removeAllListeners)
- description and source-code
```javascript
function removeAllListeners(event) {
  if (!this._events) return this;

  if (event) delete this._events[prefix ? prefix + event : event];
  else this._events = prefix ? {} : Object.create(null);

  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.http-proxy.super_.prototype.removeListener"></a>[function <span class="apidocSignatureSpan">http-proxy.super_.prototype.</span>removeListener (event, fn, context, once)](#apidoc.element.http-proxy.super_.prototype.removeListener)
- description and source-code
```javascript
function removeListener(event, fn, context, once) {
  var evt = prefix ? prefix + event : event;

  if (!this._events || !this._events[evt]) return this;

  var listeners = this._events[evt]
    , events = [];

  if (fn) {
    if (listeners.fn) {
      if (
           listeners.fn !== fn
        || (once && !listeners.once)
        || (context && listeners.context !== context)
      ) {
        events.push(listeners);
      }
    } else {
      for (var i = 0, length = listeners.length; i < length; i++) {
        if (
             listeners[i].fn !== fn
          || (once && !listeners[i].once)
          || (context && listeners[i].context !== context)
        ) {
          events.push(listeners[i]);
        }
      }
    }
  }

  //
  // Reset the array, or remove it completely if we have no more listeners.
  //
  if (events.length) {
    this._events[evt] = events.length === 1 ? events[0] : events;
  } else {
    delete this._events[evt];
  }

  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.http-proxy.super_.prototype.setMaxListeners"></a>[function <span class="apidocSignatureSpan">http-proxy.super_.prototype.</span>setMaxListeners ()](#apidoc.element.http-proxy.super_.prototype.setMaxListeners)
- description and source-code
```javascript
function setMaxListeners() {
  return this;
}
```
- example usage
```shell
n/a
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
