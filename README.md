# api documentation for  [foreman (v2.0.0)](http://strongloop.github.io/node-foreman/)  [![npm package](https://img.shields.io/npm/v/npmdoc-foreman.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-foreman) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-foreman.svg)](https://travis-ci.org/npmdoc/node-npmdoc-foreman)
#### Node Implementation of Foreman

[![NPM](https://nodei.co/npm/foreman.png?downloads=true)](https://www.npmjs.com/package/foreman)

[![apidoc](https://npmdoc.github.io/node-npmdoc-foreman/build/screenCapture.buildApidoc.browser.%252Fhome%252Ftravis%252Fbuild%252Fnpmdoc%252Fnode-npmdoc-foreman%252Ftmp%252Fbuild%252Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-foreman/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-foreman/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-foreman/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "StrongLoop, Inc."
    },
    "bin": {
        "nf": "nf.js"
    },
    "bugs": {
        "url": "https://github.com/strongloop/node-foreman/issues",
        "email": "callback@strongloop.com"
    },
    "dependencies": {
        "commander": "~2.9.0",
        "http-proxy": "~1.11.1",
        "mustache": "^2.2.1",
        "shell-quote": "~1.4.2"
    },
    "description": "Node Implementation of Foreman",
    "devDependencies": {
        "chai": "~1.9.1",
        "jshint": "^2.6.3",
        "rimraf": "~2.2.8",
        "tap": "^0.7.1"
    },
    "directories": {},
    "dist": {
        "shasum": "00acd20f9dbbe2f79d04697bcca2a77ee00ee031",
        "tarball": "https://registry.npmjs.org/foreman/-/foreman-2.0.0.tgz"
    },
    "engines": {
        "node": ">=0.6.9"
    },
    "files": [
        "forward.js",
        "nf.js",
        "proxy.js",
        "lib/"
    ],
    "gitHead": "008f16259bcbee5b1f39a83d214f42806e0470d0",
    "homepage": "http://strongloop.github.io/node-foreman/",
    "keywords": [
        "foreman",
        "upstart",
        "commandline",
        "env",
        "Procfile"
    ],
    "license": "MIT",
    "maintainers": [
        {
            "name": "bajtos",
            "email": "mbajtoss@gmail.com"
        },
        {
            "name": "chandadharap",
            "email": "chanda_dharap@yahoo.com"
        },
        {
            "name": "ibmcloud-admin",
            "email": "rmg@ca.ibm.com"
        },
        {
            "name": "kraman",
            "email": "kraman@gmail.com"
        },
        {
            "name": "octet",
            "email": "vieuxtech@gmail.com"
        },
        {
            "name": "rfeng",
            "email": "enjoyjava@gmail.com"
        },
        {
            "name": "ritch",
            "email": "skawful@gmail.com"
        },
        {
            "name": "rmg",
            "email": "r.m.graham@gmail.com"
        },
        {
            "name": "setogit",
            "email": "setogit@gmail.com"
        },
        {
            "name": "strongloop",
            "email": "strngops@us.ibm.com"
        },
        {
            "name": "superkhau",
            "email": "superkhau@gmail.com"
        }
    ],
    "name": "foreman",
    "optionalDependencies": {},
    "preferGlobal": true,
    "readme": "ERROR: No README data found!",
    "repository": {
        "type": "git",
        "url": "git+https://github.com/strongloop/node-foreman.git"
    },
    "scripts": {
        "pretest": "jshint .",
        "test": "tap test/*.test.*"
    },
    "version": "2.0.0"
}
```



# <a name="apidoc.tableOfContents"></a>[table of contents](#apidoc.tableOfContents)

#### [module foreman](#apidoc.module.foreman)
1.  object <span class="apidocSignatureSpan">foreman.</span>colors
1.  object <span class="apidocSignatureSpan">foreman.</span>envs
1.  object <span class="apidocSignatureSpan">foreman.</span>forward
1.  object <span class="apidocSignatureSpan">foreman.</span>proc
1.  object <span class="apidocSignatureSpan">foreman.</span>procfile
1.  object <span class="apidocSignatureSpan">foreman.</span>proxy
1.  object <span class="apidocSignatureSpan">foreman.</span>requirements

#### [module foreman.colors](#apidoc.module.foreman.colors)
1.  [function <span class="apidocSignatureSpan">foreman.colors.</span>blue (str)](#apidoc.element.foreman.colors.blue)
1.  [function <span class="apidocSignatureSpan">foreman.colors.</span>bright_blue (str)](#apidoc.element.foreman.colors.bright_blue)
1.  [function <span class="apidocSignatureSpan">foreman.colors.</span>bright_cyan (str)](#apidoc.element.foreman.colors.bright_cyan)
1.  [function <span class="apidocSignatureSpan">foreman.colors.</span>bright_green (str)](#apidoc.element.foreman.colors.bright_green)
1.  [function <span class="apidocSignatureSpan">foreman.colors.</span>bright_magenta (str)](#apidoc.element.foreman.colors.bright_magenta)
1.  [function <span class="apidocSignatureSpan">foreman.colors.</span>bright_red (str)](#apidoc.element.foreman.colors.bright_red)
1.  [function <span class="apidocSignatureSpan">foreman.colors.</span>bright_yellow (str)](#apidoc.element.foreman.colors.bright_yellow)
1.  [function <span class="apidocSignatureSpan">foreman.colors.</span>cyan (str)](#apidoc.element.foreman.colors.cyan)
1.  [function <span class="apidocSignatureSpan">foreman.colors.</span>green (str)](#apidoc.element.foreman.colors.green)
1.  [function <span class="apidocSignatureSpan">foreman.colors.</span>magenta (str)](#apidoc.element.foreman.colors.magenta)
1.  [function <span class="apidocSignatureSpan">foreman.colors.</span>red (str)](#apidoc.element.foreman.colors.red)
1.  [function <span class="apidocSignatureSpan">foreman.colors.</span>yellow (str)](#apidoc.element.foreman.colors.yellow)
1.  number <span class="apidocSignatureSpan">foreman.colors.</span>colors_max
1.  object <span class="apidocSignatureSpan">foreman.</span>colors

#### [module foreman.envs](#apidoc.module.foreman.envs)
1.  [function <span class="apidocSignatureSpan">foreman.envs.</span>dumpEnv (conf)](#apidoc.element.foreman.envs.dumpEnv)
1.  [function <span class="apidocSignatureSpan">foreman.envs.</span>flattenJSON (json)](#apidoc.element.foreman.envs.flattenJSON)
1.  [function <span class="apidocSignatureSpan">foreman.envs.</span>keyValue (data)](#apidoc.element.foreman.envs.keyValue)
1.  [function <span class="apidocSignatureSpan">foreman.envs.</span>loadEnvs (path)](#apidoc.element.foreman.envs.loadEnvs)

#### [module foreman.forward](#apidoc.module.foreman.forward)
1.  [function <span class="apidocSignatureSpan">foreman.forward.</span>startForward (port, hostname, emitter)](#apidoc.element.foreman.forward.startForward)

#### [module foreman.proc](#apidoc.module.foreman.proc)
1.  [function <span class="apidocSignatureSpan">foreman.proc.</span>once (input, envs, callback)](#apidoc.element.foreman.proc.once)
1.  [function <span class="apidocSignatureSpan">foreman.proc.</span>run (key, proc, emitter)](#apidoc.element.foreman.proc.run)
1.  [function <span class="apidocSignatureSpan">foreman.proc.</span>start (procs, requirements, envs, portarg, emitter)](#apidoc.element.foreman.proc.start)

#### [module foreman.procfile](#apidoc.module.foreman.procfile)
1.  [function <span class="apidocSignatureSpan">foreman.procfile.</span>loadProc (filename)](#apidoc.element.foreman.procfile.loadProc)
1.  [function <span class="apidocSignatureSpan">foreman.procfile.</span>procs (procdata)](#apidoc.element.foreman.procfile.procs)

#### [module foreman.proxy](#apidoc.module.foreman.proxy)
1.  [function <span class="apidocSignatureSpan">foreman.proxy.</span>startProxies (reqs, proc, command, emitter, portargs)](#apidoc.element.foreman.proxy.startProxies)

#### [module foreman.requirements](#apidoc.module.foreman.requirements)
1.  [function <span class="apidocSignatureSpan">foreman.requirements.</span>calculatePadding (reqs)](#apidoc.element.foreman.requirements.calculatePadding)
1.  [function <span class="apidocSignatureSpan">foreman.requirements.</span>getreqs (args, proc)](#apidoc.element.foreman.requirements.getreqs)



# <a name="apidoc.module.foreman"></a>[module foreman](#apidoc.module.foreman)



# <a name="apidoc.module.foreman.colors"></a>[module foreman.colors](#apidoc.module.foreman.colors)

#### <a name="apidoc.element.foreman.colors.blue"></a>[function <span class="apidocSignatureSpan">foreman.colors.</span>blue (str)](#apidoc.element.foreman.colors.blue)
- description and source-code
```javascript
blue = function (str) {
  return colors[color] + str + reset;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.foreman.colors.bright_blue"></a>[function <span class="apidocSignatureSpan">foreman.colors.</span>bright_blue (str)](#apidoc.element.foreman.colors.bright_blue)
- description and source-code
```javascript
bright_blue = function (str) {
  return colors[color] + str + reset;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.foreman.colors.bright_cyan"></a>[function <span class="apidocSignatureSpan">foreman.colors.</span>bright_cyan (str)](#apidoc.element.foreman.colors.bright_cyan)
- description and source-code
```javascript
bright_cyan = function (str) {
  return colors[color] + str + reset;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.foreman.colors.bright_green"></a>[function <span class="apidocSignatureSpan">foreman.colors.</span>bright_green (str)](#apidoc.element.foreman.colors.bright_green)
- description and source-code
```javascript
bright_green = function (str) {
  return colors[color] + str + reset;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.foreman.colors.bright_magenta"></a>[function <span class="apidocSignatureSpan">foreman.colors.</span>bright_magenta (str)](#apidoc.element.foreman.colors.bright_magenta)
- description and source-code
```javascript
bright_magenta = function (str) {
  return colors[color] + str + reset;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.foreman.colors.bright_red"></a>[function <span class="apidocSignatureSpan">foreman.colors.</span>bright_red (str)](#apidoc.element.foreman.colors.bright_red)
- description and source-code
```javascript
bright_red = function (str) {
  return colors[color] + str + reset;
}
```
- example usage
```shell
...
  };

  this.Warn = function Warn() {
    logger.warn(colors.yellow('[WARN] ' + this.fmt.apply(null, arguments)));
  };

  this.Error = function Error() {
    logger.error(colors.bright_red('[FAIL] ' + this.fmt.apply(null,arguments)));
  };

}

module.exports = Console;
Console.Console = new Console();
...
```

#### <a name="apidoc.element.foreman.colors.bright_yellow"></a>[function <span class="apidocSignatureSpan">foreman.colors.</span>bright_yellow (str)](#apidoc.element.foreman.colors.bright_yellow)
- description and source-code
```javascript
bright_yellow = function (str) {
  return colors[color] + str + reset;
}
```
- example usage
```shell
...
    return ppath.resolve(__dirname, type, file);
  }
}

function writeout(path) {
  return function(data) {
    if (fs.existsSync(path)) {
      display.Warn(colors.bright_yellow('Replacing: %s'), path);
    }

    fs.writeFileSync(path,data);
    display.Alert('Wrote  :',ppath.normalize(path));
  };
}
...
```

#### <a name="apidoc.element.foreman.colors.cyan"></a>[function <span class="apidocSignatureSpan">foreman.colors.</span>cyan (str)](#apidoc.element.foreman.colors.cyan)
- description and source-code
```javascript
cyan = function (str) {
  return colors[color] + str + reset;
}
```
- example usage
```shell
...
};

this.trim = trim;

// Process Specific Loggers //
this.info = function info(key, proc, string) {
  var stamp = (new Date().toLocaleTimeString()) + " " + key;
  logger.log(proc.color(this.pad(stamp,this.padding)), colors.cyan(string));
};

this.error = function error(key, proc, string) {
  var stamp = (new Date().toLocaleTimeString()) + " " + key;
  logger.error(proc.color(this.pad(stamp,this.padding)), colors.red(string));
};
...
```

#### <a name="apidoc.element.foreman.colors.green"></a>[function <span class="apidocSignatureSpan">foreman.colors.</span>green (str)](#apidoc.element.foreman.colors.green)
- description and source-code
```javascript
green = function (str) {
  return colors[color] + str + reset;
}
```
- example usage
```shell
...

  });
};

// Foreman Loggers //

this.Alert = function Alert() {
  logger.log(colors.green('[OKAY] '+ this.fmt.apply(null, arguments)));
};

this.Done = function Info() {
  logger.log(colors.cyan('[DONE] ' + this.fmt.apply(null, arguments)));
};

this.Warn = function Warn() {
...
```

#### <a name="apidoc.element.foreman.colors.magenta"></a>[function <span class="apidocSignatureSpan">foreman.colors.</span>magenta (str)](#apidoc.element.foreman.colors.magenta)
- description and source-code
```javascript
magenta = function (str) {
  return colors[color] + str + reset;
}
```
- example usage
```shell
...

program.parse(process.argv);

if (!process.argv.slice(2).length) {
  console.log(colors.cyan('   _____                           '));
  console.log(colors.cyan('  |   __|___ ___ ___ _____ ___ ___ '));
  console.log(colors.yellow('  |   __| . |  _| -_|     |   |   |'));
  console.log(colors.magenta('  |__|  |___|_| |___|_|_|_|_^_|_|_|'));
  program.outputHelp();
  process.exit(1);
}
...
```

#### <a name="apidoc.element.foreman.colors.red"></a>[function <span class="apidocSignatureSpan">foreman.colors.</span>red (str)](#apidoc.element.foreman.colors.red)
- description and source-code
```javascript
red = function (str) {
  return colors[color] + str + reset;
}
```
- example usage
```shell
...
  this.info = function info(key, proc, string) {
var stamp = (new Date().toLocaleTimeString()) + " " + key;
logger.log(proc.color(this.pad(stamp,this.padding)), colors.cyan(string));
  };

  this.error = function error(key, proc, string) {
var stamp = (new Date().toLocaleTimeString()) + " " + key;
logger.error(proc.color(this.pad(stamp,this.padding)), colors.red(string));
  };

  this.log = function log(key, proc, string) {
var self = this;

if(self.raw) {
  logger.log(string);
...
```

#### <a name="apidoc.element.foreman.colors.yellow"></a>[function <span class="apidocSignatureSpan">foreman.colors.</span>yellow (str)](#apidoc.element.foreman.colors.yellow)
- description and source-code
```javascript
yellow = function (str) {
  return colors[color] + str + reset;
}
```
- example usage
```shell
...
  };

  this.Done = function Info() {
    logger.log(colors.cyan('[DONE] ' + this.fmt.apply(null, arguments)));
  };

  this.Warn = function Warn() {
    logger.warn(colors.yellow('[WARN] ' + this.fmt.apply(null, arguments)));
  };

  this.Error = function Error() {
    logger.error(colors.bright_red('[FAIL] ' + this.fmt.apply(null,arguments)));
  };

}
...
```



# <a name="apidoc.module.foreman.envs"></a>[module foreman.envs](#apidoc.module.foreman.envs)

#### <a name="apidoc.element.foreman.envs.dumpEnv"></a>[function <span class="apidocSignatureSpan">foreman.envs.</span>dumpEnv (conf)](#apidoc.element.foreman.envs.dumpEnv)
- description and source-code
```javascript
function dumpEnv(conf) {
  var output = [];
  for (var key in conf) {
    output.push(key + '=' + conf[key]);
  }
  return output.sort().join('\n') + '\n';
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.foreman.envs.flattenJSON"></a>[function <span class="apidocSignatureSpan">foreman.envs.</span>flattenJSON (json)](#apidoc.element.foreman.envs.flattenJSON)
- description and source-code
```javascript
function flattenJSON(json) {
  var flattened = {};

  walk(json, function(path, item) {
    flattened[path.join('_').toUpperCase()] = item;
  });

  return flattened;

  function walk(obj, visitor, path) {
    var item;
    path = path || [];
    for (var key in obj) {
      item = obj[key];
      if (typeof item === 'object') {
        walk(item, visitor, path.concat(key));
      } else {
        visitor(path.concat(key), item);
      }
    }
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.foreman.envs.keyValue"></a>[function <span class="apidocSignatureSpan">foreman.envs.</span>keyValue (data)](#apidoc.element.foreman.envs.keyValue)
- description and source-code
```javascript
function keyValue(data) {
  var env = {};

  data
    .toString()
    .replace(/^\s*\#.*$/gm,'')
    .replace(/^\s*$/gm,'')
    .split(/\n/)
    .map(method('trim'))
    .filter(notBlank)
    .forEach(capturePair);

  return env;

  function notBlank(str) {
    return str.length > 2;
  }

  function capturePair(line) {
    var pair = line.split('=');
    var key = pair[0].trim();
    var rawVal = pair.slice(1).join('=').trim();
    env[key] = parseValue(rawVal);
  }

  function parseValue(val) {
    switch (val[0]) {
      case '"': return /^"([^"]*)"/.exec(val)[1];
      case "'": return /^'([^']*)'/.exec(val)[1];
      default : return val.replace(/\s*\#.*$/, '');
    }
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.foreman.envs.loadEnvs"></a>[function <span class="apidocSignatureSpan">foreman.envs.</span>loadEnvs (path)](#apidoc.element.foreman.envs.loadEnvs)
- description and source-code
```javascript
function loadEnvs(path) {
  var envs = path.split(',').map(loadEnvsFile).reduce(util._extend, {});
  var sorted = Object.create(null);
  Object.keys(envs).sort().forEach(function(k) {
    sorted[k] = envs[k];
  });
  return sorted;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.foreman.forward"></a>[module foreman.forward](#apidoc.module.foreman.forward)

#### <a name="apidoc.element.foreman.forward.startForward"></a>[function <span class="apidocSignatureSpan">foreman.forward.</span>startForward (port, hostname, emitter)](#apidoc.element.foreman.forward.startForward)
- description and source-code
```javascript
function startForward(port, hostname, emitter) {
  var proc = prog.fork(__dirname + '/../forward.js', [], {
    env: {
      PROXY_PORT: port,
      PROXY_HOST: hostname || '<ANY>'
    }
  });
  cons.Alert('Forward Proxy Started in Port %d', port);
  if(hostname) {
    cons.Alert('Intercepting requests to %s through forward proxy', hostname);
  } else {
    cons.Alert('Intercepting ALL requests through forward proxy');
  }
  emitter.once('killall', function(signal) {
    cons.Done('Killing Forward Proxy Server on Port %d',port);
    proc.kill(signal);
  });
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.foreman.proc"></a>[module foreman.proc](#apidoc.module.foreman.proc)

#### <a name="apidoc.element.foreman.proc.once"></a>[function <span class="apidocSignatureSpan">foreman.proc.</span>once (input, envs, callback)](#apidoc.element.foreman.proc.once)
- description and source-code
```javascript
function once(input, envs, callback) {
  var file, args;
  var proc = {
    command : input,
    env     : merge(merge({}, process.env), envs)
  };

  if (platform === 'win32') {
    file = process.env.comspec || 'cmd.exe';
    args = ['/s', '/c', proc.command];
  } else {
    file = '/bin/sh';
    args = ['-c', proc.command];
  }

  var child = prog.spawn(file, args, { env: proc.env, stdio: 'inherit' });

  child.on('close', function(code) {
    callback(code);
  });
}
```
- example usage
```shell
...
  });
  cons.Alert('Forward Proxy Started in Port %d', port);
  if(hostname) {
    cons.Alert('Intercepting requests to %s through forward proxy', hostname);
  } else {
    cons.Alert('Intercepting ALL requests through forward proxy');
  }
  emitter.once('killall', function(signal) {
    cons.Done('Killing Forward Proxy Server on Port %d',port);
    proc.kill(signal);
  });
}

module.exports.startForward = startForward;
...
```

#### <a name="apidoc.element.foreman.proc.run"></a>[function <span class="apidocSignatureSpan">foreman.proc.</span>run (key, proc, emitter)](#apidoc.element.foreman.proc.run)
- description and source-code
```javascript
function run(key, proc, emitter) {
  var file, args;
  if (platform === 'win32') {
    file = process.env.comspec || 'cmd.exe';
    args = ['/s', '/c', proc.command];
  } else {
    file = '/bin/sh';
    args = ['-c', proc.command];
  }
  var child = prog.spawn(file, args, { env: proc.env });

  child.stdout.on('data', function(data) {
    cons.log(key, proc, data.toString());
  });

  child.stderr.on('data', function(data) {
    cons.log(key, proc, data.toString());
  });

  child.on('close', function(code) {
    if(code === 0) {
      cons.info(key, proc, "Exited Successfully");
    } else {
      cons.error(key, proc, "Exited with exit code " + code);
    }
  });

  child.on('exit', function(code, signal) {
    emitter.emit('killall', signal);
  });

  emitter.on('killall', function(signal) {
    child.kill(signal);
  });

}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.foreman.proc.start"></a>[function <span class="apidocSignatureSpan">foreman.proc.</span>start (procs, requirements, envs, portarg, emitter)](#apidoc.element.foreman.proc.start)
- description and source-code
```javascript
function start(procs, requirements, envs, portarg, emitter){

  var j = 0;
  var k = 0;
  var port = parseInt(portarg);

  if(port < 1024) {
    return cons.Error('Only Proxies Can Bind to Privileged Ports - '+
                      'Try \'sudo nf start -x %s\'', port);
  }


  for(var key in requirements) {
    var n = parseInt(requirements[key]);

    for(var i = 0; i < n; i++) {

      var color_val = (j + k) % colors_max;

      if (!procs[key]) {
        cons.Warn("Required Key '%s' Does Not Exist in Procfile Definition", key);
        continue;
      }

      var p = {
        command : procs[key],
        color   : colors[color_val],
        env     : merge(merge({}, process.env), envs)
      };

      p.env.PORT = port + j + k * 100;
      p.env.FOREMAN_WORKER_NAME = p.env.FOREMAN_WORKER_NAME || key + "." + (i + 1);

      run(key + "." + (i + 1), p, emitter);

      j++;

    }
    j = 0;
    k++;
  }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.foreman.procfile"></a>[module foreman.procfile](#apidoc.module.foreman.procfile)

#### <a name="apidoc.element.foreman.procfile.loadProc"></a>[function <span class="apidocSignatureSpan">foreman.procfile.</span>loadProc (filename)](#apidoc.element.foreman.procfile.loadProc)
- description and source-code
```javascript
function loadProc(filename) {

  try {
    var data = fs.readFileSync(filename);
    return procs(data);
  } catch(e) {
    cons.Warn(e.message);
    if(fs.existsSync('package.json')) {
      cons.Alert("package.json file found - trying 'npm start'");
      return procs("web: npm start");
    } else {
      cons.Error("No Procfile and no package.json file found in Current Directory - See " + path.basename(process.argv[1]) + " --
help");
      return;
    }
  }

}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.foreman.procfile.procs"></a>[function <span class="apidocSignatureSpan">foreman.procfile.</span>procs (procdata)](#apidoc.element.foreman.procfile.procs)
- description and source-code
```javascript
function procs(procdata){

  var processes = {};

  procdata.toString().split(/\n/).forEach(function(line) {
    if(!line || line[0] === '#') { return; }

    var tuple = /^([A-Za-z0-9_-]+):\s*(.+)$/m.exec(line);

    var prockey = tuple[1].trim();
    var command = tuple[2].trim();

    if(!prockey) {
      throw new Error('Syntax Error in Procfile, Line %d: No Prockey Found');
    }

    if(!command) {
      throw new Error('Syntax Error in Procfile, Line %d: No Command Found');
    }

    processes[prockey] = command;
  });

  return processes;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.foreman.proxy"></a>[module foreman.proxy](#apidoc.module.foreman.proxy)

#### <a name="apidoc.element.foreman.proxy.startProxies"></a>[function <span class="apidocSignatureSpan">foreman.proxy.</span>startProxies (reqs, proc, command, emitter, portargs)](#apidoc.element.foreman.proxy.startProxies)
- description and source-code
```javascript
function startProxies(reqs, proc, command, emitter, portargs) {

  if ('proxy' in command) {

    var localhost = 'localhost';

    var ports = command.proxy.split(',');

    var ssl = {
      cert: '',
      key:  ''
    };
    if ((command.sslKey && !command.sslCert) ||
        (command.sslCert && !command.sslKey)) {
      cons.Warn('SSL key and cert must both be supplied for SSL support');
    }
    if (command.sslKey && command.sslCert) {
      command.sslKey = path.resolve(command.sslKey);
      command.sslCert = path.resolve(command.sslCert);
      if (!fs.existsSync(command.sslKey)) {
        cons.Warn('SSL key (%s) does not exist', command.sslKey);
      }
      else {
        ssl.key = command.sslKey;
      }
      if (!fs.existsSync(command.sslCert)) {
        cons.Warn('SSL cert (%s) does not exist', command.sslCert);
      }
      else {
        ssl.cert = command.sslCert;
      }
    }

    Object.keys(reqs).forEach(function(key, i) {
      f(key, i, ports, proc, reqs, portargs, localhost, emitter, ssl);
    });
  }

}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.foreman.requirements"></a>[module foreman.requirements](#apidoc.module.foreman.requirements)

#### <a name="apidoc.element.foreman.requirements.calculatePadding"></a>[function <span class="apidocSignatureSpan">foreman.requirements.</span>calculatePadding (reqs)](#apidoc.element.foreman.requirements.calculatePadding)
- description and source-code
```javascript
function calculatePadding(reqs) {
  var padding = 0;
  for(var key in reqs){
    var num = reqs[key];
    var len = key.length + num.toString().length;
    if(len > padding) {
      padding = len;
    }
  }
  return padding + 12;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.foreman.requirements.getreqs"></a>[function <span class="apidocSignatureSpan">foreman.requirements.</span>getreqs (args, proc)](#apidoc.element.foreman.requirements.getreqs)
- description and source-code
```javascript
function getreqs(args, proc) {
  var req;
  if(args && args.length > 0) {
    // Run Specific Procs
    req = parseRequirements(args);
  } else {
    // All
    req = {};
    for(var key in proc){
      req[key] = 1;
    }
  }
  return req;
}
```
- example usage
```shell
n/a
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
