# api documentation for  [unzip (v0.1.11)](https://github.com/EvanOxfeld/node-unzip)  [![npm package](https://img.shields.io/npm/v/npmdoc-unzip.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-unzip) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-unzip.svg)](https://travis-ci.org/npmdoc/node-npmdoc-unzip)
#### Unzip cross-platform streaming API compatible with fstream and fs.ReadStream

[![NPM](https://nodei.co/npm/unzip.png?downloads=true)](https://www.npmjs.com/package/unzip)

[![apidoc](https://npmdoc.github.io/node-npmdoc-unzip/build/screenCapture.buildNpmdoc.browser._2Fhome_2Ftravis_2Fbuild_2Fnpmdoc_2Fnode-npmdoc-unzip_2Ftmp_2Fbuild_2Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-unzip/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-unzip/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-unzip/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Evan Oxfeld",
        "email": "eoxfeld@gmail.com"
    },
    "bugs": {
        "url": "https://github.com/EvanOxfeld/node-unzip/issues"
    },
    "dependencies": {
        "binary": ">= 0.3.0 < 1",
        "fstream": ">= 0.1.30 < 1",
        "match-stream": ">= 0.0.2 < 1",
        "pullstream": ">= 0.4.1 < 1",
        "readable-stream": "~1.0.31",
        "setimmediate": ">= 1.0.1 < 2"
    },
    "description": "Unzip cross-platform streaming API compatible with fstream and fs.ReadStream",
    "devDependencies": {
        "dirdiff": ">= 0.0.1 < 1",
        "stream-buffers": ">= 0.2.5 < 1",
        "tap": ">= 0.3.0 < 1",
        "temp": ">= 0.4.0 < 1"
    },
    "directories": {
        "example": "examples",
        "test": "test"
    },
    "dist": {
        "shasum": "89749c63b058d7d90d619f86b98aa1535d3b97f0",
        "tarball": "https://registry.npmjs.org/unzip/-/unzip-0.1.11.tgz"
    },
    "gitHead": "5a62ecbcef6523708bb8b37decaf6e41728ac7fc",
    "homepage": "https://github.com/EvanOxfeld/node-unzip",
    "keywords": [
        "zip",
        "unzip",
        "zlib",
        "uncompress",
        "archive",
        "stream",
        "extract"
    ],
    "license": "MIT",
    "main": "unzip.js",
    "maintainers": [
        {
            "name": "evanoxfeld",
            "email": "eoxfeld@gmail.com"
        },
        {
            "name": "joeferner",
            "email": "joe@fernsroth.com"
        }
    ],
    "name": "unzip",
    "optionalDependencies": {},
    "readme": "ERROR: No README data found!",
    "repository": {
        "type": "git",
        "url": "git+https://github.com/EvanOxfeld/node-unzip.git"
    },
    "scripts": {
        "test": "tap ./test/*.js"
    },
    "version": "0.1.11"
}
```



# <a name="apidoc.tableOfContents"></a>[table of contents](#apidoc.tableOfContents)

#### [module unzip](#apidoc.module.unzip)
1.  [function <span class="apidocSignatureSpan">unzip.</span>Extract (opts)](#apidoc.element.unzip.Extract)
1.  [function <span class="apidocSignatureSpan">unzip.</span>Extract.super_ (options)](#apidoc.element.unzip.Extract.super_)
1.  [function <span class="apidocSignatureSpan">unzip.</span>Parse (opts)](#apidoc.element.unzip.Parse)
1.  [function <span class="apidocSignatureSpan">unzip.</span>Parse.super_ (options)](#apidoc.element.unzip.Parse.super_)
1.  [function <span class="apidocSignatureSpan">unzip.</span>entry ()](#apidoc.element.unzip.entry)
1.  object <span class="apidocSignatureSpan">unzip.</span>Extract.prototype
1.  object <span class="apidocSignatureSpan">unzip.</span>Extract.super_.prototype
1.  object <span class="apidocSignatureSpan">unzip.</span>Parse.prototype
1.  object <span class="apidocSignatureSpan">unzip.</span>Parse.super_.prototype
1.  object <span class="apidocSignatureSpan">unzip.</span>Parse.super_.super_.prototype
1.  object <span class="apidocSignatureSpan">unzip.</span>entry.prototype

#### [module unzip.Extract](#apidoc.module.unzip.Extract)
1.  [function <span class="apidocSignatureSpan">unzip.</span>Extract (opts)](#apidoc.element.unzip.Extract.Extract)
1.  [function <span class="apidocSignatureSpan">unzip.Extract.</span>super_ (options)](#apidoc.element.unzip.Extract.super_)

#### [module unzip.Extract.prototype](#apidoc.module.unzip.Extract.prototype)
1.  [function <span class="apidocSignatureSpan">unzip.Extract.prototype.</span>_write (chunk, encoding, callback)](#apidoc.element.unzip.Extract.prototype._write)

#### [module unzip.Extract.super_](#apidoc.module.unzip.Extract.super_)
1.  [function <span class="apidocSignatureSpan">unzip.Extract.</span>super_ ()](#apidoc.element.unzip.Extract.super_.super_)
1.  [function <span class="apidocSignatureSpan">unzip.Extract.super_.</span>WritableState (options, stream)](#apidoc.element.unzip.Extract.super_.WritableState)

#### [module unzip.Extract.super_.prototype](#apidoc.module.unzip.Extract.super_.prototype)
1.  [function <span class="apidocSignatureSpan">unzip.Extract.super_.prototype.</span>_write (chunk, encoding, cb)](#apidoc.element.unzip.Extract.super_.prototype._write)
1.  [function <span class="apidocSignatureSpan">unzip.Extract.super_.prototype.</span>end (chunk, encoding, cb)](#apidoc.element.unzip.Extract.super_.prototype.end)
1.  [function <span class="apidocSignatureSpan">unzip.Extract.super_.prototype.</span>pipe ()](#apidoc.element.unzip.Extract.super_.prototype.pipe)
1.  [function <span class="apidocSignatureSpan">unzip.Extract.super_.prototype.</span>write (chunk, encoding, cb)](#apidoc.element.unzip.Extract.super_.prototype.write)

#### [module unzip.Parse](#apidoc.module.unzip.Parse)
1.  [function <span class="apidocSignatureSpan">unzip.</span>Parse (opts)](#apidoc.element.unzip.Parse.Parse)
1.  [function <span class="apidocSignatureSpan">unzip.Parse.</span>create (opts)](#apidoc.element.unzip.Parse.create)
1.  [function <span class="apidocSignatureSpan">unzip.Parse.</span>super_ (options)](#apidoc.element.unzip.Parse.super_)

#### [module unzip.Parse.prototype](#apidoc.module.unzip.Parse.prototype)
1.  [function <span class="apidocSignatureSpan">unzip.Parse.prototype.</span>_flush (callback)](#apidoc.element.unzip.Parse.prototype._flush)
1.  [function <span class="apidocSignatureSpan">unzip.Parse.prototype.</span>_processDataDescriptor (entry)](#apidoc.element.unzip.Parse.prototype._processDataDescriptor)
1.  [function <span class="apidocSignatureSpan">unzip.Parse.prototype.</span>_readCentralDirectoryFileHeader ()](#apidoc.element.unzip.Parse.prototype._readCentralDirectoryFileHeader)
1.  [function <span class="apidocSignatureSpan">unzip.Parse.prototype.</span>_readEndOfCentralDirectoryRecord ()](#apidoc.element.unzip.Parse.prototype._readEndOfCentralDirectoryRecord)
1.  [function <span class="apidocSignatureSpan">unzip.Parse.prototype.</span>_readFile ()](#apidoc.element.unzip.Parse.prototype._readFile)
1.  [function <span class="apidocSignatureSpan">unzip.Parse.prototype.</span>_readRecord ()](#apidoc.element.unzip.Parse.prototype._readRecord)
1.  [function <span class="apidocSignatureSpan">unzip.Parse.prototype.</span>_transform (chunk, encoding, callback)](#apidoc.element.unzip.Parse.prototype._transform)
1.  [function <span class="apidocSignatureSpan">unzip.Parse.prototype.</span>addListener (type, listener)](#apidoc.element.unzip.Parse.prototype.addListener)
1.  [function <span class="apidocSignatureSpan">unzip.Parse.prototype.</span>on (type, listener)](#apidoc.element.unzip.Parse.prototype.on)
1.  [function <span class="apidocSignatureSpan">unzip.Parse.prototype.</span>pipe (dest, opts)](#apidoc.element.unzip.Parse.prototype.pipe)

#### [module unzip.Parse.super_](#apidoc.module.unzip.Parse.super_)
1.  [function <span class="apidocSignatureSpan">unzip.Parse.</span>super_ (options)](#apidoc.element.unzip.Parse.super_.super_)

#### [module unzip.Parse.super_.prototype](#apidoc.module.unzip.Parse.super_.prototype)
1.  [function <span class="apidocSignatureSpan">unzip.Parse.super_.prototype.</span>_read (n)](#apidoc.element.unzip.Parse.super_.prototype._read)
1.  [function <span class="apidocSignatureSpan">unzip.Parse.super_.prototype.</span>_transform (chunk, encoding, cb)](#apidoc.element.unzip.Parse.super_.prototype._transform)
1.  [function <span class="apidocSignatureSpan">unzip.Parse.super_.prototype.</span>_write (chunk, encoding, cb)](#apidoc.element.unzip.Parse.super_.prototype._write)
1.  [function <span class="apidocSignatureSpan">unzip.Parse.super_.prototype.</span>push (chunk, encoding)](#apidoc.element.unzip.Parse.super_.prototype.push)

#### [module unzip.Parse.super_.super_.prototype](#apidoc.module.unzip.Parse.super_.super_.prototype)
1.  [function <span class="apidocSignatureSpan">unzip.Parse.super_.super_.prototype.</span>_write (chunk, encoding, cb)](#apidoc.element.unzip.Parse.super_.super_.prototype._write)
1.  [function <span class="apidocSignatureSpan">unzip.Parse.super_.super_.prototype.</span>end (chunk, encoding, cb)](#apidoc.element.unzip.Parse.super_.super_.prototype.end)
1.  [function <span class="apidocSignatureSpan">unzip.Parse.super_.super_.prototype.</span>write (chunk, encoding, cb)](#apidoc.element.unzip.Parse.super_.super_.prototype.write)

#### [module unzip.entry](#apidoc.module.unzip.entry)
1.  [function <span class="apidocSignatureSpan">unzip.</span>entry ()](#apidoc.element.unzip.entry.entry)
1.  [function <span class="apidocSignatureSpan">unzip.entry.</span>super_ (options)](#apidoc.element.unzip.entry.super_)

#### [module unzip.entry.prototype](#apidoc.module.unzip.entry.prototype)
1.  [function <span class="apidocSignatureSpan">unzip.entry.prototype.</span>autodrain ()](#apidoc.element.unzip.entry.prototype.autodrain)



# <a name="apidoc.module.unzip"></a>[module unzip](#apidoc.module.unzip)

#### <a name="apidoc.element.unzip.Extract"></a>[function <span class="apidocSignatureSpan">unzip.</span>Extract (opts)](#apidoc.element.unzip.Extract)
- description and source-code
```javascript
function Extract(opts) {
  var self = this;
  if (!(this instanceof Extract)) {
    return new Extract(opts);
  }

  Writable.apply(this);
  this._opts = opts || { verbose: false };

  this._parser = Parse(this._opts);
  this._parser.on('error', function(err) {
    self.emit('error', err);
  });
  this.on('finish', function() {
    self._parser.end();
  });

  var writer = Writer({
    type: 'Directory',
    path: opts.path
  });
  writer.on('error', function(err) {
    self.emit('error', err);
  });
  writer.on('close', function() {
    self.emit('close')
  });

  this.on('pipe', function(source) {
    if (opts.verbose && source.path) {
      console.log('Archive: ', source.path);
    }
  });

  this._parser.pipe(writer);
}
```
- example usage
```shell
...
$ npm install unzip
'''

## Quick Examples

### Extract to a directory
'''javascript
fs.createReadStream('path/to/archive.zip').pipe(unzip.Extract({ path: 'output/path' }));
'''

Extract emits the 'close' event once the zip's contents have been fully extracted to disk.

### Parse zip file contents

Process each zip file entry or pipe entries to another stream.
...
```

#### <a name="apidoc.element.unzip.Extract.super_"></a>[function <span class="apidocSignatureSpan">unzip.</span>Extract.super_ (options)](#apidoc.element.unzip.Extract.super_)
- description and source-code
```javascript
function Writable(options) {
  var Duplex = require('./_stream_duplex');

  // Writable ctor is applied to Duplexes, though they're not
  // instanceof Writable, they're instanceof Readable.
  if (!(this instanceof Writable) && !(this instanceof Duplex))
    return new Writable(options);

  this._writableState = new WritableState(options, this);

  // legacy.
  this.writable = true;

  Stream.call(this);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.unzip.Parse"></a>[function <span class="apidocSignatureSpan">unzip.</span>Parse (opts)](#apidoc.element.unzip.Parse)
- description and source-code
```javascript
function Parse(opts) {
  var self = this;
  if (!(this instanceof Parse)) {
    return new Parse(opts);
  }

  Transform.call(this, { lowWaterMark: 0 });
  this._opts = opts || { verbose: false };
  this._hasEntryListener = false;

  this._pullStream = new PullStream();
  this._pullStream.on("error", function (e) {
    self.emit('error', e);
  });
  this._pullStream.once("end", function () {
    self._streamEnd = true;
  });
  this._pullStream.once("finish", function () {
    self._streamFinish = true;
  });

  this._readRecord();
}
```
- example usage
```shell
...
Process each zip file entry or pipe entries to another stream.

__Important__: If you do not intend to consume an entry stream's raw data, call autodrain() to dispose of the entry's
contents. Otherwise you risk running out of memory.

'''javascript
fs.createReadStream('path/to/archive.zip')
.pipe(unzip.Parse())
.on('entry', function (entry) {
  var fileName = entry.path;
  var type = entry.type; // 'Directory' or 'File'
  var size = entry.size;
  if (fileName === "this IS the file I'm looking for") {
    entry.pipe(fs.createWriteStream('output/path'));
  } else {
...
```

#### <a name="apidoc.element.unzip.Parse.super_"></a>[function <span class="apidocSignatureSpan">unzip.</span>Parse.super_ (options)](#apidoc.element.unzip.Parse.super_)
- description and source-code
```javascript
function Transform(options) {
  if (!(this instanceof Transform))
    return new Transform(options);

  Duplex.call(this, options);

  var ts = this._transformState = new TransformState(options, this);

  // when the writable side finishes, then flush out anything remaining.
  var stream = this;

  // start out asking for a readable event once data is transformed.
  this._readableState.needReadable = true;

  // we have implemented the _read method, and done the other things
  // that Readable wants before the first _read call, so unset the
  // sync guard flag.
  this._readableState.sync = false;

  this.once('finish', function() {
    if ('function' === typeof this._flush)
      this._flush(function(er) {
        done(stream, er);
      });
    else
      done(stream);
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.unzip.entry"></a>[function <span class="apidocSignatureSpan">unzip.</span>entry ()](#apidoc.element.unzip.entry)
- description and source-code
```javascript
function Entry() {
  PassThrough.call(this);
  this.props = {};
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.unzip.Extract"></a>[module unzip.Extract](#apidoc.module.unzip.Extract)

#### <a name="apidoc.element.unzip.Extract.Extract"></a>[function <span class="apidocSignatureSpan">unzip.</span>Extract (opts)](#apidoc.element.unzip.Extract.Extract)
- description and source-code
```javascript
function Extract(opts) {
  var self = this;
  if (!(this instanceof Extract)) {
    return new Extract(opts);
  }

  Writable.apply(this);
  this._opts = opts || { verbose: false };

  this._parser = Parse(this._opts);
  this._parser.on('error', function(err) {
    self.emit('error', err);
  });
  this.on('finish', function() {
    self._parser.end();
  });

  var writer = Writer({
    type: 'Directory',
    path: opts.path
  });
  writer.on('error', function(err) {
    self.emit('error', err);
  });
  writer.on('close', function() {
    self.emit('close')
  });

  this.on('pipe', function(source) {
    if (opts.verbose && source.path) {
      console.log('Archive: ', source.path);
    }
  });

  this._parser.pipe(writer);
}
```
- example usage
```shell
...
$ npm install unzip
'''

## Quick Examples

### Extract to a directory
'''javascript
fs.createReadStream('path/to/archive.zip').pipe(unzip.Extract({ path: 'output/path' }));
'''

Extract emits the 'close' event once the zip's contents have been fully extracted to disk.

### Parse zip file contents

Process each zip file entry or pipe entries to another stream.
...
```

#### <a name="apidoc.element.unzip.Extract.super_"></a>[function <span class="apidocSignatureSpan">unzip.Extract.</span>super_ (options)](#apidoc.element.unzip.Extract.super_)
- description and source-code
```javascript
function Writable(options) {
  var Duplex = require('./_stream_duplex');

  // Writable ctor is applied to Duplexes, though they're not
  // instanceof Writable, they're instanceof Readable.
  if (!(this instanceof Writable) && !(this instanceof Duplex))
    return new Writable(options);

  this._writableState = new WritableState(options, this);

  // legacy.
  this.writable = true;

  Stream.call(this);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.unzip.Extract.prototype"></a>[module unzip.Extract.prototype](#apidoc.module.unzip.Extract.prototype)

#### <a name="apidoc.element.unzip.Extract.prototype._write"></a>[function <span class="apidocSignatureSpan">unzip.Extract.prototype.</span>_write (chunk, encoding, callback)](#apidoc.element.unzip.Extract.prototype._write)
- description and source-code
```javascript
_write = function (chunk, encoding, callback) {
  if (this._parser.write(chunk)) {
    return callback();
  }

  return this._parser.once('drain', callback);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.unzip.Extract.super_"></a>[module unzip.Extract.super_](#apidoc.module.unzip.Extract.super_)

#### <a name="apidoc.element.unzip.Extract.super_.super_"></a>[function <span class="apidocSignatureSpan">unzip.Extract.</span>super_ ()](#apidoc.element.unzip.Extract.super_.super_)
- description and source-code
```javascript
function Stream() {
  EE.call(this);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.unzip.Extract.super_.WritableState"></a>[function <span class="apidocSignatureSpan">unzip.Extract.super_.</span>WritableState (options, stream)](#apidoc.element.unzip.Extract.super_.WritableState)
- description and source-code
```javascript
function WritableState(options, stream) {
  options = options || {};

  // the point at which write() starts returning false
  // Note: 0 is a valid value, means that we always return false if
  // the entire buffer is not flushed immediately on write()
  var hwm = options.highWaterMark;
  this.highWaterMark = (hwm || hwm === 0) ? hwm : 16 * 1024;

  // object stream flag to indicate whether or not this stream
  // contains buffers or objects.
  this.objectMode = !!options.objectMode;

  // cast to ints.
  this.highWaterMark = ~~this.highWaterMark;

  this.needDrain = false;
  // at the start of calling end()
  this.ending = false;
  // when end() has been called, and returned
  this.ended = false;
  // when 'finish' is emitted
  this.finished = false;

  // should we decode strings into buffers before passing to _write?
  // this is here so that some node-core streams can optimize string
  // handling at a lower level.
  var noDecode = options.decodeStrings === false;
  this.decodeStrings = !noDecode;

  // Crypto is kind of old and crusty.  Historically, its default string
  // encoding is 'binary' so we have to make this configurable.
  // Everything else in the universe uses 'utf8', though.
  this.defaultEncoding = options.defaultEncoding || 'utf8';

  // not an actual buffer we keep track of, but a measurement
  // of how much we're waiting to get pushed to some underlying
  // socket or file.
  this.length = 0;

  // a flag to see when we're in the middle of a write.
  this.writing = false;

  // a flag to be able to tell if the onwrite cb is called immediately,
  // or on a later tick.  We set this to true at first, becuase any
  // actions that shouldn't happen until "later" should generally also
  // not happen before the first write call.
  this.sync = true;

  // a flag to know if we're processing previously buffered items, which
  // may call the _write() callback in the same tick, so that we don't
  // end up in an overlapped onwrite situation.
  this.bufferProcessing = false;

  // the callback that's passed to _write(chunk,cb)
  this.onwrite = function(er) {
    onwrite(stream, er);
  };

  // the callback that the user supplies to write(chunk,encoding,cb)
  this.writecb = null;

  // the amount that is being written when _write is called.
  this.writelen = 0;

  this.buffer = [];

  // True if the error was already emitted and should not be thrown again
  this.errorEmitted = false;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.unzip.Extract.super_.prototype"></a>[module unzip.Extract.super_.prototype](#apidoc.module.unzip.Extract.super_.prototype)

#### <a name="apidoc.element.unzip.Extract.super_.prototype._write"></a>[function <span class="apidocSignatureSpan">unzip.Extract.super_.prototype.</span>_write (chunk, encoding, cb)](#apidoc.element.unzip.Extract.super_.prototype._write)
- description and source-code
```javascript
_write = function (chunk, encoding, cb) {
  cb(new Error('not implemented'));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.unzip.Extract.super_.prototype.end"></a>[function <span class="apidocSignatureSpan">unzip.Extract.super_.prototype.</span>end (chunk, encoding, cb)](#apidoc.element.unzip.Extract.super_.prototype.end)
- description and source-code
```javascript
end = function (chunk, encoding, cb) {
  var state = this._writableState;

  if (typeof chunk === 'function') {
    cb = chunk;
    chunk = null;
    encoding = null;
  } else if (typeof encoding === 'function') {
    cb = encoding;
    encoding = null;
  }

  if (typeof chunk !== 'undefined' && chunk !== null)
    this.write(chunk, encoding);

  // ignore unnecessary end() calls.
  if (!state.ending && !state.finished)
    endWritable(this, state, cb);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.unzip.Extract.super_.prototype.pipe"></a>[function <span class="apidocSignatureSpan">unzip.Extract.super_.prototype.</span>pipe ()](#apidoc.element.unzip.Extract.super_.prototype.pipe)
- description and source-code
```javascript
pipe = function () {
  this.emit('error', new Error('Cannot pipe. Not readable.'));
}
```
- example usage
```shell
...
$ npm install unzip
'''

## Quick Examples

### Extract to a directory
'''javascript
fs.createReadStream('path/to/archive.zip').pipe(unzip.Extract({ path: 'output/path' }));
'''

Extract emits the 'close' event once the zip's contents have been fully extracted to disk.

### Parse zip file contents

Process each zip file entry or pipe entries to another stream.
...
```

#### <a name="apidoc.element.unzip.Extract.super_.prototype.write"></a>[function <span class="apidocSignatureSpan">unzip.Extract.super_.prototype.</span>write (chunk, encoding, cb)](#apidoc.element.unzip.Extract.super_.prototype.write)
- description and source-code
```javascript
write = function (chunk, encoding, cb) {
  var state = this._writableState;
  var ret = false;

  if (typeof encoding === 'function') {
    cb = encoding;
    encoding = null;
  }

  if (Buffer.isBuffer(chunk))
    encoding = 'buffer';
  else if (!encoding)
    encoding = state.defaultEncoding;

  if (typeof cb !== 'function')
    cb = function() {};

  if (state.ended)
    writeAfterEnd(this, state, cb);
  else if (validChunk(this, state, chunk, cb))
    ret = writeOrBuffer(this, state, chunk, encoding, cb);

  return ret;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.unzip.Parse"></a>[module unzip.Parse](#apidoc.module.unzip.Parse)

#### <a name="apidoc.element.unzip.Parse.Parse"></a>[function <span class="apidocSignatureSpan">unzip.</span>Parse (opts)](#apidoc.element.unzip.Parse.Parse)
- description and source-code
```javascript
function Parse(opts) {
  var self = this;
  if (!(this instanceof Parse)) {
    return new Parse(opts);
  }

  Transform.call(this, { lowWaterMark: 0 });
  this._opts = opts || { verbose: false };
  this._hasEntryListener = false;

  this._pullStream = new PullStream();
  this._pullStream.on("error", function (e) {
    self.emit('error', e);
  });
  this._pullStream.once("end", function () {
    self._streamEnd = true;
  });
  this._pullStream.once("finish", function () {
    self._streamFinish = true;
  });

  this._readRecord();
}
```
- example usage
```shell
...
Process each zip file entry or pipe entries to another stream.

__Important__: If you do not intend to consume an entry stream's raw data, call autodrain() to dispose of the entry's
contents. Otherwise you risk running out of memory.

'''javascript
fs.createReadStream('path/to/archive.zip')
.pipe(unzip.Parse())
.on('entry', function (entry) {
  var fileName = entry.path;
  var type = entry.type; // 'Directory' or 'File'
  var size = entry.size;
  if (fileName === "this IS the file I'm looking for") {
    entry.pipe(fs.createWriteStream('output/path'));
  } else {
...
```

#### <a name="apidoc.element.unzip.Parse.create"></a>[function <span class="apidocSignatureSpan">unzip.Parse.</span>create (opts)](#apidoc.element.unzip.Parse.create)
- description and source-code
```javascript
function Parse(opts) {
  var self = this;
  if (!(this instanceof Parse)) {
    return new Parse(opts);
  }

  Transform.call(this, { lowWaterMark: 0 });
  this._opts = opts || { verbose: false };
  this._hasEntryListener = false;

  this._pullStream = new PullStream();
  this._pullStream.on("error", function (e) {
    self.emit('error', e);
  });
  this._pullStream.once("end", function () {
    self._streamEnd = true;
  });
  this._pullStream.once("finish", function () {
    self._streamFinish = true;
  });

  this._readRecord();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.unzip.Parse.super_"></a>[function <span class="apidocSignatureSpan">unzip.Parse.</span>super_ (options)](#apidoc.element.unzip.Parse.super_)
- description and source-code
```javascript
function Transform(options) {
  if (!(this instanceof Transform))
    return new Transform(options);

  Duplex.call(this, options);

  var ts = this._transformState = new TransformState(options, this);

  // when the writable side finishes, then flush out anything remaining.
  var stream = this;

  // start out asking for a readable event once data is transformed.
  this._readableState.needReadable = true;

  // we have implemented the _read method, and done the other things
  // that Readable wants before the first _read call, so unset the
  // sync guard flag.
  this._readableState.sync = false;

  this.once('finish', function() {
    if ('function' === typeof this._flush)
      this._flush(function(er) {
        done(stream, er);
      });
    else
      done(stream);
  });
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.unzip.Parse.prototype"></a>[module unzip.Parse.prototype](#apidoc.module.unzip.Parse.prototype)

#### <a name="apidoc.element.unzip.Parse.prototype._flush"></a>[function <span class="apidocSignatureSpan">unzip.Parse.prototype.</span>_flush (callback)](#apidoc.element.unzip.Parse.prototype._flush)
- description and source-code
```javascript
_flush = function (callback) {
  if (!this._streamEnd || !this._streamFinish) {
    return setImmediate(this._flush.bind(this, callback));
  }

  this.emit('close');
  return callback();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.unzip.Parse.prototype._processDataDescriptor"></a>[function <span class="apidocSignatureSpan">unzip.Parse.prototype.</span>_processDataDescriptor (entry)](#apidoc.element.unzip.Parse.prototype._processDataDescriptor)
- description and source-code
```javascript
_processDataDescriptor = function (entry) {
  var self = this;
  this._pullStream.pull(16, function (err, data) {
    if (err) {
      return self.emit('error', err);
    }

    var vars = binary.parse(data)
      .word32lu('dataDescriptorSignature')
      .word32lu('crc32')
      .word32lu('compressedSize')
      .word32lu('uncompressedSize')
      .vars;

    entry.size = vars.uncompressedSize;
    self._readRecord();
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.unzip.Parse.prototype._readCentralDirectoryFileHeader"></a>[function <span class="apidocSignatureSpan">unzip.Parse.prototype.</span>_readCentralDirectoryFileHeader ()](#apidoc.element.unzip.Parse.prototype._readCentralDirectoryFileHeader)
- description and source-code
```javascript
_readCentralDirectoryFileHeader = function () {
  var self = this;
  this._pullStream.pull(42, function (err, data) {
    if (err) {
      return self.emit('error', err);
    }

    var vars = binary.parse(data)
      .word16lu('versionMadeBy')
      .word16lu('versionsNeededToExtract')
      .word16lu('flags')
      .word16lu('compressionMethod')
      .word16lu('lastModifiedTime')
      .word16lu('lastModifiedDate')
      .word32lu('crc32')
      .word32lu('compressedSize')
      .word32lu('uncompressedSize')
      .word16lu('fileNameLength')
      .word16lu('extraFieldLength')
      .word16lu('fileCommentLength')
      .word16lu('diskNumber')
      .word16lu('internalFileAttributes')
      .word32lu('externalFileAttributes')
      .word32lu('offsetToLocalFileHeader')
      .vars;

    return self._pullStream.pull(vars.fileNameLength, function (err, fileName) {
      if (err) {
        return self.emit('error', err);
      }
      fileName = fileName.toString('utf8');

      self._pullStream.pull(vars.extraFieldLength, function (err, extraField) {
        if (err) {
          return self.emit('error', err);
        }
        self._pullStream.pull(vars.fileCommentLength, function (err, fileComment) {
          if (err) {
            return self.emit('error', err);
          }
          return self._readRecord();
        });
      });
    });
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.unzip.Parse.prototype._readEndOfCentralDirectoryRecord"></a>[function <span class="apidocSignatureSpan">unzip.Parse.prototype.</span>_readEndOfCentralDirectoryRecord ()](#apidoc.element.unzip.Parse.prototype._readEndOfCentralDirectoryRecord)
- description and source-code
```javascript
_readEndOfCentralDirectoryRecord = function () {
  var self = this;
  this._pullStream.pull(18, function (err, data) {
    if (err) {
      return self.emit('error', err);
    }

    var vars = binary.parse(data)
      .word16lu('diskNumber')
      .word16lu('diskStart')
      .word16lu('numberOfRecordsOnDisk')
      .word16lu('numberOfRecords')
      .word32lu('sizeOfCentralDirectory')
      .word32lu('offsetToStartOfCentralDirectory')
      .word16lu('commentLength')
      .vars;

    if (vars.commentLength) {
      setImmediate(function() {
        self._pullStream.pull(vars.commentLength, function (err, comment) {
          if (err) {
            return self.emit('error', err);
          }
          comment = comment.toString('utf8');
          return self._pullStream.end();
        });
      });

    } else {
      self._pullStream.end();
    }
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.unzip.Parse.prototype._readFile"></a>[function <span class="apidocSignatureSpan">unzip.Parse.prototype.</span>_readFile ()](#apidoc.element.unzip.Parse.prototype._readFile)
- description and source-code
```javascript
_readFile = function () {
  var self = this;
  this._pullStream.pull(26, function (err, data) {
    if (err) {
      return self.emit('error', err);
    }

    var vars = binary.parse(data)
      .word16lu('versionsNeededToExtract')
      .word16lu('flags')
      .word16lu('compressionMethod')
      .word16lu('lastModifiedTime')
      .word16lu('lastModifiedDate')
      .word32lu('crc32')
      .word32lu('compressedSize')
      .word32lu('uncompressedSize')
      .word16lu('fileNameLength')
      .word16lu('extraFieldLength')
      .vars;

    return self._pullStream.pull(vars.fileNameLength, function (err, fileName) {
      if (err) {
        return self.emit('error', err);
      }
      fileName = fileName.toString('utf8');
      var entry = new Entry();
      entry.path = fileName;
      entry.props.path = fileName;
      entry.type = (vars.compressedSize === 0 && /[\/\\]$/.test(fileName)) ? 'Directory' : 'File';

      if (self._opts.verbose) {
        if (entry.type === 'Directory') {
          console.log('   creating:', fileName);
        } else if (entry.type === 'File') {
          if (vars.compressionMethod === 0) {
            console.log(' extracting:', fileName);
          } else {
            console.log('  inflating:', fileName);
          }
        }
      }

      var hasEntryListener = self._hasEntryListener;
      if (hasEntryListener) {
        self.emit('entry', entry);
      }

      self._pullStream.pull(vars.extraFieldLength, function (err, extraField) {
        if (err) {
          return self.emit('error', err);
        }
        if (vars.compressionMethod === 0) {
          self._pullStream.pull(vars.compressedSize, function (err, compressedData) {
            if (err) {
              return self.emit('error', err);
            }

            if (hasEntryListener) {
              entry.write(compressedData);
              entry.end();
            }

            return self._readRecord();
          });
        } else {
          var fileSizeKnown = !(vars.flags & 0x08);

          var inflater = zlib.createInflateRaw();
          inflater.on('error', function (err) {
            self.emit('error', err);
          });

          if (fileSizeKnown) {
            entry.size = vars.uncompressedSize;
            if (hasEntryListener) {
              entry.on('finish', self._readRecord.bind(self));
              self._pullStream.pipe(vars.compressedSize, inflater).pipe(entry);
            } else {
              self._pullStream.drain(vars.compressedSize, function (err) {
                if (err) {
                  return self.emit('error', err);
                }
                self._readRecord();
              });
            }
          } else {
            var descriptorSig = new Buffer(4);
            descriptorSig.writeUInt32LE(0x08074b50, 0);

            var matchStream = new MatchStream({ pattern: descriptorSig }, function (buf, matched, extra) {
              if (hasEntryListener) {
                if (!matched) {
                  return this.push(buf);
                }
                this.push(buf);
              }
              setImmediate(function() {
                self._pullStream.unpipe();
                self._pullStream.prepend(extra);
                self._processDataDescriptor(entry);
              });
              return this.push(null);
            });

            self._pullStream.pipe(matchStream);
            if (hasEntryListener) {
              matchStream.pipe(inflater).pipe(entry);
            }
          }
        }
      });
    });
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.unzip.Parse.prototype._readRecord"></a>[function <span class="apidocSignatureSpan">unzip.Parse.prototype.</span>_readRecord ()](#apidoc.element.unzip.Parse.prototype._readRecord)
- description and source-code
```javascript
_readRecord = function () {
  var self = this;
  this._pullStream.pull(4, function (err, data) {
    if (err) {
      return self.emit('error', err);
    }

    if (data.length === 0) {
      return;
    }

    var signature = data.readUInt32LE(0);
    if (signature === 0x04034b50) {
      self._readFile();
    } else if (signature === 0x02014b50) {
      self._readCentralDirectoryFileHeader();
    } else if (signature === 0x06054b50) {
      self._readEndOfCentralDirectoryRecord();
    } else {
      err = new Error('invalid signature: 0x' + signature.toString(16));
      self.emit('error', err);
    }
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.unzip.Parse.prototype._transform"></a>[function <span class="apidocSignatureSpan">unzip.Parse.prototype.</span>_transform (chunk, encoding, callback)](#apidoc.element.unzip.Parse.prototype._transform)
- description and source-code
```javascript
_transform = function (chunk, encoding, callback) {
  if (this._pullStream.write(chunk)) {
    return callback();
  }

  this._pullStream.once('drain', callback);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.unzip.Parse.prototype.addListener"></a>[function <span class="apidocSignatureSpan">unzip.Parse.prototype.</span>addListener (type, listener)](#apidoc.element.unzip.Parse.prototype.addListener)
- description and source-code
```javascript
addListener = function (type, listener) {
  if ('entry' === type) {
    this._hasEntryListener = true;
  }
  return Transform.prototype.addListener.call(this, type, listener);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.unzip.Parse.prototype.on"></a>[function <span class="apidocSignatureSpan">unzip.Parse.prototype.</span>on (type, listener)](#apidoc.element.unzip.Parse.prototype.on)
- description and source-code
```javascript
on = function (type, listener) {
  if ('entry' === type) {
    this._hasEntryListener = true;
  }
  return Transform.prototype.addListener.call(this, type, listener);
}
```
- example usage
```shell
...

__Important__: If you do not intend to consume an entry stream's raw data, call autodrain() to dispose of the entry's
contents. Otherwise you risk running out of memory.

'''javascript
fs.createReadStream('path/to/archive.zip')
.pipe(unzip.Parse())
.on('entry', function (entry) {
  var fileName = entry.path;
  var type = entry.type; // 'Directory' or 'File'
  var size = entry.size;
  if (fileName === "this IS the file I'm looking for") {
    entry.pipe(fs.createWriteStream('output/path'));
  } else {
    entry.autodrain();
...
```

#### <a name="apidoc.element.unzip.Parse.prototype.pipe"></a>[function <span class="apidocSignatureSpan">unzip.Parse.prototype.</span>pipe (dest, opts)](#apidoc.element.unzip.Parse.prototype.pipe)
- description and source-code
```javascript
pipe = function (dest, opts) {
  var self = this;
  if (typeof dest.add === "function") {
    self.on("entry", function (entry) {
      dest.add(entry);
    })
  }
  return Transform.prototype.pipe.apply(this, arguments);
}
```
- example usage
```shell
...
$ npm install unzip
'''

## Quick Examples

### Extract to a directory
'''javascript
fs.createReadStream('path/to/archive.zip').pipe(unzip.Extract({ path: 'output/path' }));
'''

Extract emits the 'close' event once the zip's contents have been fully extracted to disk.

### Parse zip file contents

Process each zip file entry or pipe entries to another stream.
...
```



# <a name="apidoc.module.unzip.Parse.super_"></a>[module unzip.Parse.super_](#apidoc.module.unzip.Parse.super_)

#### <a name="apidoc.element.unzip.Parse.super_.super_"></a>[function <span class="apidocSignatureSpan">unzip.Parse.</span>super_ (options)](#apidoc.element.unzip.Parse.super_.super_)
- description and source-code
```javascript
function Duplex(options) {
  if (!(this instanceof Duplex))
    return new Duplex(options);

  Readable.call(this, options);
  Writable.call(this, options);

  if (options && options.readable === false)
    this.readable = false;

  if (options && options.writable === false)
    this.writable = false;

  this.allowHalfOpen = true;
  if (options && options.allowHalfOpen === false)
    this.allowHalfOpen = false;

  this.once('end', onend);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.unzip.Parse.super_.prototype"></a>[module unzip.Parse.super_.prototype](#apidoc.module.unzip.Parse.super_.prototype)

#### <a name="apidoc.element.unzip.Parse.super_.prototype._read"></a>[function <span class="apidocSignatureSpan">unzip.Parse.super_.prototype.</span>_read (n)](#apidoc.element.unzip.Parse.super_.prototype._read)
- description and source-code
```javascript
_read = function (n) {
  var ts = this._transformState;

  if (ts.writechunk !== null && ts.writecb && !ts.transforming) {
    ts.transforming = true;
    this._transform(ts.writechunk, ts.writeencoding, ts.afterTransform);
  } else {
    // mark that we need a transform, so that any data that comes in
    // will get processed, now that we've asked for it.
    ts.needTransform = true;
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.unzip.Parse.super_.prototype._transform"></a>[function <span class="apidocSignatureSpan">unzip.Parse.super_.prototype.</span>_transform (chunk, encoding, cb)](#apidoc.element.unzip.Parse.super_.prototype._transform)
- description and source-code
```javascript
_transform = function (chunk, encoding, cb) {
  throw new Error('not implemented');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.unzip.Parse.super_.prototype._write"></a>[function <span class="apidocSignatureSpan">unzip.Parse.super_.prototype.</span>_write (chunk, encoding, cb)](#apidoc.element.unzip.Parse.super_.prototype._write)
- description and source-code
```javascript
_write = function (chunk, encoding, cb) {
  var ts = this._transformState;
  ts.writecb = cb;
  ts.writechunk = chunk;
  ts.writeencoding = encoding;
  if (!ts.transforming) {
    var rs = this._readableState;
    if (ts.needTransform ||
        rs.needReadable ||
        rs.length < rs.highWaterMark)
      this._read(rs.highWaterMark);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.unzip.Parse.super_.prototype.push"></a>[function <span class="apidocSignatureSpan">unzip.Parse.super_.prototype.</span>push (chunk, encoding)](#apidoc.element.unzip.Parse.super_.prototype.push)
- description and source-code
```javascript
push = function (chunk, encoding) {
  this._transformState.needTransform = false;
  return Duplex.prototype.push.call(this, chunk, encoding);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.unzip.Parse.super_.super_.prototype"></a>[module unzip.Parse.super_.super_.prototype](#apidoc.module.unzip.Parse.super_.super_.prototype)

#### <a name="apidoc.element.unzip.Parse.super_.super_.prototype._write"></a>[function <span class="apidocSignatureSpan">unzip.Parse.super_.super_.prototype.</span>_write (chunk, encoding, cb)](#apidoc.element.unzip.Parse.super_.super_.prototype._write)
- description and source-code
```javascript
_write = function (chunk, encoding, cb) {
  cb(new Error('not implemented'));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.unzip.Parse.super_.super_.prototype.end"></a>[function <span class="apidocSignatureSpan">unzip.Parse.super_.super_.prototype.</span>end (chunk, encoding, cb)](#apidoc.element.unzip.Parse.super_.super_.prototype.end)
- description and source-code
```javascript
end = function (chunk, encoding, cb) {
  var state = this._writableState;

  if (typeof chunk === 'function') {
    cb = chunk;
    chunk = null;
    encoding = null;
  } else if (typeof encoding === 'function') {
    cb = encoding;
    encoding = null;
  }

  if (typeof chunk !== 'undefined' && chunk !== null)
    this.write(chunk, encoding);

  // ignore unnecessary end() calls.
  if (!state.ending && !state.finished)
    endWritable(this, state, cb);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.unzip.Parse.super_.super_.prototype.write"></a>[function <span class="apidocSignatureSpan">unzip.Parse.super_.super_.prototype.</span>write (chunk, encoding, cb)](#apidoc.element.unzip.Parse.super_.super_.prototype.write)
- description and source-code
```javascript
write = function (chunk, encoding, cb) {
  var state = this._writableState;
  var ret = false;

  if (typeof encoding === 'function') {
    cb = encoding;
    encoding = null;
  }

  if (Buffer.isBuffer(chunk))
    encoding = 'buffer';
  else if (!encoding)
    encoding = state.defaultEncoding;

  if (typeof cb !== 'function')
    cb = function() {};

  if (state.ended)
    writeAfterEnd(this, state, cb);
  else if (validChunk(this, state, chunk, cb))
    ret = writeOrBuffer(this, state, chunk, encoding, cb);

  return ret;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.unzip.entry"></a>[module unzip.entry](#apidoc.module.unzip.entry)

#### <a name="apidoc.element.unzip.entry.entry"></a>[function <span class="apidocSignatureSpan">unzip.</span>entry ()](#apidoc.element.unzip.entry.entry)
- description and source-code
```javascript
function Entry() {
  PassThrough.call(this);
  this.props = {};
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.unzip.entry.super_"></a>[function <span class="apidocSignatureSpan">unzip.entry.</span>super_ (options)](#apidoc.element.unzip.entry.super_)
- description and source-code
```javascript
function PassThrough(options) {
  if (!(this instanceof PassThrough))
    return new PassThrough(options);

  Transform.call(this, options);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.unzip.entry.prototype"></a>[module unzip.entry.prototype](#apidoc.module.unzip.entry.prototype)

#### <a name="apidoc.element.unzip.entry.prototype.autodrain"></a>[function <span class="apidocSignatureSpan">unzip.entry.prototype.</span>autodrain ()](#apidoc.element.unzip.entry.prototype.autodrain)
- description and source-code
```javascript
autodrain = function () {
  this.on('readable', this.read.bind(this));
}
```
- example usage
```shell
...
  .on('entry', function (entry) {
    var fileName = entry.path;
    var type = entry.type; // 'Directory' or 'File'
    var size = entry.size;
    if (fileName === "this IS the file I'm looking for") {
      entry.pipe(fs.createWriteStream('output/path'));
    } else {
      entry.autodrain();
    }
  });
'''

Or pipe the output of unzip.Parse() to fstream

'''javascript
...
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
