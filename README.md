# api documentation for  [trails (v2.0.2)](http://trailsjs.io)  [![npm package](https://img.shields.io/npm/v/npmdoc-trails.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-trails) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-trails.svg)](https://travis-ci.org/npmdoc/node-npmdoc-trails)
#### Modern Web Application Framework for Node.js

[![NPM](https://nodei.co/npm/trails.png?downloads=true)](https://www.npmjs.com/package/trails)

[![apidoc](https://npmdoc.github.io/node-npmdoc-trails/build/screenCapture.buildNpmdoc.browser._2Fhome_2Ftravis_2Fbuild_2Fnpmdoc_2Fnode-npmdoc-trails_2Ftmp_2Fbuild_2Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-trails/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-trails/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-trails/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Trails.js Team",
        "email": "hello@trailsjs.io"
    },
    "bugs": {
        "url": "https://github.com/trailsjs/trails/issues"
    },
    "bundleDependencies": [
        "trails-controller",
        "trails-model",
        "trails-policy",
        "trails-service"
    ],
    "contributors": [
        {
            "name": "Travis Webb",
            "email": "me@traviswebb.com",
            "url": "https://github.com/tjwebb"
        },
        {
            "name": "Konstantin Zolotarev",
            "url": "https://github.com/konstantinzolotarev"
        },
        {
            "name": "Weyland Joyner",
            "url": "https://github.com/weyj4"
        },
        {
            "name": "Jimmy Aumard",
            "url": "https://github.com/jaumard"
        },
        {
            "name": "Robert Rossmann",
            "url": "https://github.com/Alaneor"
        },
        {
            "name": "Mike Hostetler",
            "email": "mike@epicfirm.com"
        }
    ],
    "dependencies": {
        "hoek": "^4.1.0",
        "i18next": "^3.4.1",
        "joi": "^10.2.2",
        "lodash": "^4.17.2",
        "mkdirp": "^0.5.1",
        "trails-controller": "^2",
        "trails-model": "^2",
        "trails-policy": "^2",
        "trails-service": "^2"
    },
    "description": "Modern Web Application Framework for Node.js",
    "devDependencies": {
        "eslint": "^3.15.0",
        "eslint-config-trails": "^2.0.8",
        "istanbul": "^0.4.5",
        "mocha": "^3.2.0",
        "pre-commit": "^1.2.2",
        "smokesignals": "^2.1.0",
        "trailpack": "^2",
        "winston": "^2.3.1"
    },
    "directories": {},
    "dist": {
        "shasum": "58b4b4bc0f49f18a279a0aa3afce813ab4594431",
        "tarball": "https://registry.npmjs.org/trails/-/trails-2.0.2.tgz"
    },
    "engines": {
        "node": ">= 4.0.0",
        "npm": ">= 2.14.2"
    },
    "eslintConfig": {
        "extends": "trails"
    },
    "gitHead": "308dac16768f8d90f21924cb7824e5f4a4282744",
    "homepage": "http://trailsjs.io",
    "keywords": [
        "framework",
        "platform",
        "rest",
        "api",
        "rails",
        "grails",
        "sails",
        "trails",
        "trailsjs",
        "server",
        "graphql"
    ],
    "license": "MIT",
    "maintainers": [
        {
            "name": "trails",
            "email": "trailsjs@balderdash.io"
        }
    ],
    "name": "trails",
    "optionalDependencies": {},
    "pre-commit": [
        "test"
    ],
    "publishConfig": {
        "tag": "next"
    },
    "readme": "ERROR: No README data found!",
    "repository": {
        "type": "git",
        "url": "git+https://github.com/trailsjs/trails.git"
    },
    "runkitExample": "test/runkitExample.js",
    "scripts": {
        "ci": "cd .. && ci",
        "coverage": "istanbul cover node_modules/mocha/bin/_mocha",
        "test": "eslint --ignore-path .gitignore . && istanbul cover node_modules/mocha/bin/_mocha",
        "test-performance": "eslint . && mocha test-performance"
    },
    "version": "2.0.2"
}
```



# <a name="apidoc.tableOfContents"></a>[table of contents](#apidoc.tableOfContents)

#### [module trails](#apidoc.module.trails)
1.  object <span class="apidocSignatureSpan">trails.</span>core
1.  object <span class="apidocSignatureSpan">trails.</span>pathfinder
1.  object <span class="apidocSignatureSpan">trails.</span>trailpack

#### [module trails.core](#apidoc.module.trails.core)
1.  [function <span class="apidocSignatureSpan">trails.core.</span>assignGlobals ()](#apidoc.element.trails.core.assignGlobals)
1.  [function <span class="apidocSignatureSpan">trails.core.</span>bindApplicationListeners (app)](#apidoc.element.trails.core.bindApplicationListeners)
1.  [function <span class="apidocSignatureSpan">trails.core.</span>bindListeners (app)](#apidoc.element.trails.core.bindListeners)
1.  [function <span class="apidocSignatureSpan">trails.core.</span>bindMethods (app, resource)](#apidoc.element.trails.core.bindMethods)
1.  [function <span class="apidocSignatureSpan">trails.core.</span>createDefaultPaths (app)](#apidoc.element.trails.core.createDefaultPaths)
1.  [function <span class="apidocSignatureSpan">trails.core.</span>getClassMethods (obj)](#apidoc.element.trails.core.getClassMethods)
1.  [function <span class="apidocSignatureSpan">trails.core.</span>getExternalModules ()](#apidoc.element.trails.core.getExternalModules)
1.  [function <span class="apidocSignatureSpan">trails.core.</span>unbindListeners (app)](#apidoc.element.trails.core.unbindListeners)
1.  object <span class="apidocSignatureSpan">trails.core.</span>globalPropertyOptions
1.  object <span class="apidocSignatureSpan">trails.core.</span>globals
1.  object <span class="apidocSignatureSpan">trails.core.</span>reservedMethods

#### [module trails.pathfinder](#apidoc.module.trails.pathfinder)
1.  [function <span class="apidocSignatureSpan">trails.pathfinder.</span>getEventProducer (eventName, stageName, packs, path)](#apidoc.element.trails.pathfinder.getEventProducer)
1.  [function <span class="apidocSignatureSpan">trails.pathfinder.</span>getLifecyclePath (pack, stageName, packs, path)](#apidoc.element.trails.pathfinder.getLifecyclePath)
1.  [function <span class="apidocSignatureSpan">trails.pathfinder.</span>getPathErrors (path)](#apidoc.element.trails.pathfinder.getPathErrors)
1.  [function <span class="apidocSignatureSpan">trails.pathfinder.</span>isComplete (packs)](#apidoc.element.trails.pathfinder.isComplete)
1.  [function <span class="apidocSignatureSpan">trails.pathfinder.</span>isLifecycleStageValid (pack, stageName, packs)](#apidoc.element.trails.pathfinder.isLifecycleStageValid)
1.  [function <span class="apidocSignatureSpan">trails.pathfinder.</span>isLifecycleValid (pack, packs)](#apidoc.element.trails.pathfinder.isLifecycleValid)

#### [module trails.trailpack](#apidoc.module.trails.trailpack)
1.  [function <span class="apidocSignatureSpan">trails.trailpack.</span>bindTrailpackMethodListeners (app, packs)](#apidoc.element.trails.trailpack.bindTrailpackMethodListeners)
1.  [function <span class="apidocSignatureSpan">trails.trailpack.</span>bindTrailpackPhaseListeners (app, packs)](#apidoc.element.trails.trailpack.bindTrailpackPhaseListeners)



# <a name="apidoc.module.trails"></a>[module trails](#apidoc.module.trails)



# <a name="apidoc.module.trails.core"></a>[module trails.core](#apidoc.module.trails.core)

#### <a name="apidoc.element.trails.core.assignGlobals"></a>[function <span class="apidocSignatureSpan">trails.core.</span>assignGlobals ()](#apidoc.element.trails.core.assignGlobals)
- description and source-code
```javascript
assignGlobals() {
  _.each(lib.Core.globals, (type, name) => {
    if (global[name] === type) return
    if (global[name] && global[name] !== type) {
      throw new lib.Errors.NamespaceConflictError(name, Object.keys(lib.Core.globals))
    }
    const descriptor = Object.assign({ value: type }, lib.Core.globalPropertyOptions)
    Object.defineProperty(global, name, descriptor)
  })
}
```
- example usage
```shell
...

const EventEmitter = require('events').EventEmitter
const lib = require('./lib')
const i18next = require('i18next')
const NOOP = function () { }

// inject Error and Resource types into the global namespace
lib.Core.assignGlobals()

/**
 * The Trails Application. Merges the configuration and API resources
 * loads Trailpacks, initializes logging and event listeners.
 */
module.exports = class TrailsApp extends EventEmitter {
...
```

#### <a name="apidoc.element.trails.core.bindApplicationListeners"></a>[function <span class="apidocSignatureSpan">trails.core.</span>bindApplicationListeners (app)](#apidoc.element.trails.core.bindApplicationListeners)
- description and source-code
```javascript
bindApplicationListeners(app) {
  app.once('trailpack:all:configured', () => {
    if (app.config.main.freezeConfig !== true) {
      app.log.warn('freezeConfig is disabled. Configuration will not be frozen.')
      app.log.warn('Please only use this flag for testing/debugging purposes.')
    }

    app.freezeConfig()
  })
  app.once('trailpack:all:initialized', () => {
    app.log.silly(app.config.motd.silly.initialized)
    app.log.info(app.config.motd.info.initialized)
  })
  app.once('trails:ready', () => {
    app.log.info(app.config.motd.info.ready(app))
    app.log.debug(app.config.motd.debug.ready(app))
    app.log.silly(app.config.motd.silly.ready(app))

    app.log.info(app.config.motd.hr)
  })
  app.once('trails:stop', () => {
    app.log.silly(app.config.motd.silly.stop)
    app.log.info(app.config.motd.info.stop)
    app.unfreezeConfig()
  })
  app.once('trails:error:fatal', err => app.stop(err))
}
```
- example usage
```shell
...
bindListeners (app) {
  if (app.bound) {
    app.log.warn('Someone attempted to bindListeners() twice! Stacktrace below.')
    app.log.warn(console.trace())   // eslint-disable-line no-console
    return
  }

  Core.bindApplicationListeners(app)
  app.bound = true
},

/**
 * Bind listeners to trails application events
 */
bindApplicationListeners (app) {
...
```

#### <a name="apidoc.element.trails.core.bindListeners"></a>[function <span class="apidocSignatureSpan">trails.core.</span>bindListeners (app)](#apidoc.element.trails.core.bindListeners)
- description and source-code
```javascript
bindListeners(app) {
  if (app.bound) {
    app.log.warn('Someone attempted to bindListeners() twice! Stacktrace below.')
    app.log.warn(console.trace())   // eslint-disable-line no-console
    return
  }

  Core.bindApplicationListeners(app)
  app.bound = true
}
```
- example usage
```shell
...

  /**
   * Start the App. Load all Trailpacks.
   *
   * @return Promise
   */
  start () {
lib.Core.bindListeners(this)
lib.Trailpack.bindTrailpackPhaseListeners(this, this.loadedPacks)
lib.Trailpack.bindTrailpackMethodListeners(this, this.loadedPacks)

// initialize i18n
i18next.init(this.config.i18n, (err, t) => {
  if (err) {
    throw new Error('Problem loading i18n: ${err}')
...
```

#### <a name="apidoc.element.trails.core.bindMethods"></a>[function <span class="apidocSignatureSpan">trails.core.</span>bindMethods (app, resource)](#apidoc.element.trails.core.bindMethods)
- description and source-code
```javascript
bindMethods(app, resource) {
  return _.mapValues(app.api[resource], (Resource, resourceName) => {
    if (_.isPlainObject(Resource)) {
      throw new Error('${resourceName} should be a class. It is a regular object')
    }

    const obj = new Resource(app)

    obj.methods = Core.getClassMethods(obj)
    _.forEach(obj.methods, method => {
      obj[method] = obj[method].bind(obj)
    })
    return obj
  })
}
```
- example usage
```shell
...
    catch (e) {
      throw new TrailpackError(Pack, e, 'constructor')
    }
  })
  this.loadedPacks = Object.keys(this.packs).map(name => this.packs[name])

  // bind resource methods
  Object.assign(this.models, lib.Core.bindMethods(this, 'models'))
  Object.assign(this.services, lib.Core.bindMethods(this, 'services'))
  Object.assign(this.controllers, lib.Core.bindMethods(this, 'controllers'))
  Object.assign(this.policies, lib.Core.bindMethods(this, 'policies'))
}

/**
 * Start the App. Load all Trailpacks.
...
```

#### <a name="apidoc.element.trails.core.createDefaultPaths"></a>[function <span class="apidocSignatureSpan">trails.core.</span>createDefaultPaths (app)](#apidoc.element.trails.core.createDefaultPaths)
- description and source-code
```javascript
createDefaultPaths(app) {
  const paths = app.config.main.paths

  return Promise.all(_.map(paths, (dir, pathName) => {
    return new Promise((resolve, reject) => {
      fs.stat(dir, (err, stats) => {
        resolve({ err, stats })
      })
    })
    .then(result => {
      const stats = result.stats

      if (stats && !stats.isDirectory()) {
        app.log.error('The configured path "', pathName, '" is not a directory.')
        app.log.error('config.main.paths should only contain paths to directories')
        return Promise.reject()
      }

      return result
    })
    .then(stat => {
      if (stat.err && /no such file or directory/.test(stat.err.message)) {
        app.log.debug('Trails is creating the path (', pathName, ') at', dir)
      }
      mkdirp.sync(dir)
    })
  }))
}
```
- example usage
```shell
...
/**
 * Create any configured paths which may not already exist.
 */
createPaths () {
  if (this.config.main.createPaths === false) {
    this.log.warn('createPaths is disabled. Configured paths will not be created')
  }
  return lib.Core.createDefaultPaths(this)
}

/**
 * Expose the logger on the app object. The logger can be configured by
 * setting the "config.log.logger" config property.
 */
get log () {
...
```

#### <a name="apidoc.element.trails.core.getClassMethods"></a>[function <span class="apidocSignatureSpan">trails.core.</span>getClassMethods (obj)](#apidoc.element.trails.core.getClassMethods)
- description and source-code
```javascript
getClassMethods(obj) {
  const props = [ ]
  const objectRoot = new Object()

  while (!obj.isPrototypeOf(objectRoot)) {
    Object.getOwnPropertyNames(obj).forEach(prop => {
      if (props.indexOf(prop) === -1 &&
          !_.includes(Core.reservedMethods, prop) &&
          _.isFunction(obj[prop])) {

        props.push(prop)
      }
    })
    obj = Object.getPrototypeOf(obj)
  }

  return props
}
```
- example usage
```shell
...
  return _.mapValues(app.api[resource], (Resource, resourceName) => {
    if (_.isPlainObject(Resource)) {
      throw new Error('${resourceName} should be a class. It is a regular object')
    }

    const obj = new Resource(app)

    obj.methods = Core.getClassMethods(obj)
    _.forEach(obj.methods, method => {
      obj[method] = obj[method].bind(obj)
    })
    return obj
  })
},
...
```

#### <a name="apidoc.element.trails.core.getExternalModules"></a>[function <span class="apidocSignatureSpan">trails.core.</span>getExternalModules ()](#apidoc.element.trails.core.getExternalModules)
- description and source-code
```javascript
getExternalModules() {
  const rootPath = path.resolve(path.dirname(require.main.filename))
  const modulePath = path.join(rootPath, 'node_modules')
  const requiredModules = Object.keys(require.cache).filter(mod => {
    return mod.indexOf(modulePath) >= 0
  })
  return requiredModules
}
```
- example usage
```shell
...
loadedPacks: {
  enumerable: false,
  writable: true,
  value: [ ]
},
loadedModules: {
  enumerable: false,
  value: lib.Core.getExternalModules(this.pkg)
},
bound: {
  enumerable: false,
  writable: true,
  value: false
},
started: {
...
```

#### <a name="apidoc.element.trails.core.unbindListeners"></a>[function <span class="apidocSignatureSpan">trails.core.</span>unbindListeners (app)](#apidoc.element.trails.core.unbindListeners)
- description and source-code
```javascript
unbindListeners(app) {
  app.removeAllListeners()
  app.bound = false
}
```
- example usage
```shell
...
}
if (!this.started) {
  this.log.error('The application did not boot successfully.')
  this.log.error('Try increasing the loglevel to "debug" to learn more')
}

this.emit('trails:stop')
lib.Core.unbindListeners(this)

return Promise.all(
  this.loadedPacks.map(pack => {
    this.log.debug('Unloading trailpack', pack.name, '...')
    return pack.unload()
  }))
  .then(() => {
...
```



# <a name="apidoc.module.trails.pathfinder"></a>[module trails.pathfinder](#apidoc.module.trails.pathfinder)

#### <a name="apidoc.element.trails.pathfinder.getEventProducer"></a>[function <span class="apidocSignatureSpan">trails.pathfinder.</span>getEventProducer (eventName, stageName, packs, path)](#apidoc.element.trails.pathfinder.getEventProducer)
- description and source-code
```javascript
getEventProducer(eventName, stageName, packs, path) {
  const producers = packs
    .filter(pack => {
      const stage = pack.config.lifecycle[stageName]
      return path.indexOf(pack) === -1 && stage.emit.indexOf(eventName) >= 0
    })

  if (producers.length > 1) {
    return new Error('More than one trailpack produces the event ${eventName}')
  }
  if (producers.length === 0) {
    return new Errors.GraphCompletenessError(path[path.length - 1], stageName, eventName)
  }

  return producers[0]
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.trails.pathfinder.getLifecyclePath"></a>[function <span class="apidocSignatureSpan">trails.pathfinder.</span>getLifecyclePath (pack, stageName, packs, path)](#apidoc.element.trails.pathfinder.getLifecyclePath)
- description and source-code
```javascript
getLifecyclePath(pack, stageName, packs, path) {
  const stage = pack.config.lifecycle[stageName] || { }

  if (!path) {
    return Pathfinder.getLifecyclePath (pack, stageName, packs, [ pack ])
  }

  // terminate traversal. if current pack waits for no events, then it
  // necessarily reaches the sink, and indicates a complete path.
  if (!stage.listen || stage.listen.length === 0) {
    return true
  }

  // find all packs that produce the event(s) that the current pack requires
  const producers = stage.listen
    .map(eventName => {
      return Pathfinder.getEventProducer (eventName, stageName, packs, path)
    })
    .filter(producer => !!producer)


  // return first error encountered in this path. terminate traversal.
  // one or more of the required events are not available.
  const error = producers.find(producer => producer instanceof Errors.GraphCompletenessError)
  if (error) {
    return error
  }

  // all producers must themselves have complete paths.
  return producers.reduce((level, producer) => {
    const subpath = path.concat(producer)
    level[producer.name] = Pathfinder.getLifecyclePath(producer, stageName, packs, subpath)
    return level
  }, { })
}
```
- example usage
```shell
...
 * Return true if a particular stage is valid for the given pack; false
 * otherwise
 */
isLifecycleStageValid (pack, stageName, packs) {
  if (!stageName || lifecycleStages.indexOf(stageName) === -1) {
    throw new TypeError('isLifecycleStageValid: stageName must be one of ${lifecycleStages}')
  }
  const path = Pathfinder.getLifecyclePath(pack, stageName, packs)
  const terminals = Pathfinder.getPathErrors(path)
  return !terminals.some(t => t instanceof Error)
},

/**
 * Traverse the lifecycle path and return the terminal values for each of its
 * branches (lifecycle events)
...
```

#### <a name="apidoc.element.trails.pathfinder.getPathErrors"></a>[function <span class="apidocSignatureSpan">trails.pathfinder.</span>getPathErrors (path)](#apidoc.element.trails.pathfinder.getPathErrors)
- description and source-code
```javascript
getPathErrors(path) {
  if (typeof path === 'boolean') {
    return [ ]
  }
  if (path instanceof Error) {
    return [ path ]
  }
  return Object.keys(path)
    .map(key => Pathfinder.getPathErrors(path[key]))
    .reduce((terminals, t) => terminals.concat(t), [ ])
}
```
- example usage
```shell
...
 * otherwise
 */
isLifecycleStageValid (pack, stageName, packs) {
  if (!stageName || lifecycleStages.indexOf(stageName) === -1) {
    throw new TypeError('isLifecycleStageValid: stageName must be one of ${lifecycleStages}')
  }
  const path = Pathfinder.getLifecyclePath(pack, stageName, packs)
  const terminals = Pathfinder.getPathErrors(path)
  return !terminals.some(t => t instanceof Error)
},

/**
 * Traverse the lifecycle path and return the terminal values for each of its
 * branches (lifecycle events)
 */
...
```

#### <a name="apidoc.element.trails.pathfinder.isComplete"></a>[function <span class="apidocSignatureSpan">trails.pathfinder.</span>isComplete (packs)](#apidoc.element.trails.pathfinder.isComplete)
- description and source-code
```javascript
isComplete(packs) {
  return packs.every(pack => {
    return Pathfinder.isLifecycleValid (pack, packs)
  })
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.trails.pathfinder.isLifecycleStageValid"></a>[function <span class="apidocSignatureSpan">trails.pathfinder.</span>isLifecycleStageValid (pack, stageName, packs)](#apidoc.element.trails.pathfinder.isLifecycleStageValid)
- description and source-code
```javascript
isLifecycleStageValid(pack, stageName, packs) {
  if (!stageName || lifecycleStages.indexOf(stageName) === -1) {
    throw new TypeError('isLifecycleStageValid: stageName must be one of ${lifecycleStages}')
  }
  const path = Pathfinder.getLifecyclePath(pack, stageName, packs)
  const terminals = Pathfinder.getPathErrors(path)
  return !terminals.some(t => t instanceof Error)
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.trails.pathfinder.isLifecycleValid"></a>[function <span class="apidocSignatureSpan">trails.pathfinder.</span>isLifecycleValid (pack, packs)](#apidoc.element.trails.pathfinder.isLifecycleValid)
- description and source-code
```javascript
isLifecycleValid(pack, packs) {
  return lifecycleStages.every(stageName => {
    return Pathfinder.isLifecycleStageValid (pack, stageName, packs)
  })
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.trails.trailpack"></a>[module trails.trailpack](#apidoc.module.trails.trailpack)

#### <a name="apidoc.element.trails.trailpack.bindTrailpackMethodListeners"></a>[function <span class="apidocSignatureSpan">trails.trailpack.</span>bindTrailpackMethodListeners (app, packs)](#apidoc.element.trails.trailpack.bindTrailpackMethodListeners)
- description and source-code
```javascript
bindTrailpackMethodListeners(app, packs) {
  packs.map(pack => {
    const lifecycle = pack.config.lifecycle

    app.after(lifecycle.initialize.listen.concat('trailpack:all:configured'))
      .then(() => app.log.debug('trailpack: initializing', pack.name))
      .then(() => pack.initialize())
      .catch(err => app.stop(err))
      .then(() => app.emit('trailpack:${pack.name}:initialized'))

    app.after(lifecycle.configure.listen.concat('trailpack:all:validated'))
      .then(() => app.log.debug('trailpack: configuring', pack.name))
      .then(() => pack.configure())
      .catch(err => app.stop(err))
      .then(() => app.emit('trailpack:${pack.name}:configured'))

    app.after('trails:start')
      .then(() => app.log.debug('trailpack: validating', pack.name))
      .then(() => pack.validate())
      .catch(err => app.stop(err))
      .then(() => app.emit('trailpack:${pack.name}:validated'))
  })
}
```
- example usage
```shell
...
   * Start the App. Load all Trailpacks.
   *
   * @return Promise
   */
  start () {
lib.Core.bindListeners(this)
lib.Trailpack.bindTrailpackPhaseListeners(this, this.loadedPacks)
lib.Trailpack.bindTrailpackMethodListeners(this, this.loadedPacks)

// initialize i18n
i18next.init(this.config.i18n, (err, t) => {
  if (err) {
    throw new Error('Problem loading i18n: ${err}')
  }
...
```

#### <a name="apidoc.element.trails.trailpack.bindTrailpackPhaseListeners"></a>[function <span class="apidocSignatureSpan">trails.trailpack.</span>bindTrailpackPhaseListeners (app, packs)](#apidoc.element.trails.trailpack.bindTrailpackPhaseListeners)
- description and source-code
```javascript
bindTrailpackPhaseListeners(app, packs) {
  const validatedEvents = packs.map(pack => 'trailpack:${pack.name}:validated')
  const configuredEvents = packs.map(pack => 'trailpack:${pack.name}:configured')
  const initializedEvents = packs.map(pack => 'trailpack:${pack.name}:initialized')

  app.after(configuredEvents)
    .then(() => app.createPaths())
    .then(() => app.emit('trailpack:all:configured'))
    .catch(err => app.stop(err))

  app.after(validatedEvents)
    .then(() => app.emit('trailpack:all:validated'))
    .catch(err => app.stop(err))

  app.after(initializedEvents)
    .then(() => {
      app.emit('trailpack:all:initialized')
      app.emit('trails:ready')
    })
    .catch(err => app.stop(err))
}
```
- example usage
```shell
...
  /**
   * Start the App. Load all Trailpacks.
   *
   * @return Promise
   */
  start () {
lib.Core.bindListeners(this)
lib.Trailpack.bindTrailpackPhaseListeners(this, this.loadedPacks)
lib.Trailpack.bindTrailpackMethodListeners(this, this.loadedPacks)

// initialize i18n
i18next.init(this.config.i18n, (err, t) => {
  if (err) {
    throw new Error('Problem loading i18n: ${err}')
  }
...
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
