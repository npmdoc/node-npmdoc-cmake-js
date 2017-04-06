# api documentation for  [cmake-js (v3.4.1)](https://github.com/unbornchikken/cmake-js#readme)  [![npm package](https://img.shields.io/npm/v/npmdoc-cmake-js.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-cmake-js) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-cmake-js.svg)](https://travis-ci.org/npmdoc/node-npmdoc-cmake-js)
#### CMake.js - a Node.js/io.js native addon build tool

[![NPM](https://nodei.co/npm/cmake-js.png?downloads=true)](https://www.npmjs.com/package/cmake-js)

[![apidoc](https://npmdoc.github.io/node-npmdoc-cmake-js/build/screenCapture.buildNpmdoc.browser._2Fhome_2Ftravis_2Fbuild_2Fnpmdoc_2Fnode-npmdoc-cmake-js_2Ftmp_2Fbuild_2Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-cmake-js/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-cmake-js/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-cmake-js/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Gábor Mező aka unbornchikken"
    },
    "bin": {
        "cmake-js": "./bin/cmake-js"
    },
    "bugs": {
        "url": "https://github.com/unbornchikken/cmake-js/issues"
    },
    "dependencies": {
        "bluebird": "^2.9.15",
        "debug": "^2.1.3",
        "fs-extra": "1",
        "is-iojs": "^1.0.1",
        "lodash": "^3.6.0",
        "memory-stream": "0",
        "npmconf": "^2.1.2",
        "npmlog": "^1.2.0",
        "request": "^2.54.0",
        "semver": "^5.0.3",
        "splitargs": "0",
        "tar": "^1.0.3",
        "traceur": "0.0.x",
        "unzip": "^0.1.11",
        "url-join": "0",
        "which": "^1.0.9",
        "yargs": "^3.6.0"
    },
    "description": "CMake.js - a Node.js/io.js native addon build tool",
    "devDependencies": {
        "gulp": "*",
        "gulp-sequence": "*",
        "gulp-sourcemaps": "*",
        "gulp-traceur": "*",
        "mocha": "*",
        "nan": "^2.1.0"
    },
    "directories": {},
    "dist": {
        "shasum": "29b57d6e5417b3a395e549b86cb9dc1f3cd97f90",
        "tarball": "https://registry.npmjs.org/cmake-js/-/cmake-js-3.4.1.tgz"
    },
    "engines": {
        "node": ">= 0.10.0"
    },
    "gitHead": "bcefb84c44742c645f39cb914f1714157848ec21",
    "homepage": "https://github.com/unbornchikken/cmake-js#readme",
    "keywords": [
        "native",
        "addon",
        "module",
        "c",
        "c++",
        "bindings",
        "build",
        "cmake",
        "nw.js",
        "electron",
        "boost"
    ],
    "license": "MIT",
    "maintainers": [
        {
            "name": "unbornchikken",
            "email": "gabor.mezo@outlook.com"
        }
    ],
    "name": "cmake-js",
    "optionalDependencies": {},
    "readme": "ERROR: No README data found!",
    "repository": {
        "type": "git",
        "url": "git://github.com/unbornchikken/cmake-js.git"
    },
    "scripts": {
        "compile": "gulp",
        "test": "mocha tests"
    },
    "version": "3.4.1"
}
```



# <a name="apidoc.tableOfContents"></a>[table of contents](#apidoc.tableOfContents)

#### [module cmake-js](#apidoc.module.cmake-js)
1.  [function <span class="apidocSignatureSpan">cmake-js.</span>BuildSystem (options)](#apidoc.element.cmake-js.BuildSystem)
1.  [function <span class="apidocSignatureSpan">cmake-js.</span>CMLog (options)](#apidoc.element.cmake-js.CMLog)
1.  [function <span class="apidocSignatureSpan">cmake-js.</span>CMake (options)](#apidoc.element.cmake-js.CMake)
1.  [function <span class="apidocSignatureSpan">cmake-js.</span>Dist (options)](#apidoc.element.cmake-js.Dist)
1.  [function <span class="apidocSignatureSpan">cmake-js.</span>TargetOptions (options)](#apidoc.element.cmake-js.TargetOptions)
1.  [function <span class="apidocSignatureSpan">cmake-js.</span>Toolset (options)](#apidoc.element.cmake-js.Toolset)
1.  [function <span class="apidocSignatureSpan">cmake-js.</span>downloader (options)](#apidoc.element.cmake-js.downloader)
1.  [function <span class="apidocSignatureSpan">cmake-js.</span>locateNAN ()](#apidoc.element.cmake-js.locateNAN)
1.  object <span class="apidocSignatureSpan">cmake-js.</span>BuildSystem.prototype
1.  object <span class="apidocSignatureSpan">cmake-js.</span>CMLog.prototype
1.  object <span class="apidocSignatureSpan">cmake-js.</span>CMake.prototype
1.  object <span class="apidocSignatureSpan">cmake-js.</span>Dist.prototype
1.  object <span class="apidocSignatureSpan">cmake-js.</span>Toolset.prototype
1.  object <span class="apidocSignatureSpan">cmake-js.</span>downloader.prototype
1.  object <span class="apidocSignatureSpan">cmake-js.</span>environment
1.  object <span class="apidocSignatureSpan">cmake-js.</span>processHelpers

#### [module cmake-js.BuildSystem](#apidoc.module.cmake-js.BuildSystem)
1.  [function <span class="apidocSignatureSpan">cmake-js.</span>BuildSystem (options)](#apidoc.element.cmake-js.BuildSystem.BuildSystem)

#### [module cmake-js.BuildSystem.prototype](#apidoc.module.cmake-js.BuildSystem.prototype)
1.  [function <span class="apidocSignatureSpan">cmake-js.BuildSystem.prototype.</span>_ensureInstalled ()](#apidoc.element.cmake-js.BuildSystem.prototype._ensureInstalled)
1.  [function <span class="apidocSignatureSpan">cmake-js.BuildSystem.prototype.</span>_invokeCMake ()](#apidoc.element.cmake-js.BuildSystem.prototype._invokeCMake)
1.  [function <span class="apidocSignatureSpan">cmake-js.BuildSystem.prototype.</span>_showError (e)](#apidoc.element.cmake-js.BuildSystem.prototype._showError)
1.  [function <span class="apidocSignatureSpan">cmake-js.BuildSystem.prototype.</span>build ()](#apidoc.element.cmake-js.BuildSystem.prototype.build)
1.  [function <span class="apidocSignatureSpan">cmake-js.BuildSystem.prototype.</span>clean ()](#apidoc.element.cmake-js.BuildSystem.prototype.clean)
1.  [function <span class="apidocSignatureSpan">cmake-js.BuildSystem.prototype.</span>compile ()](#apidoc.element.cmake-js.BuildSystem.prototype.compile)
1.  [function <span class="apidocSignatureSpan">cmake-js.BuildSystem.prototype.</span>configure ()](#apidoc.element.cmake-js.BuildSystem.prototype.configure)
1.  [function <span class="apidocSignatureSpan">cmake-js.BuildSystem.prototype.</span>getBuildCommand ()](#apidoc.element.cmake-js.BuildSystem.prototype.getBuildCommand)
1.  [function <span class="apidocSignatureSpan">cmake-js.BuildSystem.prototype.</span>getCleanCommand ()](#apidoc.element.cmake-js.BuildSystem.prototype.getCleanCommand)
1.  [function <span class="apidocSignatureSpan">cmake-js.BuildSystem.prototype.</span>getConfigureCommand ()](#apidoc.element.cmake-js.BuildSystem.prototype.getConfigureCommand)
1.  [function <span class="apidocSignatureSpan">cmake-js.BuildSystem.prototype.</span>install ()](#apidoc.element.cmake-js.BuildSystem.prototype.install)
1.  [function <span class="apidocSignatureSpan">cmake-js.BuildSystem.prototype.</span>rebuild ()](#apidoc.element.cmake-js.BuildSystem.prototype.rebuild)
1.  [function <span class="apidocSignatureSpan">cmake-js.BuildSystem.prototype.</span>reconfigure ()](#apidoc.element.cmake-js.BuildSystem.prototype.reconfigure)

#### [module cmake-js.CMLog](#apidoc.module.cmake-js.CMLog)
1.  [function <span class="apidocSignatureSpan">cmake-js.</span>CMLog (options)](#apidoc.element.cmake-js.CMLog.CMLog)

#### [module cmake-js.CMLog.prototype](#apidoc.module.cmake-js.CMLog.prototype)
1.  [function <span class="apidocSignatureSpan">cmake-js.CMLog.prototype.</span>error (cat, msg)](#apidoc.element.cmake-js.CMLog.prototype.error)
1.  [function <span class="apidocSignatureSpan">cmake-js.CMLog.prototype.</span>http (cat, msg)](#apidoc.element.cmake-js.CMLog.prototype.http)
1.  [function <span class="apidocSignatureSpan">cmake-js.CMLog.prototype.</span>info (cat, msg)](#apidoc.element.cmake-js.CMLog.prototype.info)
1.  [function <span class="apidocSignatureSpan">cmake-js.CMLog.prototype.</span>silly (cat, msg)](#apidoc.element.cmake-js.CMLog.prototype.silly)
1.  [function <span class="apidocSignatureSpan">cmake-js.CMLog.prototype.</span>verbose (cat, msg)](#apidoc.element.cmake-js.CMLog.prototype.verbose)
1.  [function <span class="apidocSignatureSpan">cmake-js.CMLog.prototype.</span>warn (cat, msg)](#apidoc.element.cmake-js.CMLog.prototype.warn)

#### [module cmake-js.CMake](#apidoc.module.cmake-js.CMake)
1.  [function <span class="apidocSignatureSpan">cmake-js.</span>CMake (options)](#apidoc.element.cmake-js.CMake.CMake)
1.  [function <span class="apidocSignatureSpan">cmake-js.CMake.</span>getGenerators ()](#apidoc.element.cmake-js.CMake.getGenerators)
1.  [function <span class="apidocSignatureSpan">cmake-js.CMake.</span>isAvailable (options)](#apidoc.element.cmake-js.CMake.isAvailable)

#### [module cmake-js.CMake.prototype](#apidoc.module.cmake-js.CMake.prototype)
1.  [function <span class="apidocSignatureSpan">cmake-js.CMake.prototype.</span>_run (command)](#apidoc.element.cmake-js.CMake.prototype._run)
1.  [function <span class="apidocSignatureSpan">cmake-js.CMake.prototype.</span>build ()](#apidoc.element.cmake-js.CMake.prototype.build)
1.  [function <span class="apidocSignatureSpan">cmake-js.CMake.prototype.</span>clean ()](#apidoc.element.cmake-js.CMake.prototype.clean)
1.  [function <span class="apidocSignatureSpan">cmake-js.CMake.prototype.</span>compile ()](#apidoc.element.cmake-js.CMake.prototype.compile)
1.  [function <span class="apidocSignatureSpan">cmake-js.CMake.prototype.</span>configure ()](#apidoc.element.cmake-js.CMake.prototype.configure)
1.  [function <span class="apidocSignatureSpan">cmake-js.CMake.prototype.</span>ensureConfigured ()](#apidoc.element.cmake-js.CMake.prototype.ensureConfigured)
1.  [function <span class="apidocSignatureSpan">cmake-js.CMake.prototype.</span>getBuildCommand ()](#apidoc.element.cmake-js.CMake.prototype.getBuildCommand)
1.  [function <span class="apidocSignatureSpan">cmake-js.CMake.prototype.</span>getCleanCommand ()](#apidoc.element.cmake-js.CMake.prototype.getCleanCommand)
1.  [function <span class="apidocSignatureSpan">cmake-js.CMake.prototype.</span>getConfigureCommand ()](#apidoc.element.cmake-js.CMake.prototype.getConfigureCommand)
1.  [function <span class="apidocSignatureSpan">cmake-js.CMake.prototype.</span>getGenerators ()](#apidoc.element.cmake-js.CMake.prototype.getGenerators)
1.  [function <span class="apidocSignatureSpan">cmake-js.CMake.prototype.</span>rebuild ()](#apidoc.element.cmake-js.CMake.prototype.rebuild)
1.  [function <span class="apidocSignatureSpan">cmake-js.CMake.prototype.</span>reconfigure ()](#apidoc.element.cmake-js.CMake.prototype.reconfigure)
1.  [function <span class="apidocSignatureSpan">cmake-js.CMake.prototype.</span>verifyIfAvailable ()](#apidoc.element.cmake-js.CMake.prototype.verifyIfAvailable)

#### [module cmake-js.Dist](#apidoc.module.cmake-js.Dist)
1.  [function <span class="apidocSignatureSpan">cmake-js.</span>Dist (options)](#apidoc.element.cmake-js.Dist.Dist)

#### [module cmake-js.Dist.prototype](#apidoc.module.cmake-js.Dist.prototype)
1.  [function <span class="apidocSignatureSpan">cmake-js.Dist.prototype.</span>_downloadLibs ()](#apidoc.element.cmake-js.Dist.prototype._downloadLibs)
1.  [function <span class="apidocSignatureSpan">cmake-js.Dist.prototype.</span>_downloadShaSums ()](#apidoc.element.cmake-js.Dist.prototype._downloadShaSums)
1.  [function <span class="apidocSignatureSpan">cmake-js.Dist.prototype.</span>_downloadTar ()](#apidoc.element.cmake-js.Dist.prototype._downloadTar)
1.  [function <span class="apidocSignatureSpan">cmake-js.Dist.prototype.</span>download ()](#apidoc.element.cmake-js.Dist.prototype.download)
1.  [function <span class="apidocSignatureSpan">cmake-js.Dist.prototype.</span>ensureDownloaded ()](#apidoc.element.cmake-js.Dist.prototype.ensureDownloaded)

#### [module cmake-js.Toolset](#apidoc.module.cmake-js.Toolset)
1.  [function <span class="apidocSignatureSpan">cmake-js.</span>Toolset (options)](#apidoc.element.cmake-js.Toolset.Toolset)

#### [module cmake-js.Toolset.prototype](#apidoc.module.cmake-js.Toolset.prototype)
1.  [function <span class="apidocSignatureSpan">cmake-js.Toolset.prototype.</span>_getTopSupportedVisualStudioGenerator ()](#apidoc.element.cmake-js.Toolset.prototype._getTopSupportedVisualStudioGenerator)
1.  [function <span class="apidocSignatureSpan">cmake-js.Toolset.prototype.</span>_setupGNUStd (install)](#apidoc.element.cmake-js.Toolset.prototype._setupGNUStd)
1.  [function <span class="apidocSignatureSpan">cmake-js.Toolset.prototype.</span>initialize ()](#apidoc.element.cmake-js.Toolset.prototype.initialize)
1.  [function <span class="apidocSignatureSpan">cmake-js.Toolset.prototype.</span>initializePosix (install)](#apidoc.element.cmake-js.Toolset.prototype.initializePosix)
1.  [function <span class="apidocSignatureSpan">cmake-js.Toolset.prototype.</span>initializeWin ()](#apidoc.element.cmake-js.Toolset.prototype.initializeWin)

#### [module cmake-js.downloader](#apidoc.module.cmake-js.downloader)
1.  [function <span class="apidocSignatureSpan">cmake-js.</span>downloader (options)](#apidoc.element.cmake-js.downloader.downloader)

#### [module cmake-js.downloader.prototype](#apidoc.module.cmake-js.downloader.prototype)
1.  [function <span class="apidocSignatureSpan">cmake-js.downloader.prototype.</span>downloadFile ()](#apidoc.element.cmake-js.downloader.prototype.downloadFile)
1.  [function <span class="apidocSignatureSpan">cmake-js.downloader.prototype.</span>downloadString ()](#apidoc.element.cmake-js.downloader.prototype.downloadString)
1.  [function <span class="apidocSignatureSpan">cmake-js.downloader.prototype.</span>downloadTgz ()](#apidoc.element.cmake-js.downloader.prototype.downloadTgz)
1.  [function <span class="apidocSignatureSpan">cmake-js.downloader.prototype.</span>downloadToStream (url, stream, hash)](#apidoc.element.cmake-js.downloader.prototype.downloadToStream)
1.  [function <span class="apidocSignatureSpan">cmake-js.downloader.prototype.</span>downloadZip ()](#apidoc.element.cmake-js.downloader.prototype.downloadZip)
1.  [function <span class="apidocSignatureSpan">cmake-js.downloader.prototype.</span>testSum (url, sum, options)](#apidoc.element.cmake-js.downloader.prototype.testSum)

#### [module cmake-js.processHelpers](#apidoc.module.cmake-js.processHelpers)
1.  [function <span class="apidocSignatureSpan">cmake-js.processHelpers.</span>exec (command)](#apidoc.element.cmake-js.processHelpers.exec)
1.  [function <span class="apidocSignatureSpan">cmake-js.processHelpers.</span>run (command, options)](#apidoc.element.cmake-js.processHelpers.run)



# <a name="apidoc.module.cmake-js"></a>[module cmake-js](#apidoc.module.cmake-js)

#### <a name="apidoc.element.cmake-js.BuildSystem"></a>[function <span class="apidocSignatureSpan">cmake-js.</span>BuildSystem (options)](#apidoc.element.cmake-js.BuildSystem)
- description and source-code
```javascript
function BuildSystem(options) {
    this.options = options || {};
    this.options.directory = path.resolve(this.options.directory || process.cwd());
    this.log = new CMLog(this.options);
    let appConfig = appCMakeJSConfig(this.options.directory, this.log);
    if (_.isPlainObject(appConfig)) {
        if (_.keys(appConfig).length) {
            this.log.verbose("CFG", "Applying CMake.js config from root package.json:");
            this.log.verbose("CFG", JSON.stringify(appConfig));
            // Applying applications's config, if there is no explicit runtime related options specified
            this.options.runtime = this.options.runtime || appConfig.runtime;
            this.options.runtimeVersion = this.options.runtimeVersion || appConfig.runtimeVersion;
            this.options.arch = this.options.arch || appConfig.arch;
        }
    }
    this.log.verbose("CFG", "Build system options:");
    this.log.verbose("CFG", JSON.stringify(this.options));
    this.cmake = new CMake(this.options);
    this.dist = new Dist(this.options);
    this.toolset = new Toolset(this.options);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cmake-js.CMLog"></a>[function <span class="apidocSignatureSpan">cmake-js.</span>CMLog (options)](#apidoc.element.cmake-js.CMLog)
- description and source-code
```javascript
function CMLog(options) {
    this.options = options || {};
    this.debug = require("debug")(this.options.logName || "cmake-js");
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cmake-js.CMake"></a>[function <span class="apidocSignatureSpan">cmake-js.</span>CMake (options)](#apidoc.element.cmake-js.CMake)
- description and source-code
```javascript
function CMake(options) {
    this.options = options || {};
    this.log = new CMLog(this.options);
    this.dist = new Dist(this.options);
    this.projectRoot = path.resolve(this.options.directory || process.cwd());
    this.workDir = this.options.out || path.join(this.projectRoot, "build");
    this.config = this.options.debug ? "Debug" : "Release";
    this.buildDir = path.join(this.workDir, this.config);
    this._isAvailable = null;
    this.targetOptions = new TargetOptions(this.options);
    this.toolset = new Toolset(this.options);
    this.cMakeOptions = this.options.cMakeOptions || {};
    this.silent = !!options.silent;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cmake-js.Dist"></a>[function <span class="apidocSignatureSpan">cmake-js.</span>Dist (options)](#apidoc.element.cmake-js.Dist)
- description and source-code
```javascript
function Dist(options) {
    this.options = options || {};
    this.log = new CMLog(this.options);
    this.targetOptions = new TargetOptions(this.options);
    this.downloader = new Downloader(this.options);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cmake-js.TargetOptions"></a>[function <span class="apidocSignatureSpan">cmake-js.</span>TargetOptions (options)](#apidoc.element.cmake-js.TargetOptions)
- description and source-code
```javascript
function TargetOptions(options) {
    this.options = options || {};
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cmake-js.Toolset"></a>[function <span class="apidocSignatureSpan">cmake-js.</span>Toolset (options)](#apidoc.element.cmake-js.Toolset)
- description and source-code
```javascript
function Toolset(options) {
    this.options = options || {};
    this.targetOptions = new TargetOptions(this.options);
    this.generator = options.generator;
    this.cCompilerPath = null;
    this.cppCompilerPath = null;
    this.compilerFlags = [];
    this.linkerFlags = [];
    this.makePath = null;
    this.log = new CMLog(this.options);
    this._initialized = false;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cmake-js.downloader"></a>[function <span class="apidocSignatureSpan">cmake-js.</span>downloader (options)](#apidoc.element.cmake-js.downloader)
- description and source-code
```javascript
function Downloader(options) {
    this.options = options || {};
    this.log = new CMLog(this.options);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cmake-js.locateNAN"></a>[function <span class="apidocSignatureSpan">cmake-js.</span>locateNAN ()](#apidoc.element.cmake-js.locateNAN)
- description and source-code
```javascript
locateNAN = function () {
    var generator = generatorFunction.apply(this, arguments);
    var spawn = new PromiseSpawn$(undefined, undefined, yieldHandler,
                                  stack);
    spawn._generator = generator;
    spawn._next(undefined);
    return spawn.promise();
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.cmake-js.BuildSystem"></a>[module cmake-js.BuildSystem](#apidoc.module.cmake-js.BuildSystem)

#### <a name="apidoc.element.cmake-js.BuildSystem.BuildSystem"></a>[function <span class="apidocSignatureSpan">cmake-js.</span>BuildSystem (options)](#apidoc.element.cmake-js.BuildSystem.BuildSystem)
- description and source-code
```javascript
function BuildSystem(options) {
    this.options = options || {};
    this.options.directory = path.resolve(this.options.directory || process.cwd());
    this.log = new CMLog(this.options);
    let appConfig = appCMakeJSConfig(this.options.directory, this.log);
    if (_.isPlainObject(appConfig)) {
        if (_.keys(appConfig).length) {
            this.log.verbose("CFG", "Applying CMake.js config from root package.json:");
            this.log.verbose("CFG", JSON.stringify(appConfig));
            // Applying applications's config, if there is no explicit runtime related options specified
            this.options.runtime = this.options.runtime || appConfig.runtime;
            this.options.runtimeVersion = this.options.runtimeVersion || appConfig.runtimeVersion;
            this.options.arch = this.options.arch || appConfig.arch;
        }
    }
    this.log.verbose("CFG", "Build system options:");
    this.log.verbose("CFG", JSON.stringify(this.options));
    this.cmake = new CMake(this.options);
    this.dist = new Dist(this.options);
    this.toolset = new Toolset(this.options);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.cmake-js.BuildSystem.prototype"></a>[module cmake-js.BuildSystem.prototype](#apidoc.module.cmake-js.BuildSystem.prototype)

#### <a name="apidoc.element.cmake-js.BuildSystem.prototype._ensureInstalled"></a>[function <span class="apidocSignatureSpan">cmake-js.BuildSystem.prototype.</span>_ensureInstalled ()](#apidoc.element.cmake-js.BuildSystem.prototype._ensureInstalled)
- description and source-code
```javascript
_ensureInstalled = function () {
    var generator = generatorFunction.apply(this, arguments);
    var spawn = new PromiseSpawn$(undefined, undefined, yieldHandler,
                                  stack);
    spawn._generator = generator;
    spawn._next(undefined);
    return spawn.promise();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cmake-js.BuildSystem.prototype._invokeCMake"></a>[function <span class="apidocSignatureSpan">cmake-js.BuildSystem.prototype.</span>_invokeCMake ()](#apidoc.element.cmake-js.BuildSystem.prototype._invokeCMake)
- description and source-code
```javascript
_invokeCMake = function () {
    var generator = generatorFunction.apply(this, arguments);
    var spawn = new PromiseSpawn$(undefined, undefined, yieldHandler,
                                  stack);
    spawn._generator = generator;
    spawn._next(undefined);
    return spawn.promise();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cmake-js.BuildSystem.prototype._showError"></a>[function <span class="apidocSignatureSpan">cmake-js.BuildSystem.prototype.</span>_showError (e)](#apidoc.element.cmake-js.BuildSystem.prototype._showError)
- description and source-code
```javascript
_showError = function (e) {
    if (this.log.level === "verbose" || this.log.level === "silly") {
        this.log.error("OMG", e.stack);
    }
    else {
        this.log.error("OMG", e.message);
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cmake-js.BuildSystem.prototype.build"></a>[function <span class="apidocSignatureSpan">cmake-js.BuildSystem.prototype.</span>build ()](#apidoc.element.cmake-js.BuildSystem.prototype.build)
- description and source-code
```javascript
build = function () {
    return this._invokeCMake("build");
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cmake-js.BuildSystem.prototype.clean"></a>[function <span class="apidocSignatureSpan">cmake-js.BuildSystem.prototype.</span>clean ()](#apidoc.element.cmake-js.BuildSystem.prototype.clean)
- description and source-code
```javascript
clean = function () {
    return this._invokeCMake("clean");
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cmake-js.BuildSystem.prototype.compile"></a>[function <span class="apidocSignatureSpan">cmake-js.BuildSystem.prototype.</span>compile ()](#apidoc.element.cmake-js.BuildSystem.prototype.compile)
- description and source-code
```javascript
compile = function () {
    return this._invokeCMake("compile");
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cmake-js.BuildSystem.prototype.configure"></a>[function <span class="apidocSignatureSpan">cmake-js.BuildSystem.prototype.</span>configure ()](#apidoc.element.cmake-js.BuildSystem.prototype.configure)
- description and source-code
```javascript
configure = function () {
    return this._invokeCMake("configure");
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cmake-js.BuildSystem.prototype.getBuildCommand"></a>[function <span class="apidocSignatureSpan">cmake-js.BuildSystem.prototype.</span>getBuildCommand ()](#apidoc.element.cmake-js.BuildSystem.prototype.getBuildCommand)
- description and source-code
```javascript
getBuildCommand = function () {
    return this._invokeCMake("getBuildCommand");
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cmake-js.BuildSystem.prototype.getCleanCommand"></a>[function <span class="apidocSignatureSpan">cmake-js.BuildSystem.prototype.</span>getCleanCommand ()](#apidoc.element.cmake-js.BuildSystem.prototype.getCleanCommand)
- description and source-code
```javascript
getCleanCommand = function () {
    return this._invokeCMake("getCleanCommand");
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cmake-js.BuildSystem.prototype.getConfigureCommand"></a>[function <span class="apidocSignatureSpan">cmake-js.BuildSystem.prototype.</span>getConfigureCommand ()](#apidoc.element.cmake-js.BuildSystem.prototype.getConfigureCommand)
- description and source-code
```javascript
getConfigureCommand = function () {
    return this._invokeCMake("getConfigureCommand");
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cmake-js.BuildSystem.prototype.install"></a>[function <span class="apidocSignatureSpan">cmake-js.BuildSystem.prototype.</span>install ()](#apidoc.element.cmake-js.BuildSystem.prototype.install)
- description and source-code
```javascript
install = function () {
    return this._ensureInstalled();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cmake-js.BuildSystem.prototype.rebuild"></a>[function <span class="apidocSignatureSpan">cmake-js.BuildSystem.prototype.</span>rebuild ()](#apidoc.element.cmake-js.BuildSystem.prototype.rebuild)
- description and source-code
```javascript
rebuild = function () {
    return this._invokeCMake("rebuild");
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cmake-js.BuildSystem.prototype.reconfigure"></a>[function <span class="apidocSignatureSpan">cmake-js.BuildSystem.prototype.</span>reconfigure ()](#apidoc.element.cmake-js.BuildSystem.prototype.reconfigure)
- description and source-code
```javascript
reconfigure = function () {
    return this._invokeCMake("reconfigure");
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.cmake-js.CMLog"></a>[module cmake-js.CMLog](#apidoc.module.cmake-js.CMLog)

#### <a name="apidoc.element.cmake-js.CMLog.CMLog"></a>[function <span class="apidocSignatureSpan">cmake-js.</span>CMLog (options)](#apidoc.element.cmake-js.CMLog.CMLog)
- description and source-code
```javascript
function CMLog(options) {
    this.options = options || {};
    this.debug = require("debug")(this.options.logName || "cmake-js");
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.cmake-js.CMLog.prototype"></a>[module cmake-js.CMLog.prototype](#apidoc.module.cmake-js.CMLog.prototype)

#### <a name="apidoc.element.cmake-js.CMLog.prototype.error"></a>[function <span class="apidocSignatureSpan">cmake-js.CMLog.prototype.</span>error (cat, msg)](#apidoc.element.cmake-js.CMLog.prototype.error)
- description and source-code
```javascript
error = function (cat, msg) {
    if (this.options.noLog) {
        this.debug(cat + ": " + msg);
    }
    else {
        log.error(cat, msg);
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cmake-js.CMLog.prototype.http"></a>[function <span class="apidocSignatureSpan">cmake-js.CMLog.prototype.</span>http (cat, msg)](#apidoc.element.cmake-js.CMLog.prototype.http)
- description and source-code
```javascript
http = function (cat, msg) {
    if (this.options.noLog) {
        this.debug(cat + ": " + msg);
    }
    else {
        log.http(cat, msg);
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cmake-js.CMLog.prototype.info"></a>[function <span class="apidocSignatureSpan">cmake-js.CMLog.prototype.</span>info (cat, msg)](#apidoc.element.cmake-js.CMLog.prototype.info)
- description and source-code
```javascript
info = function (cat, msg) {
    if (this.options.noLog) {
        this.debug(cat + ": " + msg);
    }
    else {
        log.info(cat, msg);
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cmake-js.CMLog.prototype.silly"></a>[function <span class="apidocSignatureSpan">cmake-js.CMLog.prototype.</span>silly (cat, msg)](#apidoc.element.cmake-js.CMLog.prototype.silly)
- description and source-code
```javascript
silly = function (cat, msg) {
    if (this.options.noLog) {
        this.debug(cat + ": " + msg);
    }
    else {
        log.silly(cat, msg);
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cmake-js.CMLog.prototype.verbose"></a>[function <span class="apidocSignatureSpan">cmake-js.CMLog.prototype.</span>verbose (cat, msg)](#apidoc.element.cmake-js.CMLog.prototype.verbose)
- description and source-code
```javascript
verbose = function (cat, msg) {
    if (this.options.noLog) {
        this.debug(cat + ": " + msg);
    }
    else {
        log.verbose(cat, msg);
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cmake-js.CMLog.prototype.warn"></a>[function <span class="apidocSignatureSpan">cmake-js.CMLog.prototype.</span>warn (cat, msg)](#apidoc.element.cmake-js.CMLog.prototype.warn)
- description and source-code
```javascript
warn = function (cat, msg) {
    if (this.options.noLog) {
        this.debug(cat + ": " + msg);
    }
    else {
        log.warn(cat, msg);
    }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.cmake-js.CMake"></a>[module cmake-js.CMake](#apidoc.module.cmake-js.CMake)

#### <a name="apidoc.element.cmake-js.CMake.CMake"></a>[function <span class="apidocSignatureSpan">cmake-js.</span>CMake (options)](#apidoc.element.cmake-js.CMake.CMake)
- description and source-code
```javascript
function CMake(options) {
    this.options = options || {};
    this.log = new CMLog(this.options);
    this.dist = new Dist(this.options);
    this.projectRoot = path.resolve(this.options.directory || process.cwd());
    this.workDir = this.options.out || path.join(this.projectRoot, "build");
    this.config = this.options.debug ? "Debug" : "Release";
    this.buildDir = path.join(this.workDir, this.config);
    this._isAvailable = null;
    this.targetOptions = new TargetOptions(this.options);
    this.toolset = new Toolset(this.options);
    this.cMakeOptions = this.options.cMakeOptions || {};
    this.silent = !!options.silent;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cmake-js.CMake.getGenerators"></a>[function <span class="apidocSignatureSpan">cmake-js.CMake.</span>getGenerators ()](#apidoc.element.cmake-js.CMake.getGenerators)
- description and source-code
```javascript
getGenerators = function () {
    var generator = generatorFunction.apply(this, arguments);
    var spawn = new PromiseSpawn$(undefined, undefined, yieldHandler,
                                  stack);
    spawn._generator = generator;
    spawn._next(undefined);
    return spawn.promise();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cmake-js.CMake.isAvailable"></a>[function <span class="apidocSignatureSpan">cmake-js.CMake.</span>isAvailable (options)](#apidoc.element.cmake-js.CMake.isAvailable)
- description and source-code
```javascript
isAvailable = function (options) {
    options = options || {};
    try {
        if (options.cmakePath) {
            let stat = fs.lstatSync(options.cmakePath);
            return !stat.isDirectory();
        }
        else {
            which.sync("cmake");
            return true;
        }
    }
    catch (e) {
        _.noop(e);
    }
    return false;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.cmake-js.CMake.prototype"></a>[module cmake-js.CMake.prototype](#apidoc.module.cmake-js.CMake.prototype)

#### <a name="apidoc.element.cmake-js.CMake.prototype._run"></a>[function <span class="apidocSignatureSpan">cmake-js.CMake.prototype.</span>_run (command)](#apidoc.element.cmake-js.CMake.prototype._run)
- description and source-code
```javascript
_run = function (command) {
    this.log.info("RUN", command);
    return processHelpers.run(command, {silent: this.silent});
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cmake-js.CMake.prototype.build"></a>[function <span class="apidocSignatureSpan">cmake-js.CMake.prototype.</span>build ()](#apidoc.element.cmake-js.CMake.prototype.build)
- description and source-code
```javascript
build = function () {
    var generator = generatorFunction.apply(this, arguments);
    var spawn = new PromiseSpawn$(undefined, undefined, yieldHandler,
                                  stack);
    spawn._generator = generator;
    spawn._next(undefined);
    return spawn.promise();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cmake-js.CMake.prototype.clean"></a>[function <span class="apidocSignatureSpan">cmake-js.CMake.prototype.</span>clean ()](#apidoc.element.cmake-js.CMake.prototype.clean)
- description and source-code
```javascript
clean = function () {
    this.verifyIfAvailable();

    this.log.info("CMD", "CLEAN");
    return this._run(this.getCleanCommand());
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cmake-js.CMake.prototype.compile"></a>[function <span class="apidocSignatureSpan">cmake-js.CMake.prototype.</span>compile ()](#apidoc.element.cmake-js.CMake.prototype.compile)
- description and source-code
```javascript
compile = function () {
    var generator = generatorFunction.apply(this, arguments);
    var spawn = new PromiseSpawn$(undefined, undefined, yieldHandler,
                                  stack);
    spawn._generator = generator;
    spawn._next(undefined);
    return spawn.promise();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cmake-js.CMake.prototype.configure"></a>[function <span class="apidocSignatureSpan">cmake-js.CMake.prototype.</span>configure ()](#apidoc.element.cmake-js.CMake.prototype.configure)
- description and source-code
```javascript
configure = function () {
    var generator = generatorFunction.apply(this, arguments);
    var spawn = new PromiseSpawn$(undefined, undefined, yieldHandler,
                                  stack);
    spawn._generator = generator;
    spawn._next(undefined);
    return spawn.promise();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cmake-js.CMake.prototype.ensureConfigured"></a>[function <span class="apidocSignatureSpan">cmake-js.CMake.prototype.</span>ensureConfigured ()](#apidoc.element.cmake-js.CMake.prototype.ensureConfigured)
- description and source-code
```javascript
ensureConfigured = function () {
    var generator = generatorFunction.apply(this, arguments);
    var spawn = new PromiseSpawn$(undefined, undefined, yieldHandler,
                                  stack);
    spawn._generator = generator;
    spawn._next(undefined);
    return spawn.promise();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cmake-js.CMake.prototype.getBuildCommand"></a>[function <span class="apidocSignatureSpan">cmake-js.CMake.prototype.</span>getBuildCommand ()](#apidoc.element.cmake-js.CMake.prototype.getBuildCommand)
- description and source-code
```javascript
getBuildCommand = function () {
    return Bluebird.resolve(this.path + " --build \"" + this.workDir + "\" --config " + this.config);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cmake-js.CMake.prototype.getCleanCommand"></a>[function <span class="apidocSignatureSpan">cmake-js.CMake.prototype.</span>getCleanCommand ()](#apidoc.element.cmake-js.CMake.prototype.getCleanCommand)
- description and source-code
```javascript
getCleanCommand = function () {
    return this.path + " -E remove_directory \"" + this.workDir + "\"";
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cmake-js.CMake.prototype.getConfigureCommand"></a>[function <span class="apidocSignatureSpan">cmake-js.CMake.prototype.</span>getConfigureCommand ()](#apidoc.element.cmake-js.CMake.prototype.getConfigureCommand)
- description and source-code
```javascript
getConfigureCommand = function () {
    var generator = generatorFunction.apply(this, arguments);
    var spawn = new PromiseSpawn$(undefined, undefined, yieldHandler,
                                  stack);
    spawn._generator = generator;
    spawn._next(undefined);
    return spawn.promise();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cmake-js.CMake.prototype.getGenerators"></a>[function <span class="apidocSignatureSpan">cmake-js.CMake.prototype.</span>getGenerators ()](#apidoc.element.cmake-js.CMake.prototype.getGenerators)
- description and source-code
```javascript
getGenerators = function () {
    return CMake.getGenerators(this.options);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cmake-js.CMake.prototype.rebuild"></a>[function <span class="apidocSignatureSpan">cmake-js.CMake.prototype.</span>rebuild ()](#apidoc.element.cmake-js.CMake.prototype.rebuild)
- description and source-code
```javascript
rebuild = function () {
    var generator = generatorFunction.apply(this, arguments);
    var spawn = new PromiseSpawn$(undefined, undefined, yieldHandler,
                                  stack);
    spawn._generator = generator;
    spawn._next(undefined);
    return spawn.promise();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cmake-js.CMake.prototype.reconfigure"></a>[function <span class="apidocSignatureSpan">cmake-js.CMake.prototype.</span>reconfigure ()](#apidoc.element.cmake-js.CMake.prototype.reconfigure)
- description and source-code
```javascript
reconfigure = function () {
    var generator = generatorFunction.apply(this, arguments);
    var spawn = new PromiseSpawn$(undefined, undefined, yieldHandler,
                                  stack);
    spawn._generator = generator;
    spawn._next(undefined);
    return spawn.promise();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cmake-js.CMake.prototype.verifyIfAvailable"></a>[function <span class="apidocSignatureSpan">cmake-js.CMake.prototype.</span>verifyIfAvailable ()](#apidoc.element.cmake-js.CMake.prototype.verifyIfAvailable)
- description and source-code
```javascript
verifyIfAvailable = function () {
    if (!this.isAvailable) {
        throw new Error("CMake executable is not found. Please use your system's package manager to install it, or you can get installers
 from there: http://cmake.org.");
    }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.cmake-js.Dist"></a>[module cmake-js.Dist](#apidoc.module.cmake-js.Dist)

#### <a name="apidoc.element.cmake-js.Dist.Dist"></a>[function <span class="apidocSignatureSpan">cmake-js.</span>Dist (options)](#apidoc.element.cmake-js.Dist.Dist)
- description and source-code
```javascript
function Dist(options) {
    this.options = options || {};
    this.log = new CMLog(this.options);
    this.targetOptions = new TargetOptions(this.options);
    this.downloader = new Downloader(this.options);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.cmake-js.Dist.prototype"></a>[module cmake-js.Dist.prototype](#apidoc.module.cmake-js.Dist.prototype)

#### <a name="apidoc.element.cmake-js.Dist.prototype._downloadLibs"></a>[function <span class="apidocSignatureSpan">cmake-js.Dist.prototype.</span>_downloadLibs ()](#apidoc.element.cmake-js.Dist.prototype._downloadLibs)
- description and source-code
```javascript
_downloadLibs = function () {
    var generator = generatorFunction.apply(this, arguments);
    var spawn = new PromiseSpawn$(undefined, undefined, yieldHandler,
                                  stack);
    spawn._generator = generator;
    spawn._next(undefined);
    return spawn.promise();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cmake-js.Dist.prototype._downloadShaSums"></a>[function <span class="apidocSignatureSpan">cmake-js.Dist.prototype.</span>_downloadShaSums ()](#apidoc.element.cmake-js.Dist.prototype._downloadShaSums)
- description and source-code
```javascript
_downloadShaSums = function () {
    var generator = generatorFunction.apply(this, arguments);
    var spawn = new PromiseSpawn$(undefined, undefined, yieldHandler,
                                  stack);
    spawn._generator = generator;
    spawn._next(undefined);
    return spawn.promise();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cmake-js.Dist.prototype._downloadTar"></a>[function <span class="apidocSignatureSpan">cmake-js.Dist.prototype.</span>_downloadTar ()](#apidoc.element.cmake-js.Dist.prototype._downloadTar)
- description and source-code
```javascript
_downloadTar = function () {
    var generator = generatorFunction.apply(this, arguments);
    var spawn = new PromiseSpawn$(undefined, undefined, yieldHandler,
                                  stack);
    spawn._generator = generator;
    spawn._next(undefined);
    return spawn.promise();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cmake-js.Dist.prototype.download"></a>[function <span class="apidocSignatureSpan">cmake-js.Dist.prototype.</span>download ()](#apidoc.element.cmake-js.Dist.prototype.download)
- description and source-code
```javascript
download = function () {
    var generator = generatorFunction.apply(this, arguments);
    var spawn = new PromiseSpawn$(undefined, undefined, yieldHandler,
                                  stack);
    spawn._generator = generator;
    spawn._next(undefined);
    return spawn.promise();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cmake-js.Dist.prototype.ensureDownloaded"></a>[function <span class="apidocSignatureSpan">cmake-js.Dist.prototype.</span>ensureDownloaded ()](#apidoc.element.cmake-js.Dist.prototype.ensureDownloaded)
- description and source-code
```javascript
ensureDownloaded = function () {
    var generator = generatorFunction.apply(this, arguments);
    var spawn = new PromiseSpawn$(undefined, undefined, yieldHandler,
                                  stack);
    spawn._generator = generator;
    spawn._next(undefined);
    return spawn.promise();
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.cmake-js.Toolset"></a>[module cmake-js.Toolset](#apidoc.module.cmake-js.Toolset)

#### <a name="apidoc.element.cmake-js.Toolset.Toolset"></a>[function <span class="apidocSignatureSpan">cmake-js.</span>Toolset (options)](#apidoc.element.cmake-js.Toolset.Toolset)
- description and source-code
```javascript
function Toolset(options) {
    this.options = options || {};
    this.targetOptions = new TargetOptions(this.options);
    this.generator = options.generator;
    this.cCompilerPath = null;
    this.cppCompilerPath = null;
    this.compilerFlags = [];
    this.linkerFlags = [];
    this.makePath = null;
    this.log = new CMLog(this.options);
    this._initialized = false;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.cmake-js.Toolset.prototype"></a>[module cmake-js.Toolset.prototype](#apidoc.module.cmake-js.Toolset.prototype)

#### <a name="apidoc.element.cmake-js.Toolset.prototype._getTopSupportedVisualStudioGenerator"></a>[function <span class="apidocSignatureSpan">cmake-js.Toolset.prototype.</span>_getTopSupportedVisualStudioGenerator ()](#apidoc.element.cmake-js.Toolset.prototype._getTopSupportedVisualStudioGenerator)
- description and source-code
```javascript
_getTopSupportedVisualStudioGenerator = function () {
    var generator = generatorFunction.apply(this, arguments);
    var spawn = new PromiseSpawn$(undefined, undefined, yieldHandler,
                                  stack);
    spawn._generator = generator;
    spawn._next(undefined);
    return spawn.promise();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cmake-js.Toolset.prototype._setupGNUStd"></a>[function <span class="apidocSignatureSpan">cmake-js.Toolset.prototype.</span>_setupGNUStd (install)](#apidoc.element.cmake-js.Toolset.prototype._setupGNUStd)
- description and source-code
```javascript
_setupGNUStd = function (install) {
    if (this.options.std) {
        if (this.options.std !== "c++98") {
            if (install) {
                this.log.info("TOOL", 'Using ${this.options.std} compiler standard.');
            }
            this.compilerFlags.push("-std=" + this.options.std);
        }
    }
    else {
        if (install) {
            this.log.info("TOOL", "Using c++11 compiler standard.");
        }
        this.compilerFlags.push("-std=c++11");
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cmake-js.Toolset.prototype.initialize"></a>[function <span class="apidocSignatureSpan">cmake-js.Toolset.prototype.</span>initialize ()](#apidoc.element.cmake-js.Toolset.prototype.initialize)
- description and source-code
```javascript
initialize = function () {
    var generator = generatorFunction.apply(this, arguments);
    var spawn = new PromiseSpawn$(undefined, undefined, yieldHandler,
                                  stack);
    spawn._generator = generator;
    spawn._next(undefined);
    return spawn.promise();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cmake-js.Toolset.prototype.initializePosix"></a>[function <span class="apidocSignatureSpan">cmake-js.Toolset.prototype.</span>initializePosix (install)](#apidoc.element.cmake-js.Toolset.prototype.initializePosix)
- description and source-code
```javascript
initializePosix = function (install) {
    // 1: Compiler
    if (!environment.isGPPAvailable && !environment.isClangAvailable) {
        if (environment.isOSX) {
            throw new Error("C++ Compiler toolset is not available. Install Xcode Commandline Tools from Apple Dev Center, or install
 Clang with homebrew by invoking: 'brew install llvm --with-clang --with-asan'.");
        }
        else {
            throw new Error("C++ Compiler toolset is not available. Install proper compiler toolset with your package manager, eg
. 'sudo apt-get install g++'.");
        }
    }

    if (this.options.preferClang && environment.isClangAvailable) {
        if (install) {
            this.log.info("TOOL", "Using clang++ compiler, because preferClang option is set, and clang++ is available.");
        }
        this.cppCompilerPath = "clang++";
        this.cCompilerPath = "clang";
    }
    else if (this.options.preferGnu && environment.isGPPAvailable) {
        if (install) {
            this.log.info("TOOL", "Using g++ compiler, because preferGnu option is set, and g++ is available.");
        }
        this.cppCompilerPath = "g++";
        this.cCompilerPath = "gcc";
    }
    // if it's already set because of options...
    if (this.generator) {
        if (install) {
            this.log.info("TOOL", "Using " + this.options.generator + " generator, as specified from commandline.");
        }
    }
    // 2: Generator
    else if (environment.isOSX) {
        if (this.options.preferXcode) {
            if (install) {
                this.log.info("TOOL", "Using Xcode generator, because preferXcode option is set.");
            }
            this.generator = "Xcode";
        }
        else if (this.options.preferMake && environment.isMakeAvailable) {
            if (install) {
                this.log.info("TOOL", "Using Unix Makefiles generator, because preferMake option is set, and make is available.");
            }
            this.generator = "Unix Makefiles";
        }
        else if (environment.isNinjaAvailable) {
            if (install) {
                this.log.info("TOOL", "Using Ninja generator, because ninja is available.");
            }
            this.generator = "Ninja";
        }
        else {
            if (install) {
                this.log.info("TOOL", "Using Unix Makefiles generator.");
            }
            this.generator = "Unix Makefiles";
        }
    }
    else {
        if (this.options.preferMake && environment.isMakeAvailable) {
            if (install) {
                this.log.info("TOOL", "Using Unix Makefiles generator, because preferMake option is set, and make is available.");
            }
            this.generator = "Unix Makefiles";
        }
        else if (environment.isNinjaAvailable) {
            if (install) {
                this.log.info("TOOL", "Using Ninja generator, because ninja is available.");
            }
            this.generator = "Ninja";
        }
        else {
            if (install) {
                this.log.info("TOOL", "Using Unix Makefiles generator.");
            }
            this.generator = "Unix Makefiles";
        }
    }

    // 3: Flags
    this._setupGNUStd(install);

    if (environment.isOSX) {
        if (install) {
            this.log.verbose("TOOL", "Setting default OSX compiler flags.");
        }

        this.compilerFlags.push("-D_DARWIN_USE_64_BIT_INODE=1");
        this.compilerFlags.push("-D_LARGEFILE_SOURCE");
        this.compilerFlags.push("-D_FILE_OFFSET_BITS=64");
        this.compilerFlags.push("-DBUILDING_NODE_EXTENSION");
        this.compilerFlags.push("-w");
        this.linkerFlags.push("-undefined dynamic_lookup");
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cmake-js.Toolset.prototype.initializeWin"></a>[function <span class="apidocSignatureSpan">cmake-js.Toolset.prototype.</span>initializeWin ()](#apidoc.element.cmake-js.Toolset.prototype.initializeWin)
- description and source-code
```javascript
initializeWin = function () {
    var generator = generatorFunction.apply(this, arguments);
    var spawn = new PromiseSpawn$(undefined, undefined, yieldHandler,
                                  stack);
    spawn._generator = generator;
    spawn._next(undefined);
    return spawn.promise();
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.cmake-js.downloader"></a>[module cmake-js.downloader](#apidoc.module.cmake-js.downloader)

#### <a name="apidoc.element.cmake-js.downloader.downloader"></a>[function <span class="apidocSignatureSpan">cmake-js.</span>downloader (options)](#apidoc.element.cmake-js.downloader.downloader)
- description and source-code
```javascript
function Downloader(options) {
    this.options = options || {};
    this.log = new CMLog(this.options);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.cmake-js.downloader.prototype"></a>[module cmake-js.downloader.prototype](#apidoc.module.cmake-js.downloader.prototype)

#### <a name="apidoc.element.cmake-js.downloader.prototype.downloadFile"></a>[function <span class="apidocSignatureSpan">cmake-js.downloader.prototype.</span>downloadFile ()](#apidoc.element.cmake-js.downloader.prototype.downloadFile)
- description and source-code
```javascript
downloadFile = function () {
    var generator = generatorFunction.apply(this, arguments);
    var spawn = new PromiseSpawn$(undefined, undefined, yieldHandler,
                                  stack);
    spawn._generator = generator;
    spawn._next(undefined);
    return spawn.promise();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cmake-js.downloader.prototype.downloadString"></a>[function <span class="apidocSignatureSpan">cmake-js.downloader.prototype.</span>downloadString ()](#apidoc.element.cmake-js.downloader.prototype.downloadString)
- description and source-code
```javascript
downloadString = function () {
    var generator = generatorFunction.apply(this, arguments);
    var spawn = new PromiseSpawn$(undefined, undefined, yieldHandler,
                                  stack);
    spawn._generator = generator;
    spawn._next(undefined);
    return spawn.promise();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cmake-js.downloader.prototype.downloadTgz"></a>[function <span class="apidocSignatureSpan">cmake-js.downloader.prototype.</span>downloadTgz ()](#apidoc.element.cmake-js.downloader.prototype.downloadTgz)
- description and source-code
```javascript
downloadTgz = function () {
    var generator = generatorFunction.apply(this, arguments);
    var spawn = new PromiseSpawn$(undefined, undefined, yieldHandler,
                                  stack);
    spawn._generator = generator;
    spawn._next(undefined);
    return spawn.promise();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cmake-js.downloader.prototype.downloadToStream"></a>[function <span class="apidocSignatureSpan">cmake-js.downloader.prototype.</span>downloadToStream (url, stream, hash)](#apidoc.element.cmake-js.downloader.prototype.downloadToStream)
- description and source-code
```javascript
downloadToStream = function (url, stream, hash) {
    let self = this;
    let shasum = hash ? crypto.createHash(hash) : null;
    return new Bluebird(function (resolve, reject) {
        let length = 0;
        let done = 0;
        let lastPercent = 0;
        request
            .get(url)
            .on("error", function (err) {
                reject(err);
            })
            .on("response", function(data) {
                length = parseInt(data.headers["content-length"]);
                if (!_.isNumber(length)) {
                    length = 0;
                }
            })
            .on("data", function (chunk) {
                if (shasum) {
                    shasum.update(chunk);
                }
                if (length) {
                    done += chunk.length;
                    let percent = done / length * 100;
                    percent = Math.round(percent / 10) * 10 + 10;
                    if (percent > lastPercent) {
                        self.log.verbose("DWNL", "\t" + lastPercent + "%");
                        lastPercent = percent;
                    }
                }
            })
            .pipe(stream);

        stream.once("error", function (err) {
            reject(err);
        });

        stream.once("finish", function () {
            resolve(shasum ? shasum.digest("hex") : undefined);
        });
    });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cmake-js.downloader.prototype.downloadZip"></a>[function <span class="apidocSignatureSpan">cmake-js.downloader.prototype.</span>downloadZip ()](#apidoc.element.cmake-js.downloader.prototype.downloadZip)
- description and source-code
```javascript
downloadZip = function () {
    var generator = generatorFunction.apply(this, arguments);
    var spawn = new PromiseSpawn$(undefined, undefined, yieldHandler,
                                  stack);
    spawn._generator = generator;
    spawn._next(undefined);
    return spawn.promise();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cmake-js.downloader.prototype.testSum"></a>[function <span class="apidocSignatureSpan">cmake-js.downloader.prototype.</span>testSum (url, sum, options)](#apidoc.element.cmake-js.downloader.prototype.testSum)
- description and source-code
```javascript
testSum = function (url, sum, options) {
    if (options.hash && sum && options.sum && options.sum !== sum) {
        throw new Error(options.hash.toUpperCase() + " sum of download '" + url + "' mismatch!");
    }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.cmake-js.processHelpers"></a>[module cmake-js.processHelpers](#apidoc.module.cmake-js.processHelpers)

#### <a name="apidoc.element.cmake-js.processHelpers.exec"></a>[function <span class="apidocSignatureSpan">cmake-js.processHelpers.</span>exec (command)](#apidoc.element.cmake-js.processHelpers.exec)
- description and source-code
```javascript
exec = function (command) {
    return new Bluebird(function (resolve, reject) {
        exec(command, function (err, stdout, stderr) {
            if (err) {
                reject(new Error(err.message + "\n" + (stdout || stderr)));
            }
            else {
               resolve(stdout);
            }
        });
    });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cmake-js.processHelpers.run"></a>[function <span class="apidocSignatureSpan">cmake-js.processHelpers.</span>run (command, options)](#apidoc.element.cmake-js.processHelpers.run)
- description and source-code
```javascript
run = function (command, options) {
    options = _.defaults(options, {silent: false});
    return new Bluebird(function (resolve, reject) {
        let args = splitargs(command);
        let name = args[0];
        args.splice(0, 1);
        let child = spawn(name, args, {stdio: options.silent ? "ignore" : "inherit"});
        let ended = false;
        child.on("error", function (e) {
            if (!ended) {
                reject(e);
                ended = true;
            }
        });
        child.on("exit", function (code, signal) {
            if (!ended) {
                if (code === 0) {
                    resolve();
                }
                else {
                    reject(new Error("Process terminated: " + code || signal));
                }
                ended = true;
            }
        });
    });
}
```
- example usage
```shell
n/a
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
