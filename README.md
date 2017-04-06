# api documentation for  [flatiron (v0.4.3)](https://github.com/flatiron/flatiron)  [![npm package](https://img.shields.io/npm/v/npmdoc-flatiron.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-flatiron) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-flatiron.svg)](https://travis-ci.org/npmdoc/node-npmdoc-flatiron)
#### An elegant blend of convention and configuration for building apps in Node.js and the browser

[![NPM](https://nodei.co/npm/flatiron.png?downloads=true)](https://www.npmjs.com/package/flatiron)

[![apidoc](https://npmdoc.github.io/node-npmdoc-flatiron/build/screenCapture.buildNpmdoc.browser._2Fhome_2Ftravis_2Fbuild_2Fnpmdoc_2Fnode-npmdoc-flatiron_2Ftmp_2Fbuild_2Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-flatiron/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-flatiron/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-flatiron/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Nodejitsu Inc.",
        "email": "info@nodejitsu.com"
    },
    "bin": {
        "flatiron": "./bin/flatiron"
    },
    "bugs": {
        "url": "https://github.com/flatiron/flatiron/issues"
    },
    "dependencies": {
        "broadway": "~0.3.2",
        "director": "1.2.7",
        "optimist": "0.6.0",
        "prompt": "0.2.14"
    },
    "description": "An elegant blend of convention and configuration for building apps in Node.js and the browser",
    "devDependencies": {
        "request": "2.x.x",
        "resourceful": "0.3.x",
        "st": "0.1.x",
        "union": "0.4.x",
        "vows": "0.7.x"
    },
    "directories": {},
    "dist": {
        "shasum": "248cf79a3da7d7dc379e2a11c92a2719cbb540f6",
        "tarball": "https://registry.npmjs.org/flatiron/-/flatiron-0.4.3.tgz"
    },
    "engines": {
        "node": ">= 0.4.0"
    },
    "gitHead": "0182515b94b1fc7bd76378d42db1033ecfa44b96",
    "homepage": "https://github.com/flatiron/flatiron",
    "main": "./lib/flatiron",
    "maintainers": [
        {
            "name": "indexzero",
            "email": "charlie.robbins@gmail.com"
        },
        {
            "name": "jcrugzz",
            "email": "jcrugzz@gmail.com"
        },
        {
            "name": "swaagie",
            "email": "info@martijnswaagman.nl"
        }
    ],
    "name": "flatiron",
    "optionalDependencies": {},
    "readme": "ERROR: No README data found!",
    "repository": {
        "type": "git",
        "url": "git+ssh://git@github.com/flatiron/flatiron.git"
    },
    "scripts": {
        "test": "vows --spec"
    },
    "version": "0.4.3"
}
```



# <a name="apidoc.tableOfContents"></a>[table of contents](#apidoc.tableOfContents)

#### [module flatiron](#apidoc.module.flatiron)
1.  [function <span class="apidocSignatureSpan">flatiron.</span>App (options)](#apidoc.element.flatiron.App)
1.  [function <span class="apidocSignatureSpan">flatiron.</span>App.super_ (options)](#apidoc.element.flatiron.App.super_)
1.  [function <span class="apidocSignatureSpan">flatiron.</span>createApp (options)](#apidoc.element.flatiron.createApp)
1.  object <span class="apidocSignatureSpan">flatiron.</span>App.super_.prototype
1.  object <span class="apidocSignatureSpan">flatiron.</span>App.super_.super_.prototype
1.  object <span class="apidocSignatureSpan">flatiron.</span>common
1.  object <span class="apidocSignatureSpan">flatiron.</span>common.directories
1.  object <span class="apidocSignatureSpan">flatiron.</span>constants
1.  object <span class="apidocSignatureSpan">flatiron.</span>formats
1.  object <span class="apidocSignatureSpan">flatiron.</span>plugins
1.  string <span class="apidocSignatureSpan">flatiron.</span>version

#### [module flatiron.App](#apidoc.module.flatiron.App)
1.  [function <span class="apidocSignatureSpan">flatiron.</span>App (options)](#apidoc.element.flatiron.App.App)
1.  [function <span class="apidocSignatureSpan">flatiron.App.</span>super_ (options)](#apidoc.element.flatiron.App.super_)

#### [module flatiron.App.super_](#apidoc.module.flatiron.App.super_)
1.  [function <span class="apidocSignatureSpan">flatiron.App.</span>super_ (conf)](#apidoc.element.flatiron.App.super_.super_)

#### [module flatiron.App.super_.prototype](#apidoc.module.flatiron.App.super_.prototype)
1.  [function <span class="apidocSignatureSpan">flatiron.App.super_.prototype.</span>init (options, callback)](#apidoc.element.flatiron.App.super_.prototype.init)
1.  [function <span class="apidocSignatureSpan">flatiron.App.super_.prototype.</span>inspect ()](#apidoc.element.flatiron.App.super_.prototype.inspect)
1.  [function <span class="apidocSignatureSpan">flatiron.App.super_.prototype.</span>remove (name)](#apidoc.element.flatiron.App.super_.prototype.remove)
1.  [function <span class="apidocSignatureSpan">flatiron.App.super_.prototype.</span>use (plugin, options, callback)](#apidoc.element.flatiron.App.super_.prototype.use)

#### [module flatiron.App.super_.super_.prototype](#apidoc.module.flatiron.App.super_.super_.prototype)
1.  [function <span class="apidocSignatureSpan">flatiron.App.super_.super_.prototype.</span>addListener (type, listener)](#apidoc.element.flatiron.App.super_.super_.prototype.addListener)
1.  [function <span class="apidocSignatureSpan">flatiron.App.super_.super_.prototype.</span>emit ()](#apidoc.element.flatiron.App.super_.super_.prototype.emit)
1.  [function <span class="apidocSignatureSpan">flatiron.App.super_.super_.prototype.</span>listeners (type)](#apidoc.element.flatiron.App.super_.super_.prototype.listeners)
1.  [function <span class="apidocSignatureSpan">flatiron.App.super_.super_.prototype.</span>listenersAny ()](#apidoc.element.flatiron.App.super_.super_.prototype.listenersAny)
1.  [function <span class="apidocSignatureSpan">flatiron.App.super_.super_.prototype.</span>many (event, ttl, fn)](#apidoc.element.flatiron.App.super_.super_.prototype.many)
1.  [function <span class="apidocSignatureSpan">flatiron.App.super_.super_.prototype.</span>off (type, listener)](#apidoc.element.flatiron.App.super_.super_.prototype.off)
1.  [function <span class="apidocSignatureSpan">flatiron.App.super_.super_.prototype.</span>offAny (fn)](#apidoc.element.flatiron.App.super_.super_.prototype.offAny)
1.  [function <span class="apidocSignatureSpan">flatiron.App.super_.super_.prototype.</span>on (type, listener)](#apidoc.element.flatiron.App.super_.super_.prototype.on)
1.  [function <span class="apidocSignatureSpan">flatiron.App.super_.super_.prototype.</span>onAny (fn)](#apidoc.element.flatiron.App.super_.super_.prototype.onAny)
1.  [function <span class="apidocSignatureSpan">flatiron.App.super_.super_.prototype.</span>once (event, fn)](#apidoc.element.flatiron.App.super_.super_.prototype.once)
1.  [function <span class="apidocSignatureSpan">flatiron.App.super_.super_.prototype.</span>removeAllListeners (type)](#apidoc.element.flatiron.App.super_.super_.prototype.removeAllListeners)
1.  [function <span class="apidocSignatureSpan">flatiron.App.super_.super_.prototype.</span>removeListener (type, listener)](#apidoc.element.flatiron.App.super_.super_.prototype.removeListener)
1.  [function <span class="apidocSignatureSpan">flatiron.App.super_.super_.prototype.</span>setMaxListeners (n)](#apidoc.element.flatiron.App.super_.super_.prototype.setMaxListeners)
1.  string <span class="apidocSignatureSpan">flatiron.App.super_.super_.prototype.</span>delimiter
1.  string <span class="apidocSignatureSpan">flatiron.App.super_.super_.prototype.</span>event

#### [module flatiron.common](#apidoc.module.flatiron.common)
1.  [function <span class="apidocSignatureSpan">flatiron.common.</span>_errnoException (err, syscall, original)](#apidoc.element.flatiron.common._errnoException)
1.  [function <span class="apidocSignatureSpan">flatiron.common.</span>_exceptionWithHostPort (err, syscall, address, port, additional)](#apidoc.element.flatiron.common._exceptionWithHostPort)
1.  [function <span class="apidocSignatureSpan">flatiron.common.</span>_extend (target, source)](#apidoc.element.flatiron.common._extend)
1.  [function <span class="apidocSignatureSpan">flatiron.common.</span>camelToUnderscore (obj)](#apidoc.element.flatiron.common.camelToUnderscore)
1.  [function <span class="apidocSignatureSpan">flatiron.common.</span>capitalize (lower_case_and_underscored_word, first_letter_in_uppercase)](#apidoc.element.flatiron.common.capitalize)
1.  [function <span class="apidocSignatureSpan">flatiron.common.</span>clone (object, filter)](#apidoc.element.flatiron.common.clone)
1.  [function <span class="apidocSignatureSpan">flatiron.common.</span>createPath (obj, path, value)](#apidoc.element.flatiron.common.createPath)
1.  [function <span class="apidocSignatureSpan">flatiron.common.</span>debug ()](#apidoc.element.flatiron.common.debug)
1.  [function <span class="apidocSignatureSpan">flatiron.common.</span>debuglog (set)](#apidoc.element.flatiron.common.debuglog)
1.  [function <span class="apidocSignatureSpan">flatiron.common.</span>deprecate (fn, msg)](#apidoc.element.flatiron.common.deprecate)
1.  [function <span class="apidocSignatureSpan">flatiron.common.</span>each (obj, iterator)](#apidoc.element.flatiron.common.each)
1.  [function <span class="apidocSignatureSpan">flatiron.common.</span>error ()](#apidoc.element.flatiron.common.error)
1.  [function <span class="apidocSignatureSpan">flatiron.common.</span>escapeRegExp (str)](#apidoc.element.flatiron.common.escapeRegExp)
1.  [function <span class="apidocSignatureSpan">flatiron.common.</span>filter (obj, pred)](#apidoc.element.flatiron.common.filter)
1.  [function <span class="apidocSignatureSpan">flatiron.common.</span>find (obj, pred)](#apidoc.element.flatiron.common.find)
1.  [function <span class="apidocSignatureSpan">flatiron.common.</span>inherits (ctor, superCtor)](#apidoc.element.flatiron.common.inherits)
1.  [function <span class="apidocSignatureSpan">flatiron.common.</span>inspect (obj, opts)](#apidoc.element.flatiron.common.inspect)
1.  [function <span class="apidocSignatureSpan">flatiron.common.</span>isArray ()](#apidoc.element.flatiron.common.isArray)
1.  [function <span class="apidocSignatureSpan">flatiron.common.</span>isBoolean (arg)](#apidoc.element.flatiron.common.isBoolean)
1.  [function <span class="apidocSignatureSpan">flatiron.common.</span>isBuffer (b)](#apidoc.element.flatiron.common.isBuffer)
1.  [function <span class="apidocSignatureSpan">flatiron.common.</span>isDate (d)](#apidoc.element.flatiron.common.isDate)
1.  [function <span class="apidocSignatureSpan">flatiron.common.</span>isError (e)](#apidoc.element.flatiron.common.isError)
1.  [function <span class="apidocSignatureSpan">flatiron.common.</span>isFunction (arg)](#apidoc.element.flatiron.common.isFunction)
1.  [function <span class="apidocSignatureSpan">flatiron.common.</span>isNull (arg)](#apidoc.element.flatiron.common.isNull)
1.  [function <span class="apidocSignatureSpan">flatiron.common.</span>isNullOrUndefined (arg)](#apidoc.element.flatiron.common.isNullOrUndefined)
1.  [function <span class="apidocSignatureSpan">flatiron.common.</span>isNumber (arg)](#apidoc.element.flatiron.common.isNumber)
1.  [function <span class="apidocSignatureSpan">flatiron.common.</span>isObject (arg)](#apidoc.element.flatiron.common.isObject)
1.  [function <span class="apidocSignatureSpan">flatiron.common.</span>isPrimitive (arg)](#apidoc.element.flatiron.common.isPrimitive)
1.  [function <span class="apidocSignatureSpan">flatiron.common.</span>isRegExp (re)](#apidoc.element.flatiron.common.isRegExp)
1.  [function <span class="apidocSignatureSpan">flatiron.common.</span>isString (arg)](#apidoc.element.flatiron.common.isString)
1.  [function <span class="apidocSignatureSpan">flatiron.common.</span>isSymbol (arg)](#apidoc.element.flatiron.common.isSymbol)
1.  [function <span class="apidocSignatureSpan">flatiron.common.</span>isUndefined (arg)](#apidoc.element.flatiron.common.isUndefined)
1.  [function <span class="apidocSignatureSpan">flatiron.common.</span>log ()](#apidoc.element.flatiron.common.log)
1.  [function <span class="apidocSignatureSpan">flatiron.common.</span>mixin (target)](#apidoc.element.flatiron.common.mixin)
1.  [function <span class="apidocSignatureSpan">flatiron.common.</span>pad (str, len, chr)](#apidoc.element.flatiron.common.pad)
1.  [function <span class="apidocSignatureSpan">flatiron.common.</span>path (obj, path)](#apidoc.element.flatiron.common.path)
1.  [function <span class="apidocSignatureSpan">flatiron.common.</span>print ()](#apidoc.element.flatiron.common.print)
1.  [function <span class="apidocSignatureSpan">flatiron.common.</span>puts ()](#apidoc.element.flatiron.common.puts)
1.  [function <span class="apidocSignatureSpan">flatiron.common.</span>randomString (length)](#apidoc.element.flatiron.common.randomString)
1.  [function <span class="apidocSignatureSpan">flatiron.common.</span>rargs (_args, slice)](#apidoc.element.flatiron.common.rargs)
1.  [function <span class="apidocSignatureSpan">flatiron.common.</span>requireDir (directory)](#apidoc.element.flatiron.common.requireDir)
1.  [function <span class="apidocSignatureSpan">flatiron.common.</span>requireDirLazy (directory)](#apidoc.element.flatiron.common.requireDirLazy)
1.  [function <span class="apidocSignatureSpan">flatiron.common.</span>templateUsage (app, commands)](#apidoc.element.flatiron.common.templateUsage)
1.  [function <span class="apidocSignatureSpan">flatiron.common.</span>tryReaddirSync (dir)](#apidoc.element.flatiron.common.tryReaddirSync)
1.  [function <span class="apidocSignatureSpan">flatiron.common.</span>underscoreToCamel (obj)](#apidoc.element.flatiron.common.underscoreToCamel)
1.  [function <span class="apidocSignatureSpan">flatiron.common.</span>uuid ()](#apidoc.element.flatiron.common.uuid)
1.  object <span class="apidocSignatureSpan">flatiron.common.</span>directories

#### [module flatiron.common.directories](#apidoc.module.flatiron.common.directories)
1.  [function <span class="apidocSignatureSpan">flatiron.common.directories.</span>create (dirs, callback)](#apidoc.element.flatiron.common.directories.create)
1.  [function <span class="apidocSignatureSpan">flatiron.common.directories.</span>normalize (keys, dirs)](#apidoc.element.flatiron.common.directories.normalize)
1.  [function <span class="apidocSignatureSpan">flatiron.common.directories.</span>remove (dirs, callback)](#apidoc.element.flatiron.common.directories.remove)



# <a name="apidoc.module.flatiron"></a>[module flatiron](#apidoc.module.flatiron)

#### <a name="apidoc.element.flatiron.App"></a>[function <span class="apidocSignatureSpan">flatiron.</span>App (options)](#apidoc.element.flatiron.App)
- description and source-code
```javascript
App = function (options) {
  broadway.App.call(this, options);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.flatiron.App.super_"></a>[function <span class="apidocSignatureSpan">flatiron.</span>App.super_ (options)](#apidoc.element.flatiron.App.super_)
- description and source-code
```javascript
App.super_ = function (options) {
  //
  // Setup options and 'App' constants.
  //
  options        = options || {};
  this.root      = options.root;
  this.delimiter = options.delimiter || '::';

  //
  // Inherit from 'EventEmitter2'
  //
  events.EventEmitter2.call(this, {
    delimiter: this.delimiter,
    wildcard: true
  });

  //
  // Setup other relevant options such as the plugins
  // for this instance.
  //
  this.options      = options;
  this.env          = options.env || process.env['NODE_ENV'] || 'development'
  this.plugins      = options.plugins || {};
  this.initialized  = false;
  this.bootstrapper = options.bootstrapper || bootstrapper;
  this.initializers = {};
  this.initlist     = [];

  //
  // Bootstrap this instance
  //
  this.bootstrapper.bootstrap(this);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.flatiron.createApp"></a>[function <span class="apidocSignatureSpan">flatiron.</span>createApp (options)](#apidoc.element.flatiron.createApp)
- description and source-code
```javascript
createApp = function (options) {
  return new flatiron.App(options);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.flatiron.App"></a>[module flatiron.App](#apidoc.module.flatiron.App)

#### <a name="apidoc.element.flatiron.App.App"></a>[function <span class="apidocSignatureSpan">flatiron.</span>App (options)](#apidoc.element.flatiron.App.App)
- description and source-code
```javascript
App = function (options) {
  broadway.App.call(this, options);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.flatiron.App.super_"></a>[function <span class="apidocSignatureSpan">flatiron.App.</span>super_ (options)](#apidoc.element.flatiron.App.super_)
- description and source-code
```javascript
super_ = function (options) {
  //
  // Setup options and 'App' constants.
  //
  options        = options || {};
  this.root      = options.root;
  this.delimiter = options.delimiter || '::';

  //
  // Inherit from 'EventEmitter2'
  //
  events.EventEmitter2.call(this, {
    delimiter: this.delimiter,
    wildcard: true
  });

  //
  // Setup other relevant options such as the plugins
  // for this instance.
  //
  this.options      = options;
  this.env          = options.env || process.env['NODE_ENV'] || 'development'
  this.plugins      = options.plugins || {};
  this.initialized  = false;
  this.bootstrapper = options.bootstrapper || bootstrapper;
  this.initializers = {};
  this.initlist     = [];

  //
  // Bootstrap this instance
  //
  this.bootstrapper.bootstrap(this);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.flatiron.App.super_"></a>[module flatiron.App.super_](#apidoc.module.flatiron.App.super_)

#### <a name="apidoc.element.flatiron.App.super_.super_"></a>[function <span class="apidocSignatureSpan">flatiron.App.</span>super_ (conf)](#apidoc.element.flatiron.App.super_.super_)
- description and source-code
```javascript
function EventEmitter(conf) {
  this._events = {};
  this.newListener = false;
  configure.call(this, conf);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.flatiron.App.super_.prototype"></a>[module flatiron.App.super_.prototype](#apidoc.module.flatiron.App.super_.prototype)

#### <a name="apidoc.element.flatiron.App.super_.prototype.init"></a>[function <span class="apidocSignatureSpan">flatiron.App.super_.prototype.</span>init (options, callback)](#apidoc.element.flatiron.App.super_.prototype.init)
- description and source-code
```javascript
init = function (options, callback) {
  if (!callback && typeof options === 'function') {
    callback = options;
    options = {};
  }

  if (this.initialized) {
    return callback();
  }

  var self = this;
  options = options   || {};
  callback = callback || function () {};
  this.env = options.env || this.env;
  this.options = common.mixin({}, this.options, options);

  function onComplete() {
    self.initialized = true;
    self.emit('init');
    callback();
  }

  function ensureFeatures (err) {
    return err
      ? onError(err)
      : features.ensure(this, onComplete);
  }

  function initPlugin(plugin, next) {
    if (typeof self.initializers[plugin] === 'function') {
      return self.initializers[plugin].call(self, function (err) {
        if (err) {
          return next(err);
        }

        self.emit(['plugin', plugin, 'init']);
        self.initializers[plugin] = true;
        next();
      });
    }

    next();
  }

  function initPlugins() {
    async.forEach(self.initlist, initPlugin, ensureFeatures);
  }

  //
  // Emit and respond with any errors that may short
  // circuit the process.
  //
  function onError(err) {
    self.emit(['error', 'init'], err);
    callback(err);
  }

  //
  // Run the bootstrapper, initialize plugins, and
  // ensure features for this instance.
  //
  this.bootstrapper.init(this, initPlugins);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.flatiron.App.super_.prototype.inspect"></a>[function <span class="apidocSignatureSpan">flatiron.App.super_.prototype.</span>inspect ()](#apidoc.element.flatiron.App.super_.prototype.inspect)
- description and source-code
```javascript
inspect = function () {

}
```
- example usage
```shell
...
this.res.end('Hello world!\n');
});

// POST to /
app.router.post('/', function () {
this.res.writeHead(200, { 'Content-Type': 'text/plain' });
this.res.write('Hey, you posted some cool data!\n');
this.res.end(util.inspect(this.req.body, true, 2, true) + '\n');
});

// Parameterized routes
app.router.get('/sandwich/:type', function (type) {
if (~['bacon', 'burger'].indexOf(type)) {
  this.res.writeHead(200, { 'Content-Type': 'text/plain' });
  this.res.end('Serving ' + type + ' sandwich!\n');
...
```

#### <a name="apidoc.element.flatiron.App.super_.prototype.remove"></a>[function <span class="apidocSignatureSpan">flatiron.App.super_.prototype.</span>remove (name)](#apidoc.element.flatiron.App.super_.prototype.remove)
- description and source-code
```javascript
remove = function (name) {
  // if this is a plugin object set the name to the plugins name
  if (name.name) {
    name = name.name;
  }

  if (this.plugins[name] && this.plugins[name].detach) {
    this.plugins[name].detach.call(this);
  }

  delete this.plugins[name];
  delete this.options[name];
  delete this.initializers[name];

  var init = this.initlist.indexOf(name);

  if (init !== -1) {
    this.initlist.splice(1, init);
  }
}
```
- example usage
```shell
...
// add the 'file' store the the config
app.config.use('file', { file: 'path/to/config.json' });

// or using an alternate syntax
app.config.env().file({ file: 'path/to/config.json' });

// and removing stores
app.config.remove('literal');
'''

### 'app.log'

'flatiron.app' will also load a ['log'](https://github.com/flatiron/broadway/blob/master/lib/broadway/plugins/log.js) plugin during
 the init phase, which attaches a [winston container](https://github.com/flatiron/winston) to 'app.log'. This logger is configured
 by combining the 'app.options.log' property with the configuration retrieved from 'app.config.get('log')'.

## Create An HTTP Server with 'flatiron.plugins.http(options)':
...
```

#### <a name="apidoc.element.flatiron.App.super_.prototype.use"></a>[function <span class="apidocSignatureSpan">flatiron.App.super_.prototype.</span>use (plugin, options, callback)](#apidoc.element.flatiron.App.super_.prototype.use)
- description and source-code
```javascript
use = function (plugin, options, callback) {
  options = options || {};

  if (typeof plugin === 'undefined') {
    console.log('Cannot load invalid plugin!');
    return callback && callback(new Error('Invalid plugin'));
  }

  var name = plugin.name,
      self = this;

  // If the plugin doesn't have a name, use itself as an identifier for the plugins hash.
  if (!name) {
    name = common.uuid();
  }

  if (this.plugins[name]) {
    return callback && callback();
  }

  //
  // Setup state on this instance for the specified plugin
  //
  this.plugins[name] = plugin;
  this.options[name] = common.mixin({}, options, this.options[name] || {});

  //
  // Attach the specified plugin to this instance, extending
  // the 'App' with new functionality.
  //
  if (this.plugins[name].attach && options.attach !== false) {
    this.plugins[name].attach.call(this, options);
  }

  //
  // Setup the initializer only if 'options.init' is
  // not false. This allows for some plugins to be lazy-loaded
  //
  if (options.init === false) {
    return callback && callback();
  }

  if (!this.initialized) {
    this.initializers[name] = plugin.init || true;
    this.initlist.push(name);
    return callback && callback();
  }
  else if (plugin.init) {
    plugin.init.call(this, function (err) {
      var args = err
        ? [['plugin', name, 'error'], err]
        : [['plugin', name, 'init']];

      self.emit.apply(self, args);
      return callback && (err ? callback(err) : callback());
    });
  }
}
```
- example usage
```shell
...

# Example HTTP Server:

'''js
var flatiron = require('flatiron'),
    app = flatiron.app;

app.use(flatiron.plugins.http);

app.router.get('/', function () {
  this.res.writeHead(200, { 'Content-Type': 'text/plain' });
  this.res.end('Hello world!\n');
});

app.start(8080);
...
```



# <a name="apidoc.module.flatiron.App.super_.super_.prototype"></a>[module flatiron.App.super_.super_.prototype](#apidoc.module.flatiron.App.super_.super_.prototype)

#### <a name="apidoc.element.flatiron.App.super_.super_.prototype.addListener"></a>[function <span class="apidocSignatureSpan">flatiron.App.super_.super_.prototype.</span>addListener (type, listener)](#apidoc.element.flatiron.App.super_.super_.prototype.addListener)
- description and source-code
```javascript
addListener = function (type, listener) {

  if (typeof type === 'function') {
    this.onAny(type);
    return this;
  }

  if (typeof listener !== 'function') {
    throw new Error('on only accepts instances of Function');
  }
  this._events || init.call(this);

  // To avoid recursion in the case that type == "newListeners"! Before
  // adding it to the listeners, first emit "newListeners".
  this.emit('newListener', type, listener);

  if(this.wildcard) {
    growListenerTree.call(this, type, listener);
    return this;
  }

  if (!this._events[type]) {
    // Optimize the case of one listener. Don't need the extra array object.
    this._events[type] = listener;
  }
  else if(typeof this._events[type] === 'function') {
    // Adding the second element, need to change to array.
    this._events[type] = [this._events[type], listener];
  }
  else if (isArray(this._events[type])) {
    // If we've already got an array, just append.
    this._events[type].push(listener);

    // Check for listener leak
    if (!this._events[type].warned) {

      var m = defaultMaxListeners;

      if (typeof this._events.maxListeners !== 'undefined') {
        m = this._events.maxListeners;
      }

      if (m > 0 && this._events[type].length > m) {

        this._events[type].warned = true;
        console.error('(node) warning: possible EventEmitter memory ' +
                      'leak detected. %d listeners added. ' +
                      'Use emitter.setMaxListeners() to increase limit.',
                      this._events[type].length);
        console.trace();
      }
    }
  }
  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.flatiron.App.super_.super_.prototype.emit"></a>[function <span class="apidocSignatureSpan">flatiron.App.super_.super_.prototype.</span>emit ()](#apidoc.element.flatiron.App.super_.super_.prototype.emit)
- description and source-code
```javascript
emit = function () {

  this._events || init.call(this);

  var type = arguments[0];

  if (type === 'newListener' && !this.newListener) {
    if (!this._events.newListener) { return false; }
  }

  // Loop through the *_all* functions and invoke them.
  if (this._all) {
    var l = arguments.length;
    var args = new Array(l - 1);
    for (var i = 1; i < l; i++) args[i - 1] = arguments[i];
    for (i = 0, l = this._all.length; i < l; i++) {
      this.event = type;
      this._all[i].apply(this, args);
    }
  }

  // If there is no 'error' event listener then throw.
  if (type === 'error') {

    if (!this._all &&
      !this._events.error &&
      !(this.wildcard && this.listenerTree.error)) {

      if (arguments[1] instanceof Error) {
        throw arguments[1]; // Unhandled 'error' event
      } else {
        throw new Error("Uncaught, unspecified 'error' event.");
      }
      return false;
    }
  }

  var handler;

  if(this.wildcard) {
    handler = [];
    var ns = typeof type === 'string' ? type.split(this.delimiter) : type.slice();
    searchListenerTree.call(this, handler, ns, this.listenerTree, 0);
  }
  else {
    handler = this._events[type];
  }

  if (typeof handler === 'function') {
    this.event = type;
    if (arguments.length === 1) {
      handler.call(this);
    }
    else if (arguments.length > 1)
      switch (arguments.length) {
        case 2:
          handler.call(this, arguments[1]);
          break;
        case 3:
          handler.call(this, arguments[1], arguments[2]);
          break;
        // slower
        default:
          var l = arguments.length;
          var args = new Array(l - 1);
          for (var i = 1; i < l; i++) args[i - 1] = arguments[i];
          handler.apply(this, args);
      }
    return true;
  }
  else if (handler) {
    var l = arguments.length;
    var args = new Array(l - 1);
    for (var i = 1; i < l; i++) args[i - 1] = arguments[i];

    var listeners = handler.slice();
    for (var i = 0, l = listeners.length; i < l; i++) {
      this.event = type;
      listeners[i].apply(this, args);
    }
    return (listeners.length > 0) || !!this._all;
  }
  else {
    return !!this._all;
  }

}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.flatiron.App.super_.super_.prototype.listeners"></a>[function <span class="apidocSignatureSpan">flatiron.App.super_.super_.prototype.</span>listeners (type)](#apidoc.element.flatiron.App.super_.super_.prototype.listeners)
- description and source-code
```javascript
listeners = function (type) {
  if(this.wildcard) {
    var handlers = [];
    var ns = typeof type === 'string' ? type.split(this.delimiter) : type.slice();
    searchListenerTree.call(this, handlers, ns, this.listenerTree, 0);
    return handlers;
  }

  this._events || init.call(this);

  if (!this._events[type]) this._events[type] = [];
  if (!isArray(this._events[type])) {
    this._events[type] = [this._events[type]];
  }
  return this._events[type];
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.flatiron.App.super_.super_.prototype.listenersAny"></a>[function <span class="apidocSignatureSpan">flatiron.App.super_.super_.prototype.</span>listenersAny ()](#apidoc.element.flatiron.App.super_.super_.prototype.listenersAny)
- description and source-code
```javascript
listenersAny = function () {

  if(this._all) {
    return this._all;
  }
  else {
    return [];
  }

}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.flatiron.App.super_.super_.prototype.many"></a>[function <span class="apidocSignatureSpan">flatiron.App.super_.super_.prototype.</span>many (event, ttl, fn)](#apidoc.element.flatiron.App.super_.super_.prototype.many)
- description and source-code
```javascript
many = function (event, ttl, fn) {
  var self = this;

  if (typeof fn !== 'function') {
    throw new Error('many only accepts instances of Function');
  }

  function listener() {
    if (--ttl === 0) {
      self.off(event, listener);
    }
    fn.apply(this, arguments);
  }

  listener._origin = fn;

  this.on(event, listener);

  return self;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.flatiron.App.super_.super_.prototype.off"></a>[function <span class="apidocSignatureSpan">flatiron.App.super_.super_.prototype.</span>off (type, listener)](#apidoc.element.flatiron.App.super_.super_.prototype.off)
- description and source-code
```javascript
off = function (type, listener) {
  if (typeof listener !== 'function') {
    throw new Error('removeListener only takes instances of Function');
  }

  var handlers,leafs=[];

  if(this.wildcard) {
    var ns = typeof type === 'string' ? type.split(this.delimiter) : type.slice();
    leafs = searchListenerTree.call(this, null, ns, this.listenerTree, 0);
  }
  else {
    // does not use listeners(), so no side effect of creating _events[type]
    if (!this._events[type]) return this;
    handlers = this._events[type];
    leafs.push({_listeners:handlers});
  }

  for (var iLeaf=0; iLeaf<leafs.length; iLeaf++) {
    var leaf = leafs[iLeaf];
    handlers = leaf._listeners;
    if (isArray(handlers)) {

      var position = -1;

      for (var i = 0, length = handlers.length; i < length; i++) {
        if (handlers[i] === listener ||
          (handlers[i].listener && handlers[i].listener === listener) ||
          (handlers[i]._origin && handlers[i]._origin === listener)) {
          position = i;
          break;
        }
      }

      if (position < 0) {
        continue;
      }

      if(this.wildcard) {
        leaf._listeners.splice(position, 1);
      }
      else {
        this._events[type].splice(position, 1);
      }

      if (handlers.length === 0) {
        if(this.wildcard) {
          delete leaf._listeners;
        }
        else {
          delete this._events[type];
        }
      }
      return this;
    }
    else if (handlers === listener ||
      (handlers.listener && handlers.listener === listener) ||
      (handlers._origin && handlers._origin === listener)) {
      if(this.wildcard) {
        delete leaf._listeners;
      }
      else {
        delete this._events[type];
      }
    }
  }

  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.flatiron.App.super_.super_.prototype.offAny"></a>[function <span class="apidocSignatureSpan">flatiron.App.super_.super_.prototype.</span>offAny (fn)](#apidoc.element.flatiron.App.super_.super_.prototype.offAny)
- description and source-code
```javascript
offAny = function (fn) {
  var i = 0, l = 0, fns;
  if (fn && this._all && this._all.length > 0) {
    fns = this._all;
    for(i = 0, l = fns.length; i < l; i++) {
      if(fn === fns[i]) {
        fns.splice(i, 1);
        return this;
      }
    }
  } else {
    this._all = [];
  }
  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.flatiron.App.super_.super_.prototype.on"></a>[function <span class="apidocSignatureSpan">flatiron.App.super_.super_.prototype.</span>on (type, listener)](#apidoc.element.flatiron.App.super_.super_.prototype.on)
- description and source-code
```javascript
on = function (type, listener) {

  if (typeof type === 'function') {
    this.onAny(type);
    return this;
  }

  if (typeof listener !== 'function') {
    throw new Error('on only accepts instances of Function');
  }
  this._events || init.call(this);

  // To avoid recursion in the case that type == "newListeners"! Before
  // adding it to the listeners, first emit "newListeners".
  this.emit('newListener', type, listener);

  if(this.wildcard) {
    growListenerTree.call(this, type, listener);
    return this;
  }

  if (!this._events[type]) {
    // Optimize the case of one listener. Don't need the extra array object.
    this._events[type] = listener;
  }
  else if(typeof this._events[type] === 'function') {
    // Adding the second element, need to change to array.
    this._events[type] = [this._events[type], listener];
  }
  else if (isArray(this._events[type])) {
    // If we've already got an array, just append.
    this._events[type].push(listener);

    // Check for listener leak
    if (!this._events[type].warned) {

      var m = defaultMaxListeners;

      if (typeof this._events.maxListeners !== 'undefined') {
        m = this._events.maxListeners;
      }

      if (m > 0 && this._events[type].length > m) {

        this._events[type].warned = true;
        console.error('(node) warning: possible EventEmitter memory ' +
                      'leak detected. %d listeners added. ' +
                      'Use emitter.setMaxListeners() to increase limit.',
                      this._events[type].length);
        console.trace();
      }
    }
  }
  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.flatiron.App.super_.super_.prototype.onAny"></a>[function <span class="apidocSignatureSpan">flatiron.App.super_.super_.prototype.</span>onAny (fn)](#apidoc.element.flatiron.App.super_.super_.prototype.onAny)
- description and source-code
```javascript
onAny = function (fn) {

  if (typeof fn !== 'function') {
    throw new Error('onAny only accepts instances of Function');
  }

  if(!this._all) {
    this._all = [];
  }

  // Add the function to the event listener collection.
  this._all.push(fn);
  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.flatiron.App.super_.super_.prototype.once"></a>[function <span class="apidocSignatureSpan">flatiron.App.super_.super_.prototype.</span>once (event, fn)](#apidoc.element.flatiron.App.super_.super_.prototype.once)
- description and source-code
```javascript
once = function (event, fn) {
  this.many(event, 1, fn);
  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.flatiron.App.super_.super_.prototype.removeAllListeners"></a>[function <span class="apidocSignatureSpan">flatiron.App.super_.super_.prototype.</span>removeAllListeners (type)](#apidoc.element.flatiron.App.super_.super_.prototype.removeAllListeners)
- description and source-code
```javascript
removeAllListeners = function (type) {
  if (arguments.length === 0) {
    !this._events || init.call(this);
    return this;
  }

  if(this.wildcard) {
    var ns = typeof type === 'string' ? type.split(this.delimiter) : type.slice();
    var leafs = searchListenerTree.call(this, null, ns, this.listenerTree, 0);

    for (var iLeaf=0; iLeaf<leafs.length; iLeaf++) {
      var leaf = leafs[iLeaf];
      leaf._listeners = null;
    }
  }
  else {
    if (!this._events[type]) return this;
    this._events[type] = null;
  }
  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.flatiron.App.super_.super_.prototype.removeListener"></a>[function <span class="apidocSignatureSpan">flatiron.App.super_.super_.prototype.</span>removeListener (type, listener)](#apidoc.element.flatiron.App.super_.super_.prototype.removeListener)
- description and source-code
```javascript
removeListener = function (type, listener) {
  if (typeof listener !== 'function') {
    throw new Error('removeListener only takes instances of Function');
  }

  var handlers,leafs=[];

  if(this.wildcard) {
    var ns = typeof type === 'string' ? type.split(this.delimiter) : type.slice();
    leafs = searchListenerTree.call(this, null, ns, this.listenerTree, 0);
  }
  else {
    // does not use listeners(), so no side effect of creating _events[type]
    if (!this._events[type]) return this;
    handlers = this._events[type];
    leafs.push({_listeners:handlers});
  }

  for (var iLeaf=0; iLeaf<leafs.length; iLeaf++) {
    var leaf = leafs[iLeaf];
    handlers = leaf._listeners;
    if (isArray(handlers)) {

      var position = -1;

      for (var i = 0, length = handlers.length; i < length; i++) {
        if (handlers[i] === listener ||
          (handlers[i].listener && handlers[i].listener === listener) ||
          (handlers[i]._origin && handlers[i]._origin === listener)) {
          position = i;
          break;
        }
      }

      if (position < 0) {
        continue;
      }

      if(this.wildcard) {
        leaf._listeners.splice(position, 1);
      }
      else {
        this._events[type].splice(position, 1);
      }

      if (handlers.length === 0) {
        if(this.wildcard) {
          delete leaf._listeners;
        }
        else {
          delete this._events[type];
        }
      }
      return this;
    }
    else if (handlers === listener ||
      (handlers.listener && handlers.listener === listener) ||
      (handlers._origin && handlers._origin === listener)) {
      if(this.wildcard) {
        delete leaf._listeners;
      }
      else {
        delete this._events[type];
      }
    }
  }

  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.flatiron.App.super_.super_.prototype.setMaxListeners"></a>[function <span class="apidocSignatureSpan">flatiron.App.super_.super_.prototype.</span>setMaxListeners (n)](#apidoc.element.flatiron.App.super_.super_.prototype.setMaxListeners)
- description and source-code
```javascript
setMaxListeners = function (n) {
  this._events || init.call(this);
  this._events.maxListeners = n;
  if (!this._conf) this._conf = {};
  this._conf.maxListeners = n;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.flatiron.common"></a>[module flatiron.common](#apidoc.module.flatiron.common)

#### <a name="apidoc.element.flatiron.common._errnoException"></a>[function <span class="apidocSignatureSpan">flatiron.common.</span>_errnoException (err, syscall, original)](#apidoc.element.flatiron.common._errnoException)
- description and source-code
```javascript
_errnoException = function (err, syscall, original) {
  var errname = uv.errname(err);
  var message = '${syscall} ${errname}';
  if (original)
    message += ' ' + original;
  var e = new Error(message);
  e.code = errname;
  e.errno = errname;
  e.syscall = syscall;
  return e;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.flatiron.common._exceptionWithHostPort"></a>[function <span class="apidocSignatureSpan">flatiron.common.</span>_exceptionWithHostPort (err, syscall, address, port, additional)](#apidoc.element.flatiron.common._exceptionWithHostPort)
- description and source-code
```javascript
_exceptionWithHostPort = function (err, syscall, address, port, additional) {
  var details;
  if (port && port > 0) {
    details = '${address}:${port}';
  } else {
    details = address;
  }

  if (additional) {
    details += ' - Local (${additional})';
  }
  var ex = exports._errnoException(err, syscall, details);
  ex.address = address;
  if (port) {
    ex.port = port;
  }
  return ex;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.flatiron.common._extend"></a>[function <span class="apidocSignatureSpan">flatiron.common.</span>_extend (target, source)](#apidoc.element.flatiron.common._extend)
- description and source-code
```javascript
_extend = function (target, source) {
  // Don't do anything if source isn't an object
  if (source === null || typeof source !== 'object') return target;

  var keys = Object.keys(source);
  var i = keys.length;
  while (i--) {
    target[keys[i]] = source[keys[i]];
  }
  return target;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.flatiron.common.camelToUnderscore"></a>[function <span class="apidocSignatureSpan">flatiron.common.</span>camelToUnderscore (obj)](#apidoc.element.flatiron.common.camelToUnderscore)
- description and source-code
```javascript
camelToUnderscore = function (obj) {
  if (typeof obj !== 'object' || obj === null) {
    return obj;
  }

  if (Array.isArray(obj)) {
    obj.forEach(utile.camelToUnderscore);
    return obj;
  }

  Object.keys(obj).forEach(function (key) {
    var k = utile.inflect.underscore(key);
    if (k !== key) {
      obj[k] = obj[key];
      delete obj[key];
      key = k;
    }
    utile.camelToUnderscore(obj[key]);
  });

  return obj;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.flatiron.common.capitalize"></a>[function <span class="apidocSignatureSpan">flatiron.common.</span>capitalize (lower_case_and_underscored_word, first_letter_in_uppercase)](#apidoc.element.flatiron.common.capitalize)
- description and source-code
```javascript
capitalize = function (lower_case_and_underscored_word, first_letter_in_uppercase) {
  var result;
  if (first_letter_in_uppercase == null) first_letter_in_uppercase = true;
  result = util.string.gsub(lower_case_and_underscored_word, /\/(.?)/, function($) {
    return "." + (util.string.upcase($[1]));
  });
  result = util.string.gsub(result, /(?:_)(.)/, function($) {
    return util.string.upcase($[1]);
  });
  if (first_letter_in_uppercase) {
    return util.string.upcase(result);
  } else {
    return util.string.downcase(result);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.flatiron.common.clone"></a>[function <span class="apidocSignatureSpan">flatiron.common.</span>clone (object, filter)](#apidoc.element.flatiron.common.clone)
- description and source-code
```javascript
clone = function (object, filter) {
  return Object.keys(object).reduce(filter ? function (obj, k) {
    if (filter(k)) obj[k] = object[k];
    return obj;
  } : function (obj, k) {
    obj[k] = object[k];
    return obj;
  }, {});
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.flatiron.common.createPath"></a>[function <span class="apidocSignatureSpan">flatiron.common.</span>createPath (obj, path, value)](#apidoc.element.flatiron.common.createPath)
- description and source-code
```javascript
createPath = function (obj, path, value) {
  var key, i;

  for (i in path) {
    key = path[i];
    if (!obj[key]) {
      obj[key] = ((+i + 1 === path.length) ? value : {});
    }

    obj = obj[key];
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.flatiron.common.debug"></a>[function <span class="apidocSignatureSpan">flatiron.common.</span>debug ()](#apidoc.element.flatiron.common.debug)
- description and source-code
```javascript
function deprecated() {
  warned = exports.printDeprecationMessage(msg, warned, deprecated);
  if (new.target) {
    return Reflect.construct(fn, arguments, new.target);
  }
  return fn.apply(this, arguments);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.flatiron.common.debuglog"></a>[function <span class="apidocSignatureSpan">flatiron.common.</span>debuglog (set)](#apidoc.element.flatiron.common.debuglog)
- description and source-code
```javascript
debuglog = function (set) {
  if (debugEnviron === undefined)
    debugEnviron = process.env.NODE_DEBUG || '';
  set = set.toUpperCase();
  if (!debugs[set]) {
    if (new RegExp('\\b${set}\\b', 'i').test(debugEnviron)) {
      var pid = process.pid;
      debugs[set] = function() {
        var msg = exports.format.apply(exports, arguments);
        console.error('%s %d: %s', set, pid, msg);
      };
    } else {
      debugs[set] = function() {};
    }
  }
  return debugs[set];
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.flatiron.common.deprecate"></a>[function <span class="apidocSignatureSpan">flatiron.common.</span>deprecate (fn, msg)](#apidoc.element.flatiron.common.deprecate)
- description and source-code
```javascript
deprecate = function (fn, msg) {
  // Allow for deprecating things in the process of starting up.
  if (global.process === undefined) {
    return function() {
      return exports._deprecate(fn, msg).apply(this, arguments);
    };
  }

  if (process.noDeprecation === true) {
    return fn;
  }

  var warned = false;
  function deprecated() {
    warned = exports.printDeprecationMessage(msg, warned, deprecated);
    if (new.target) {
      return Reflect.construct(fn, arguments, new.target);
    }
    return fn.apply(this, arguments);
  }

  // The wrapper will keep the same prototype as fn to maintain prototype chain
  Object.setPrototypeOf(deprecated, fn);
  if (fn.prototype) {
    // Setting this (rather than using Object.setPrototype, as above) ensures
    // that calling the unwrapped constructor gives an instanceof the wrapped
    // constructor.
    deprecated.prototype = fn.prototype;
  }

  return deprecated;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.flatiron.common.each"></a>[function <span class="apidocSignatureSpan">flatiron.common.</span>each (obj, iterator)](#apidoc.element.flatiron.common.each)
- description and source-code
```javascript
each = function (obj, iterator) {
  Object.keys(obj).forEach(function (key) {
    iterator(obj[key], key, obj);
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.flatiron.common.error"></a>[function <span class="apidocSignatureSpan">flatiron.common.</span>error ()](#apidoc.element.flatiron.common.error)
- description and source-code
```javascript
function deprecated() {
  warned = exports.printDeprecationMessage(msg, warned, deprecated);
  if (new.target) {
    return Reflect.construct(fn, arguments, new.target);
  }
  return fn.apply(this, arguments);
}
```
- example usage
```shell
...

app.commands.friendly = function (cb) {
  cb(null);
}

app.start(function (err) {
  if (err) {
    app.log.error(err.message || 'You didn\'t call any commands!');
    app.log.warn('NOT OK.');
    return process.exit(1);
  }
  app.log.info('OK.');
});
'''
...
```

#### <a name="apidoc.element.flatiron.common.escapeRegExp"></a>[function <span class="apidocSignatureSpan">flatiron.common.</span>escapeRegExp (str)](#apidoc.element.flatiron.common.escapeRegExp)
- description and source-code
```javascript
escapeRegExp = function (str) {
  return str.replace(/[\-\[\]\/\{\}\(\)\*\+\?\.\\\^\$\|]/g, "\\$&");
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.flatiron.common.filter"></a>[function <span class="apidocSignatureSpan">flatiron.common.</span>filter (obj, pred)](#apidoc.element.flatiron.common.filter)
- description and source-code
```javascript
filter = function (obj, pred) {
  var copy;
  if (Array.isArray(obj)) {
    copy = [];
    utile.each(obj, function (val, key) {
      if (pred(val, key, obj)) {
        copy.push(val);
      }
    });
  }
  else {
    copy = {};
    utile.each(obj, function (val, key) {
      if (pred(val, key, obj)) {
        copy[key] = val;
      }
    });
  }
  return copy;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.flatiron.common.find"></a>[function <span class="apidocSignatureSpan">flatiron.common.</span>find (obj, pred)](#apidoc.element.flatiron.common.find)
- description and source-code
```javascript
find = function (obj, pred) {
  var value, key;

  for (key in obj) {
    value = obj[key];
    if (pred(value, key)) {
      return value;
    }
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.flatiron.common.inherits"></a>[function <span class="apidocSignatureSpan">flatiron.common.</span>inherits (ctor, superCtor)](#apidoc.element.flatiron.common.inherits)
- description and source-code
```javascript
inherits = function (ctor, superCtor) {

  if (ctor === undefined || ctor === null)
    throw new TypeError('The constructor to "inherits" must not be ' +
                        'null or undefined');

  if (superCtor === undefined || superCtor === null)
    throw new TypeError('The super constructor to "inherits" must not ' +
                        'be null or undefined');

  if (superCtor.prototype === undefined)
    throw new TypeError('The super constructor to "inherits" must ' +
                        'have a prototype');

  ctor.super_ = superCtor;
  Object.setPrototypeOf(ctor.prototype, superCtor.prototype);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.flatiron.common.inspect"></a>[function <span class="apidocSignatureSpan">flatiron.common.</span>inspect (obj, opts)](#apidoc.element.flatiron.common.inspect)
- description and source-code
```javascript
function inspect(obj, opts) {
  // default options
  var ctx = {
    seen: [],
    stylize: stylizeNoColor
  };
  // legacy...
  if (arguments[2] !== undefined) ctx.depth = arguments[2];
  if (arguments[3] !== undefined) ctx.colors = arguments[3];
  if (typeof opts === 'boolean') {
    // legacy...
    ctx.showHidden = opts;
  }
  // Set default and user-specified options
  ctx = Object.assign({}, inspect.defaultOptions, ctx, opts);
  if (ctx.colors) ctx.stylize = stylizeWithColor;
  if (ctx.maxArrayLength === null) ctx.maxArrayLength = Infinity;
  return formatValue(ctx, obj, ctx.depth);
}
```
- example usage
```shell
...
this.res.end('Hello world!\n');
});

// POST to /
app.router.post('/', function () {
this.res.writeHead(200, { 'Content-Type': 'text/plain' });
this.res.write('Hey, you posted some cool data!\n');
this.res.end(util.inspect(this.req.body, true, 2, true) + '\n');
});

// Parameterized routes
app.router.get('/sandwich/:type', function (type) {
if (~['bacon', 'burger'].indexOf(type)) {
  this.res.writeHead(200, { 'Content-Type': 'text/plain' });
  this.res.end('Serving ' + type + ' sandwich!\n');
...
```

#### <a name="apidoc.element.flatiron.common.isArray"></a>[function <span class="apidocSignatureSpan">flatiron.common.</span>isArray ()](#apidoc.element.flatiron.common.isArray)
- description and source-code
```javascript
function isArray() { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.flatiron.common.isBoolean"></a>[function <span class="apidocSignatureSpan">flatiron.common.</span>isBoolean (arg)](#apidoc.element.flatiron.common.isBoolean)
- description and source-code
```javascript
function isBoolean(arg) {
  return typeof arg === 'boolean';
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.flatiron.common.isBuffer"></a>[function <span class="apidocSignatureSpan">flatiron.common.</span>isBuffer (b)](#apidoc.element.flatiron.common.isBuffer)
- description and source-code
```javascript
function isBuffer(b) {
  return b instanceof Buffer;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.flatiron.common.isDate"></a>[function <span class="apidocSignatureSpan">flatiron.common.</span>isDate (d)](#apidoc.element.flatiron.common.isDate)
- description and source-code
```javascript
function isDate(d) {
  return binding.isDate(d);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.flatiron.common.isError"></a>[function <span class="apidocSignatureSpan">flatiron.common.</span>isError (e)](#apidoc.element.flatiron.common.isError)
- description and source-code
```javascript
function isError(e) {
  return exports.objectToString(e) === '[object Error]' || e instanceof Error;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.flatiron.common.isFunction"></a>[function <span class="apidocSignatureSpan">flatiron.common.</span>isFunction (arg)](#apidoc.element.flatiron.common.isFunction)
- description and source-code
```javascript
function isFunction(arg) {
  return typeof arg === 'function';
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.flatiron.common.isNull"></a>[function <span class="apidocSignatureSpan">flatiron.common.</span>isNull (arg)](#apidoc.element.flatiron.common.isNull)
- description and source-code
```javascript
function isNull(arg) {
  return arg === null;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.flatiron.common.isNullOrUndefined"></a>[function <span class="apidocSignatureSpan">flatiron.common.</span>isNullOrUndefined (arg)](#apidoc.element.flatiron.common.isNullOrUndefined)
- description and source-code
```javascript
function isNullOrUndefined(arg) {
  return arg === null || arg === undefined;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.flatiron.common.isNumber"></a>[function <span class="apidocSignatureSpan">flatiron.common.</span>isNumber (arg)](#apidoc.element.flatiron.common.isNumber)
- description and source-code
```javascript
function isNumber(arg) {
  return typeof arg === 'number';
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.flatiron.common.isObject"></a>[function <span class="apidocSignatureSpan">flatiron.common.</span>isObject (arg)](#apidoc.element.flatiron.common.isObject)
- description and source-code
```javascript
function isObject(arg) {
  return arg !== null && typeof arg === 'object';
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.flatiron.common.isPrimitive"></a>[function <span class="apidocSignatureSpan">flatiron.common.</span>isPrimitive (arg)](#apidoc.element.flatiron.common.isPrimitive)
- description and source-code
```javascript
function isPrimitive(arg) {
  return arg === null ||
         typeof arg !== 'object' && typeof arg !== 'function';
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.flatiron.common.isRegExp"></a>[function <span class="apidocSignatureSpan">flatiron.common.</span>isRegExp (re)](#apidoc.element.flatiron.common.isRegExp)
- description and source-code
```javascript
function isRegExp(re) {
  return binding.isRegExp(re);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.flatiron.common.isString"></a>[function <span class="apidocSignatureSpan">flatiron.common.</span>isString (arg)](#apidoc.element.flatiron.common.isString)
- description and source-code
```javascript
function isString(arg) {
  return typeof arg === 'string';
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.flatiron.common.isSymbol"></a>[function <span class="apidocSignatureSpan">flatiron.common.</span>isSymbol (arg)](#apidoc.element.flatiron.common.isSymbol)
- description and source-code
```javascript
function isSymbol(arg) {
  return typeof arg === 'symbol';
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.flatiron.common.isUndefined"></a>[function <span class="apidocSignatureSpan">flatiron.common.</span>isUndefined (arg)](#apidoc.element.flatiron.common.isUndefined)
- description and source-code
```javascript
function isUndefined(arg) {
  return arg === undefined;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.flatiron.common.log"></a>[function <span class="apidocSignatureSpan">flatiron.common.</span>log ()](#apidoc.element.flatiron.common.log)
- description and source-code
```javascript
log = function () {
  console.log('%s - %s', timestamp(), exports.format.apply(exports, arguments));
}
```
- example usage
```shell
...
};

app.use(hello, {
  message: "Hi! How are you?"
});

// Will print, "Hi! How are you?"
console.log(app.hello);
'''

Virtually all additional functionality in flatiron comes from broadway plugins, such as 'flatiron.plugins.http' and 'flatiron.plugins
.cli'.

### 'app.config'

'flatiron.app' comes with a ['config'](https://github.com/flatiron/broadway/blob/master/lib/broadway/plugins/config.js) plugin pre
-loaded, which adds configuration management courtesy [nconf](https://github.com/flatiron/nconf). 'app.config' has the same api
as the 'nconf' object.
...
```

#### <a name="apidoc.element.flatiron.common.mixin"></a>[function <span class="apidocSignatureSpan">flatiron.common.</span>mixin (target)](#apidoc.element.flatiron.common.mixin)
- description and source-code
```javascript
mixin = function (target) {
  utile.rargs(arguments, 1).forEach(function (o) {
    Object.getOwnPropertyNames(o).forEach(function(attr) {
      var getter = Object.getOwnPropertyDescriptor(o, attr).get,
          setter = Object.getOwnPropertyDescriptor(o, attr).set;

      if (!getter && !setter) {
        target[attr] = o[attr];
      }
      else {
        Object.defineProperty(target, attr, {
          get: getter,
          set: setter
        });
      }
    });
  });

  return target;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.flatiron.common.pad"></a>[function <span class="apidocSignatureSpan">flatiron.common.</span>pad (str, len, chr)](#apidoc.element.flatiron.common.pad)
- description and source-code
```javascript
function pad(str, len, chr) {
  var s;
  if (!chr) {
    chr = ' ';
  }
  str = str || '';
  s = str;
  if (str.length < len) {
    for (var i = 0; i < (len - str.length); i++) {
      s += chr;
    }
  }
  return s;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.flatiron.common.path"></a>[function <span class="apidocSignatureSpan">flatiron.common.</span>path (obj, path)](#apidoc.element.flatiron.common.path)
- description and source-code
```javascript
path = function (obj, path) {
  var key, i;

  for (i in path) {
    if (typeof obj === 'undefined') {
      return undefined;
    }

    key = path[i];
    obj = obj[key];
  }

  return obj;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.flatiron.common.print"></a>[function <span class="apidocSignatureSpan">flatiron.common.</span>print ()](#apidoc.element.flatiron.common.print)
- description and source-code
```javascript
function deprecated() {
  warned = exports.printDeprecationMessage(msg, warned, deprecated);
  if (new.target) {
    return Reflect.construct(fn, arguments, new.target);
  }
  return fn.apply(this, arguments);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.flatiron.common.puts"></a>[function <span class="apidocSignatureSpan">flatiron.common.</span>puts ()](#apidoc.element.flatiron.common.puts)
- description and source-code
```javascript
function deprecated() {
  warned = exports.printDeprecationMessage(msg, warned, deprecated);
  if (new.target) {
    return Reflect.construct(fn, arguments, new.target);
  }
  return fn.apply(this, arguments);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.flatiron.common.randomString"></a>[function <span class="apidocSignatureSpan">flatiron.common.</span>randomString (length)](#apidoc.element.flatiron.common.randomString)
- description and source-code
```javascript
randomString = function (length) {
  var chars, rand, i, ret, mod, bits;

  chars = 'ABCDEFGHIJKLMNOPQRSTUVWXYZabcdefghijklmnopqrstuvwxyz0123456789_-';
  ret = '';
  // standard 4
  mod = 4;
  // default is 16
  bits = length * mod || 64;

  // in v8, Math.random() yields 32 pseudo-random bits (in spidermonkey it gives 53)
  while (bits > 0) {
    // 32-bit integer
    rand = Math.floor(Math.random() * 0x100000000);
    //we use the top bits
    for (i = 26; i > 0 && bits > 0; i -= mod, bits -= mod) {
      ret += chars[0x3F & rand >>> i];
    }
  }

  return ret;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.flatiron.common.rargs"></a>[function <span class="apidocSignatureSpan">flatiron.common.</span>rargs (_args, slice)](#apidoc.element.flatiron.common.rargs)
- description and source-code
```javascript
rargs = function (_args, slice) {
  if (!slice) {
    slice = 0;
  }

  var len = (_args || []).length,
      args = new Array(len - slice),
      i;

  //
  // Convert the raw '_args' to a proper Array.
  //
  for (i = slice; i < len; i++) {
    args[i - slice] = _args[i];
  }

  return args;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.flatiron.common.requireDir"></a>[function <span class="apidocSignatureSpan">flatiron.common.</span>requireDir (directory)](#apidoc.element.flatiron.common.requireDir)
- description and source-code
```javascript
requireDir = function (directory) {
  var result = {},
      files = fs.readdirSync(directory);

  files.forEach(function (file) {
    if (file.substr(-3) === '.js') {
      file = file.substr(0, file.length - 3);
    }
    result[file] = require(path.resolve(directory, file));
  });
  return result;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.flatiron.common.requireDirLazy"></a>[function <span class="apidocSignatureSpan">flatiron.common.</span>requireDirLazy (directory)](#apidoc.element.flatiron.common.requireDirLazy)
- description and source-code
```javascript
requireDirLazy = function (directory) {
  var result = {},
      files = fs.readdirSync(directory);

  files.forEach(function (file) {
    if (file.substr(-3) === '.js') {
      file = file.substr(0, file.length - 3);
    }
    Object.defineProperty(result, file, {
      get: function() {
        return result[file] = require(path.resolve(directory, file));
      }
    });
  });

  return result;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.flatiron.common.templateUsage"></a>[function <span class="apidocSignatureSpan">flatiron.common.</span>templateUsage (app, commands)](#apidoc.element.flatiron.common.templateUsage)
- description and source-code
```javascript
templateUsage = function (app, commands) {
  if (!app.name) {
    return commands;
  }

  function templateUsage(usage) {
    return usage.map(function (line) {
      return line.replace(/\<app\>/ig, app.name);
    });
  }

  Object.keys(commands).forEach(function (command) {
    if (command === 'usage') {
      commands.usage = templateUsage(commands.usage);
    }
    else if (commands[command].usage) {
      commands[command].usage = templateUsage(commands[command].usage);
    }
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.flatiron.common.tryReaddirSync"></a>[function <span class="apidocSignatureSpan">flatiron.common.</span>tryReaddirSync (dir)](#apidoc.element.flatiron.common.tryReaddirSync)
- description and source-code
```javascript
tryReaddirSync = function (dir) {
  try { return fs.readdirSync(dir) }
  catch (err) { return [] }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.flatiron.common.underscoreToCamel"></a>[function <span class="apidocSignatureSpan">flatiron.common.</span>underscoreToCamel (obj)](#apidoc.element.flatiron.common.underscoreToCamel)
- description and source-code
```javascript
underscoreToCamel = function (obj) {
  if (typeof obj !== 'object' || obj === null) {
    return obj;
  }

  if (Array.isArray(obj)) {
    obj.forEach(utile.underscoreToCamel);
    return obj;
  }

  Object.keys(obj).forEach(function (key) {
    var k = utile.inflect.camelize(key, false);
    if (k !== key) {
      obj[k] = obj[key];
      delete obj[key];
      key = k;
    }
    utile.underscoreToCamel(obj[key]);
  });

  return obj;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.flatiron.common.uuid"></a>[function <span class="apidocSignatureSpan">flatiron.common.</span>uuid ()](#apidoc.element.flatiron.common.uuid)
- description and source-code
```javascript
uuid = function () {
  return String(id++);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.flatiron.common.directories"></a>[module flatiron.common.directories](#apidoc.module.flatiron.common.directories)

#### <a name="apidoc.element.flatiron.common.directories.create"></a>[function <span class="apidocSignatureSpan">flatiron.common.directories.</span>create (dirs, callback)](#apidoc.element.flatiron.common.directories.create)
- description and source-code
```javascript
create = function (dirs, callback) {
  function createDir(dir, next) {
    mkdirp(dir, 0755, function () {
      next(null, dir);
    });
  }

  if (!dirs) {
    return callback();
  }

  async.mapSeries(Object.keys(dirs).map(function (key) {
    return dirs[key]
  }), createDir, callback);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.flatiron.common.directories.normalize"></a>[function <span class="apidocSignatureSpan">flatiron.common.directories.</span>normalize (keys, dirs)](#apidoc.element.flatiron.common.directories.normalize)
- description and source-code
```javascript
normalize = function (keys, dirs) {
  var normalized = {};

  Object.keys(dirs).forEach(function (key) {
    normalized[key] = dirs[key];
    Object.keys(keys).forEach(function (constant) {
      normalized[key] = normalized[key].replace(constant, keys[constant]);
    });
  });

  return normalized;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.flatiron.common.directories.remove"></a>[function <span class="apidocSignatureSpan">flatiron.common.directories.</span>remove (dirs, callback)](#apidoc.element.flatiron.common.directories.remove)
- description and source-code
```javascript
remove = function (dirs, callback) {
  function removeDir (dir, next) {
    rimraf(dir, function () {
      next(null, dir);
    });
  }

  if (!dirs) {
    return callback();
  }

  async.mapSeries(Object.keys(dirs).map(function (key) {
    return dirs[key]
  }), removeDir, callback);
}
```
- example usage
```shell
...
// add the 'file' store the the config
app.config.use('file', { file: 'path/to/config.json' });

// or using an alternate syntax
app.config.env().file({ file: 'path/to/config.json' });

// and removing stores
app.config.remove('literal');
'''

### 'app.log'

'flatiron.app' will also load a ['log'](https://github.com/flatiron/broadway/blob/master/lib/broadway/plugins/log.js) plugin during
 the init phase, which attaches a [winston container](https://github.com/flatiron/winston) to 'app.log'. This logger is configured
 by combining the 'app.options.log' property with the configuration retrieved from 'app.config.get('log')'.

## Create An HTTP Server with 'flatiron.plugins.http(options)':
...
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
