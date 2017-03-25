# api documentation for  [prompt (v1.0.0)](https://github.com/flatiron/prompt#readme)  [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-prompt.svg)](https://travis-ci.org/npmdoc/node-npmdoc-prompt)
#### A beautiful command-line prompt for node.js

[![NPM](https://nodei.co/npm/prompt.png?downloads=true)](https://www.npmjs.com/package/prompt)

[![apidoc](https://npmdoc.github.io/node-npmdoc-prompt/build/screen-capture.buildNpmdoc.browser._2Fhome_2Ftravis_2Fbuild_2Fnpmdoc_2Fnode-npmdoc-prompt_2Ftmp_2Fbuild_2Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-prompt/build..beta..travis-ci.org/apidoc.html)

![package-listing](https://npmdoc.github.io/node-npmdoc-prompt/build/screen-capture.npmPackageListing.svg)



# package.json

```json

{
    "author": {
        "name": "Nodejitsu Inc.",
        "email": "info@nodejitsu.com"
    },
    "bugs": {
        "url": "https://github.com/flatiron/prompt/issues"
    },
    "dependencies": {
        "colors": "^1.1.2",
        "pkginfo": "0.x.x",
        "read": "1.0.x",
        "revalidator": "0.1.x",
        "utile": "0.3.x",
        "winston": "2.1.x"
    },
    "description": "A beautiful command-line prompt for node.js",
    "devDependencies": {
        "vows": "0.7.0"
    },
    "directories": {},
    "dist": {
        "shasum": "8e57123c396ab988897fb327fd3aedc3e735e4fe",
        "tarball": "https://registry.npmjs.org/prompt/-/prompt-1.0.0.tgz"
    },
    "engines": {
        "node": ">= 0.6.6"
    },
    "gitHead": "11f2a2b5123a55c5edd9f11e07f4190e6cf61907",
    "homepage": "https://github.com/flatiron/prompt#readme",
    "license": "MIT",
    "main": "./lib/prompt",
    "maintainers": [
        {
            "name": "indexzero",
            "email": "charlie.robbins@gmail.com"
        },
        {
            "name": "fedor.indutny",
            "email": "fedor.indutny@gmail.com"
        },
        {
            "name": "jcrugzz",
            "email": "jcrugzz@gmail.com"
        }
    ],
    "name": "prompt",
    "optionalDependencies": {},
    "readme": "ERROR: No README data found!",
    "repository": {
        "type": "git",
        "url": "git+ssh://git@github.com/flatiron/prompt.git"
    },
    "scripts": {
        "test": "vows test/prompt-test.js --spec",
        "test-all": "vows --spec"
    },
    "version": "1.0.0"
}
```



# <a name="apidoc.tableOfContents"></a>[table of contents](#apidoc.tableOfContents)

#### [module prompt](#apidoc.module.prompt)
1.  boolean <span class="apidocSignatureSpan">prompt.</span>allowEmpty
1.  boolean <span class="apidocSignatureSpan">prompt.</span>colors
1.  boolean <span class="apidocSignatureSpan">prompt.</span>paused
1.  boolean <span class="apidocSignatureSpan">prompt.</span>started
1.  boolean <span class="apidocSignatureSpan">prompt.</span>stopped
1.  [function <span class="apidocSignatureSpan">prompt.</span>_performValidation (name, prop, against, schema, line, callback)](#apidoc.element.prompt._performValidation)
1.  [function <span class="apidocSignatureSpan">prompt.</span>_remember (property, value)](#apidoc.element.prompt._remember)
1.  [function <span class="apidocSignatureSpan">prompt.</span>addProperties (obj, properties, callback)](#apidoc.element.prompt.addProperties)
1.  [function <span class="apidocSignatureSpan">prompt.</span>confirm ()](#apidoc.element.prompt.confirm)
1.  [function <span class="apidocSignatureSpan">prompt.</span>get (schema, callback)](#apidoc.element.prompt.get)
1.  [function <span class="apidocSignatureSpan">prompt.</span>getInput (prop, callback)](#apidoc.element.prompt.getInput)
1.  [function <span class="apidocSignatureSpan">prompt.</span>history (search)](#apidoc.element.prompt.history)
1.  [function <span class="apidocSignatureSpan">prompt.</span>pause ()](#apidoc.element.prompt.pause)
1.  [function <span class="apidocSignatureSpan">prompt.</span>resume ()](#apidoc.element.prompt.resume)
1.  [function <span class="apidocSignatureSpan">prompt.</span>start (options)](#apidoc.element.prompt.start)
1.  [function <span class="apidocSignatureSpan">prompt.</span>stop ()](#apidoc.element.prompt.stop)
1.  object <span class="apidocSignatureSpan">prompt.</span>logger
1.  object <span class="apidocSignatureSpan">prompt.</span>properties
1.  string <span class="apidocSignatureSpan">prompt.</span>delimiter
1.  string <span class="apidocSignatureSpan">prompt.</span>message

#### [module prompt.logger](#apidoc.module.prompt.logger)
1.  boolean <span class="apidocSignatureSpan">prompt.logger.</span>emitErrs
1.  boolean <span class="apidocSignatureSpan">prompt.logger.</span>exitOnError
1.  boolean <span class="apidocSignatureSpan">prompt.logger.</span>padLevels
1.  boolean <span class="apidocSignatureSpan">prompt.logger.</span>stripColors
1.  [function <span class="apidocSignatureSpan">prompt.logger.</span>data (msg)](#apidoc.element.prompt.logger.data)
1.  [function <span class="apidocSignatureSpan">prompt.logger.</span>debug (msg)](#apidoc.element.prompt.logger.debug)
1.  [function <span class="apidocSignatureSpan">prompt.logger.</span>error (msg)](#apidoc.element.prompt.logger.error)
1.  [function <span class="apidocSignatureSpan">prompt.logger.</span>help (msg)](#apidoc.element.prompt.logger.help)
1.  [function <span class="apidocSignatureSpan">prompt.logger.</span>info (msg)](#apidoc.element.prompt.logger.info)
1.  [function <span class="apidocSignatureSpan">prompt.logger.</span>input (msg)](#apidoc.element.prompt.logger.input)
1.  [function <span class="apidocSignatureSpan">prompt.logger.</span>prompt (msg)](#apidoc.element.prompt.logger.prompt)
1.  [function <span class="apidocSignatureSpan">prompt.logger.</span>silly (msg)](#apidoc.element.prompt.logger.silly)
1.  [function <span class="apidocSignatureSpan">prompt.logger.</span>verbose (msg)](#apidoc.element.prompt.logger.verbose)
1.  [function <span class="apidocSignatureSpan">prompt.logger.</span>warn (msg)](#apidoc.element.prompt.logger.warn)
1.  number <span class="apidocSignatureSpan">prompt.logger.</span>_eventsCount
1.  number <span class="apidocSignatureSpan">prompt.logger.</span>levelLength
1.  object <span class="apidocSignatureSpan">prompt.logger.</span>_events
1.  object <span class="apidocSignatureSpan">prompt.logger.</span>_names
1.  object <span class="apidocSignatureSpan">prompt.logger.</span>domain
1.  object <span class="apidocSignatureSpan">prompt.logger.</span>exceptionHandlers
1.  object <span class="apidocSignatureSpan">prompt.logger.</span>filters
1.  object <span class="apidocSignatureSpan">prompt.logger.</span>levels
1.  object <span class="apidocSignatureSpan">prompt.logger.</span>profilers
1.  object <span class="apidocSignatureSpan">prompt.logger.</span>rewriters
1.  object <span class="apidocSignatureSpan">prompt.logger.</span>transports
1.  string <span class="apidocSignatureSpan">prompt.logger.</span>level



# <a name="apidoc.module.prompt"></a>[module prompt](#apidoc.module.prompt)

#### <a name="apidoc.element.prompt._performValidation"></a>[function <span class="apidocSignatureSpan">prompt.</span>_performValidation (name, prop, against, schema, line, callback)](#apidoc.element.prompt._performValidation)
- description and source-code
```javascript
_performValidation = function (name, prop, against, schema, line, callback) {
  var numericInput, valid, msg;
  try {
    valid = validate(against, schema);
  }
  catch (err) {
    return (line !== -1) ? callback(err) : false;
  }

  if (!valid.valid) {
    if (prop.schema.message) {
      logger.error(prop.schema.message);
    } else {
      msg = line !== -1 ? 'Invalid input for ' : 'Invalid command-line input for ';

      if (prompt.colors) {
        logger.error(msg + name.grey);
      }
      else {
        logger.error(msg + name);
      }
    }

    prompt.emit('invalid', prop, line);
  }

  return valid.valid;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.prompt._remember"></a>[function <span class="apidocSignatureSpan">prompt.</span>_remember (property, value)](#apidoc.element.prompt._remember)
- description and source-code
```javascript
_remember = function (property, value) {
  history.unshift({
    property: property,
    value: value
  });

  //
  // If the length of the 'history' Array
  // has exceeded the specified length to remember,
  // 'prompt.memory', truncate it.
  //
  if (history.length > prompt.memory) {
    history.splice(prompt.memory, history.length - prompt.memory);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.prompt.addProperties"></a>[function <span class="apidocSignatureSpan">prompt.</span>addProperties (obj, properties, callback)](#apidoc.element.prompt.addProperties)
- description and source-code
```javascript
addProperties = function (obj, properties, callback) {
  properties = properties.filter(function (prop) {
    return typeof obj[prop] === 'undefined';
  });

  if (properties.length === 0) {
    return callback(obj);
  }

  prompt.get(properties, function (err, results) {
    if (err) {
      return callback(err);
    }
    else if (!results) {
      return callback(null, obj);
    }

    function putNested (obj, path, value) {
      var last = obj, key;

      while (path.length > 1) {
        key = path.shift();
        if (!last[key]) {
          last[key] = {};
        }

        last = last[key];
      }

      last[path.shift()] = value;
    }

    Object.keys(results).forEach(function (key) {
      putNested(obj, key.split('.'), results[key]);
    });

    callback(null, obj);
  });

  return prompt;
}
```
- example usage
```shell
...
## Features

* prompts the user for input
* supports validation and defaults
* hides passwords

## Usage
Using prompt is relatively straight forward. There are two core methods you should be aware of: 'prompt.get()' and 'prompt.addProperties
()'. Their methods take strings representing property names in addition to objects for complex property validation (and more). There
 are a number of [examples][0] that you should examine for detailed usage.

### Getting Basic Prompt Information
Getting started with 'prompt' is easy. Lets take a look at 'examples/simple-prompt.js':

''' js
var prompt = require('prompt');
...
```

#### <a name="apidoc.element.prompt.confirm"></a>[function <span class="apidocSignatureSpan">prompt.</span>confirm ()](#apidoc.element.prompt.confirm)
- description and source-code
```javascript
confirm = function () {
  var args     = Array.prototype.slice.call(arguments),
      msg      = args.shift(),
      callback = args.pop(),
      opts     = args.shift(),
      vars     = !Array.isArray(msg) ? [msg] : msg,
      RX_Y     = /^[yt]{1}/i,
      RX_YN    = /^[yntf]{1}/i;

  function confirm(target, next) {
    var yes = target.yes || RX_Y,
      options = utile.mixin({
        description: typeof target === 'string' ? target : target.description||'yes/no',
        pattern: target.pattern || RX_YN,
        name: 'confirm',
        message: target.message || 'yes/no'
      }, opts || {});


    prompt.get([options], function (err, result) {
      next(err ? false : yes.test(result[options.name]));
    });
  }

  async.rejectSeries(vars, confirm, function(result) {
    callback(null, result.length===0);
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.prompt.get"></a>[function <span class="apidocSignatureSpan">prompt.</span>get (schema, callback)](#apidoc.element.prompt.get)
- description and source-code
```javascript
get = function (schema, callback) {
  //
  // Transforms a full JSON-schema into an array describing path and sub-schemas.
  // Used for iteration purposes.
  //
  function untangle(schema, path) {
    var results = [];
    path = path || [];

    if (schema.properties) {
      //
      // Iterate over the properties in the schema and use recursion
      // to process sub-properties.
      //
      Object.keys(schema.properties).forEach(function (key) {
        var obj = {};
        obj[key] = schema.properties[key];

        //
        // Concat a sub-untangling to the results.
        //
        results = results.concat(untangle(obj[key], path.concat(key)));
      });

      // Return the results.
      return results;
    }

    //
    // This is a schema "leaf".
    //
    return {
      path: path,
      schema: schema
    };
  }

  //
  // Iterate over the values in the schema, represented as
  // a legit single-property object subschemas. Accepts 'schema'
  // of the forms:
  //
  //    'prop-name'
  //
  //    ['string-name', { path: ['or-well-formed-subschema'], properties: ... }]
  //
  //    { path: ['or-well-formed-subschema'], properties: ... ] }
  //
  //    { properties: { 'schema-with-no-path' } }
  //
  // And transforms them all into
  //
  //    { path: ['path', 'to', 'property'], properties: { path: { to: ...} } }
  //
  function iterate(schema, get, done) {
    var iterator = [],
        result = {};

    if (typeof schema === 'string') {
      //
      // We can iterate over a single string.
      //
      iterator.push({
        path: [schema],
        schema: prompt.properties[schema.toLowerCase()] || {}
      });
    }
    else if (Array.isArray(schema)) {
      //
      // An array of strings and/or single-prop schema and/or no-prop schema.
      //
      iterator = schema.map(function (element) {
        if (typeof element === 'string') {
          return {
            path: [element],
            schema: prompt.properties[element.toLowerCase()] || {}
          };
        }
        else if (element.properties) {
          return {
            path: [Object.keys(element.properties)[0]],
            schema: element.properties[Object.keys(element.properties)[0]]
          };
        }
        else if (element.path && element.schema) {
          return element;
        }
        else {
          return {
            path: [element.name || 'question'],
            schema: element
          };
        }
      });
    }
    else if (schema.properties) {
      //
      // Or a complete schema 'untangle' it for use.
      //
      iterator = untangle(schema);
    }
    else {
      //
      // Or a partial schema and path.
      // TODO: Evaluate need for this option.
      //
      iterator = [{
        schema: schema.schema ? schema.schema : schema,
        path: schema.path || [schema.name || 'question']
      }];
    }

    //
    // Now, iterate and assemble the result.
    //
    async.forEachSeries(iterator, function (branch, next) {
      get(branch, function assembler(err, line) {
        if (err) {
          return next(err);
        }

        function build(path, line) {
          var obj = {};
          if (path.length) {
            obj[path[0]] = build(path.slice(1), line);
            return obj;
          }

          return line;
        }

        function attach(obj, attr) {
          var keys;
          if (typeof attr !== 'object' || attr instanceof Array) {
            return attr;
          }

          keys = Object.keys(attr);
          if (keys.length) {
            if (!obj[keys[0]]) {
              obj[keys[0]] = {};
            }
            obj[keys[0]] = attach(obj[keys[0]], attr[keys[0]]);
          }

          return obj;
        }

        result = attach(result, build(branch.path, line));
        next();
      });
    }, function (err) {
      return err ? done(err) : done(null, result);
    });
  }

  iterate(schema, function get(target, next) {
    prompt.getInput(target, function (err, line) {
      return err ? next(err) : next(null, line);
    });
  }, callback);

  r ...
```
- example usage
```shell
...
## Features

* prompts the user for input
* supports validation and defaults
* hides passwords

## Usage
Using prompt is relatively straight forward. There are two core methods you should be aware of: 'prompt.get()' and 'prompt.addProperties
()'. Their methods take strings representing property names in addition to objects for complex property validation (and more). There
 are a number of [examples][0] that you should examine for detailed usage.

### Getting Basic Prompt Information
Getting started with 'prompt' is easy. Lets take a look at 'examples/simple-prompt.js':

''' js
var prompt = require('prompt');
...
```

#### <a name="apidoc.element.prompt.getInput"></a>[function <span class="apidocSignatureSpan">prompt.</span>getInput (prop, callback)](#apidoc.element.prompt.getInput)
- description and source-code
```javascript
getInput = function (prop, callback) {
  var schema = prop.schema || prop,
      propName = prop.path && prop.path.join(':') || prop,
      storedSchema = prompt.properties[propName.toLowerCase()],
      delim = prompt.delimiter,
      defaultLine,
      against,
      hidden,
      length,
      valid,
      name,
      raw,
      msg;

  //
  // If there is a stored schema for 'propName' in 'propmpt.properties'
  // then use it.
  //
  if (schema instanceof Object && !Object.keys(schema).length &&
    typeof storedSchema !== 'undefined') {
    schema = storedSchema;
  }

  //
  // Build a proper validation schema if we just have a string
  // and no 'storedSchema'.
  //
  if (typeof prop === 'string' && !storedSchema) {
    schema = {};
  }

  schema = convert(schema);
  defaultLine = schema.default;
  name = prop.description || schema.description || propName;
  raw = prompt.colors
    ? [colors.grey(name), colors.grey(delim)]
    : [name, delim];

  if (prompt.message)
    raw.unshift(prompt.message, delim);

  prop = {
    schema: schema,
    path: propName.split(':')
  };

  //
  // If the schema has no 'properties' value then set
  // it to an object containing the current schema
  // for 'propName'.
  //
  if (!schema.properties) {
    schema = (function () {
      var obj = { properties: {} };
      obj.properties[propName] = schema;
      return obj;
    })();
  }

  //
  // Handle overrides here.
  // TODO: Make overrides nestable
  //
  if (prompt.override && prompt.override[propName]) {
    if (prompt._performValidation(name, prop, prompt.override, schema, -1, callback)) {
      return callback(null, prompt.override[propName]);
    }

    delete prompt.override[propName];
  }

  //
  // Check if we should skip this prompt
  //
  if (typeof prop.schema.ask === 'function' &&
    !prop.schema.ask()) {
    return callback(null, prop.schema.default || '');
  }

  var type = (schema.properties && schema.properties[propName] &&
              schema.properties[propName].type || '').toLowerCase().trim(),
      wait = type === 'array';

  if (type === 'array') {
    length = prop.schema.maxItems;
    if (length) {
      msg = (tmp.length + 1).toString() + '/' + length.toString();
    }
    else {
      msg = (tmp.length + 1).toString();
    }
    msg += delim;
    raw.push(prompt.colors ? msg.grey : msg);
  }

  //
  // Calculate the raw length and colorize the prompt
  //
  length = raw.join('').length;
  raw[0] = raw[0];
  msg = raw.join('');

  if (schema.help) {
    schema.help.forEach(function (line) {
      logger.help(line);
    });
  }

  //
  // Emit a "prompting" event
  //
  prompt.emit('prompt', prop);

  //
  // If there is no default line, set it to an empty string
  //
  if(typeof defaultLine === 'undefined') {
    defaultLine = '';
  }

  //
  // set to string for readline ( will not accept Numbers )
  //
  defaultLine = defaultLine.toString();

  //
  // Make the actual read
  //
  read({
    prompt: msg,
    silent: prop.schema && prop.schema.hidden,
    replace: prop.schema && prop.schema.replace,
    default: defaultLine,
    input: stdin,
    output: stdout
  }, function (err, line) {
    if (err && wait === false) {
      return callback(err);
    }

    var against = {},
        numericInput,
        isValid;

    if (line !== '') {

      if (schema.properties[propName]) {
        var type = (schema.properties[propName].type || '').toLowerCase().trim() || undefined;

        //
        // If type is some sort of numeric create a Number object to pass to revalidator
        //
        if (type === 'number' || type === 'integer') {
          line = Number(line);
        }

        //
        // Attempt to parse input as a boolean if the schema expects a boolean
        //
        if (type == 'boolean') {
          if(line.toLowerCase() === "true" || line.toLowerCase() === 't') {
            line = true;
          } else if(line.toLowerCase() === "false" || line.toLowerCase() === 'f') {
            line = false;
          }
        }

        //
        // If the type is an array, wait for the end. Fixes #54 ...
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.prompt.history"></a>[function <span class="apidocSignatureSpan">prompt.</span>history (search)](#apidoc.element.prompt.history)
- description and source-code
```javascript
history = function (search) {
  if (typeof search === 'number') {
    return history[search] || {};
  }

  var names = history.map(function (pair) {
    return typeof pair.property === 'string'
      ? pair.property
      : pair.property.name;
  });

  if (!~names.indexOf(search)) {
    return null;
  }

  return history.filter(function (pair) {
    return typeof pair.property === 'string'
      ? pair.property === search
      : pair.property.name === search;
  })[0];
}
```
- example usage
```shell
...
    proxy: {
      description: 'Proxy url',
    },
    proxyCredentials: {
      description: 'Proxy credentials',
      ask: function() {
        // only ask for proxy credentials if a proxy was set
        return prompt.history('proxy').value > 0;
      }
    }
  }
};

//
// Start the prompt
...
```

#### <a name="apidoc.element.prompt.pause"></a>[function <span class="apidocSignatureSpan">prompt.</span>pause ()](#apidoc.element.prompt.pause)
- description and source-code
```javascript
pause = function () {
  if (!prompt.started || prompt.stopped || prompt.paused) {
    return;
  }

  stdin.pause();
  prompt.emit('pause');
  prompt.paused = true;
  return prompt;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.prompt.resume"></a>[function <span class="apidocSignatureSpan">prompt.</span>resume ()](#apidoc.element.prompt.resume)
- description and source-code
```javascript
resume = function () {
  if (!prompt.started || !prompt.paused) {
    return;
  }

  stdin.resume();
  prompt.emit('resume');
  prompt.paused = false;
  return prompt;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.prompt.start"></a>[function <span class="apidocSignatureSpan">prompt.</span>start (options)](#apidoc.element.prompt.start)
- description and source-code
```javascript
start = function (options) {
  if (prompt.started) {
    return;
  }

  options = options        || {};
  stdin   = options.stdin  || process.stdin;
  stdout  = options.stdout || process.stdout;

  //
  // By default: Remember the last '10' prompt property /
  // answer pairs and don't allow empty responses globally.
  //
  prompt.memory     = options.memory     || 10;
  prompt.allowEmpty = options.allowEmpty || false;
  prompt.message    = options.message    || prompt.message;
  prompt.delimiter  = options.delimiter  || prompt.delimiter;
  prompt.colors     = options.colors     || prompt.colors;

  if (process.platform !== 'win32') {
    // windows falls apart trying to deal with SIGINT
    process.on('SIGINT', function () {
      stdout.write('\n');
      process.exit(1);
    });
  }

  prompt.emit('start');
  prompt.started = true;
  prompt.stopped = false;
  return prompt;
}
```
- example usage
```shell
...

''' js
var prompt = require('prompt');

//
// Start the prompt
//
prompt.start();

//
// Get two properties from the user: username and email
//
prompt.get(['username', 'email'], function (err, result) {
  //
  // Log the results.
...
```

#### <a name="apidoc.element.prompt.stop"></a>[function <span class="apidocSignatureSpan">prompt.</span>stop ()](#apidoc.element.prompt.stop)
- description and source-code
```javascript
stop = function () {
    if (prompt.stopped || !prompt.started) {
        return;
    }

    stdin.destroy();
    prompt.emit('stop');
    prompt.stopped = true;
    prompt.started = false;
    prompt.paused = false;
    return prompt;
}
```
- example usage
```shell
...
}

get_username_prompt(_);

//
// Clean the prompt
//
prompt.stop();
'''

## Installation

''' bash
  $ [sudo] npm install prompt
'''
...
```



# <a name="apidoc.module.prompt.logger"></a>[module prompt.logger](#apidoc.module.prompt.logger)

#### <a name="apidoc.element.prompt.logger.data"></a>[function <span class="apidocSignatureSpan">prompt.logger.</span>data (msg)](#apidoc.element.prompt.logger.data)
- description and source-code
```javascript
data = function (msg) {
  // build argument list (level, msg, ... [string interpolate], [{metadata}], [callback])
  var args = [level].concat(Array.prototype.slice.call(arguments));
  target.log.apply(target, args);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.prompt.logger.debug"></a>[function <span class="apidocSignatureSpan">prompt.logger.</span>debug (msg)](#apidoc.element.prompt.logger.debug)
- description and source-code
```javascript
debug = function (msg) {
  // build argument list (level, msg, ... [string interpolate], [{metadata}], [callback])
  var args = [level].concat(Array.prototype.slice.call(arguments));
  target.log.apply(target, args);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.prompt.logger.error"></a>[function <span class="apidocSignatureSpan">prompt.logger.</span>error (msg)](#apidoc.element.prompt.logger.error)
- description and source-code
```javascript
error = function (msg) {
  // build argument list (level, msg, ... [string interpolate], [{metadata}], [callback])
  var args = [level].concat(Array.prototype.slice.call(arguments));
  target.log.apply(target, args);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.prompt.logger.help"></a>[function <span class="apidocSignatureSpan">prompt.logger.</span>help (msg)](#apidoc.element.prompt.logger.help)
- description and source-code
```javascript
help = function (msg) {
  // build argument list (level, msg, ... [string interpolate], [{metadata}], [callback])
  var args = [level].concat(Array.prototype.slice.call(arguments));
  target.log.apply(target, args);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.prompt.logger.info"></a>[function <span class="apidocSignatureSpan">prompt.logger.</span>info (msg)](#apidoc.element.prompt.logger.info)
- description and source-code
```javascript
info = function (msg) {
  // build argument list (level, msg, ... [string interpolate], [{metadata}], [callback])
  var args = [level].concat(Array.prototype.slice.call(arguments));
  target.log.apply(target, args);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.prompt.logger.input"></a>[function <span class="apidocSignatureSpan">prompt.logger.</span>input (msg)](#apidoc.element.prompt.logger.input)
- description and source-code
```javascript
input = function (msg) {
  // build argument list (level, msg, ... [string interpolate], [{metadata}], [callback])
  var args = [level].concat(Array.prototype.slice.call(arguments));
  target.log.apply(target, args);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.prompt.logger.prompt"></a>[function <span class="apidocSignatureSpan">prompt.logger.</span>prompt (msg)](#apidoc.element.prompt.logger.prompt)
- description and source-code
```javascript
prompt = function (msg) {
  // build argument list (level, msg, ... [string interpolate], [{metadata}], [callback])
  var args = [level].concat(Array.prototype.slice.call(arguments));
  target.log.apply(target, args);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.prompt.logger.silly"></a>[function <span class="apidocSignatureSpan">prompt.logger.</span>silly (msg)](#apidoc.element.prompt.logger.silly)
- description and source-code
```javascript
silly = function (msg) {
  // build argument list (level, msg, ... [string interpolate], [{metadata}], [callback])
  var args = [level].concat(Array.prototype.slice.call(arguments));
  target.log.apply(target, args);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.prompt.logger.verbose"></a>[function <span class="apidocSignatureSpan">prompt.logger.</span>verbose (msg)](#apidoc.element.prompt.logger.verbose)
- description and source-code
```javascript
verbose = function (msg) {
  // build argument list (level, msg, ... [string interpolate], [{metadata}], [callback])
  var args = [level].concat(Array.prototype.slice.call(arguments));
  target.log.apply(target, args);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.prompt.logger.warn"></a>[function <span class="apidocSignatureSpan">prompt.logger.</span>warn (msg)](#apidoc.element.prompt.logger.warn)
- description and source-code
```javascript
warn = function (msg) {
  // build argument list (level, msg, ... [string interpolate], [{metadata}], [callback])
  var args = [level].concat(Array.prototype.slice.call(arguments));
  target.log.apply(target, args);
}
```
- example usage
```shell
n/a
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
