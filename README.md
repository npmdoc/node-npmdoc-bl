# api documentation for  [bl (v1.2.0)](https://github.com/rvagg/bl)  [![npm package](https://img.shields.io/npm/v/npmdoc-bl.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-bl) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-bl.svg)](https://travis-ci.org/npmdoc/node-npmdoc-bl)
#### Buffer List: collect buffers and access with a standard readable Buffer interface, streamable too!

[![NPM](https://nodei.co/npm/bl.png?downloads=true)](https://www.npmjs.com/package/bl)

[![apidoc](https://npmdoc.github.io/node-npmdoc-bl/build/screen-capture.buildNpmdoc.browser._2Fhome_2Ftravis_2Fbuild_2Fnpmdoc_2Fnode-npmdoc-bl_2Ftmp_2Fbuild_2Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-bl/build..beta..travis-ci.org/apidoc.html)

![package-listing](https://npmdoc.github.io/node-npmdoc-bl/build/screen-capture.npmPackageListing.svg)



# package.json

```json

{
    "authors": [
        "Rod Vagg <rod@vagg.org> (https://github.com/rvagg)",
        "Matteo Collina <matteo.collina@gmail.com> (https://github.com/mcollina)",
        "Jarett Cruger <jcrugzz@gmail.com> (https://github.com/jcrugzz)"
    ],
    "bugs": {
        "url": "https://github.com/rvagg/bl/issues"
    },
    "dependencies": {
        "readable-stream": "^2.0.5"
    },
    "description": "Buffer List: collect buffers and access with a standard readable Buffer interface, streamable too!",
    "devDependencies": {
        "faucet": "0.0.1",
        "hash_file": "~0.1.1",
        "tape": "~4.6.0"
    },
    "directories": {},
    "dist": {
        "shasum": "1397e7ec42c5f5dc387470c500e34a9f6be9ea98",
        "tarball": "https://registry.npmjs.org/bl/-/bl-1.2.0.tgz"
    },
    "gitHead": "199e5c1807c378c8af5d81be0bb3c30921ce530a",
    "homepage": "https://github.com/rvagg/bl",
    "keywords": [
        "buffer",
        "buffers",
        "stream",
        "awesomesauce"
    ],
    "license": "MIT",
    "main": "bl.js",
    "maintainers": [
        {
            "name": "matteo.collina",
            "email": "hello@matteocollina.com"
        },
        {
            "name": "rvagg",
            "email": "rod@vagg.org"
        }
    ],
    "name": "bl",
    "optionalDependencies": {},
    "readme": "ERROR: No README data found!",
    "repository": {
        "type": "git",
        "url": "git+https://github.com/rvagg/bl.git"
    },
    "scripts": {
        "test": "node test/test.js | faucet"
    },
    "version": "1.2.0"
}
```



# <a name="apidoc.tableOfContents"></a>[table of contents](#apidoc.tableOfContents)

#### [module bl](#apidoc.module.bl)
1.  [function <span class="apidocSignatureSpan">bl.</span>super_ (options)](#apidoc.element.bl.super_)
1.  [function <span class="apidocSignatureSpan">bl.</span>super_.super_ (options)](#apidoc.element.bl.super_.super_)
1.  object <span class="apidocSignatureSpan">bl.</span>super_.prototype
1.  object <span class="apidocSignatureSpan">bl.</span>super_.super_.prototype

#### [module bl.super_](#apidoc.module.bl.super_)
1.  [function <span class="apidocSignatureSpan">bl.</span>super_ (options)](#apidoc.element.bl.super_.super_)

#### [module bl.super_.prototype](#apidoc.module.bl.super_.prototype)
1.  [function <span class="apidocSignatureSpan">bl.super_.prototype.</span>_write (chunk, encoding, cb)](#apidoc.element.bl.super_.prototype._write)
1.  [function <span class="apidocSignatureSpan">bl.super_.prototype.</span>cork ()](#apidoc.element.bl.super_.prototype.cork)
1.  [function <span class="apidocSignatureSpan">bl.super_.prototype.</span>end (chunk, encoding, cb)](#apidoc.element.bl.super_.prototype.end)
1.  [function <span class="apidocSignatureSpan">bl.super_.prototype.</span>setDefaultEncoding (encoding)](#apidoc.element.bl.super_.prototype.setDefaultEncoding)
1.  [function <span class="apidocSignatureSpan">bl.super_.prototype.</span>uncork ()](#apidoc.element.bl.super_.prototype.uncork)
1.  [function <span class="apidocSignatureSpan">bl.super_.prototype.</span>write (chunk, encoding, cb)](#apidoc.element.bl.super_.prototype.write)
1.  object <span class="apidocSignatureSpan">bl.super_.prototype.</span>_writev

#### [module bl.super_.super_](#apidoc.module.bl.super_.super_)
1.  [function <span class="apidocSignatureSpan">bl.super_.</span>super_ ()](#apidoc.element.bl.super_.super_.super_)
1.  [function <span class="apidocSignatureSpan">bl.super_.super_.</span>ReadableState (options, stream)](#apidoc.element.bl.super_.super_.ReadableState)
1.  [function <span class="apidocSignatureSpan">bl.super_.super_.</span>_fromList (n, state)](#apidoc.element.bl.super_.super_._fromList)

#### [module bl.super_.super_.prototype](#apidoc.module.bl.super_.super_.prototype)
1.  [function <span class="apidocSignatureSpan">bl.super_.super_.prototype.</span>_read (n)](#apidoc.element.bl.super_.super_.prototype._read)
1.  [function <span class="apidocSignatureSpan">bl.super_.super_.prototype.</span>addListener (ev, fn)](#apidoc.element.bl.super_.super_.prototype.addListener)
1.  [function <span class="apidocSignatureSpan">bl.super_.super_.prototype.</span>isPaused ()](#apidoc.element.bl.super_.super_.prototype.isPaused)
1.  [function <span class="apidocSignatureSpan">bl.super_.super_.prototype.</span>on (ev, fn)](#apidoc.element.bl.super_.super_.prototype.on)
1.  [function <span class="apidocSignatureSpan">bl.super_.super_.prototype.</span>pause ()](#apidoc.element.bl.super_.super_.prototype.pause)
1.  [function <span class="apidocSignatureSpan">bl.super_.super_.prototype.</span>pipe (dest, pipeOpts)](#apidoc.element.bl.super_.super_.prototype.pipe)
1.  [function <span class="apidocSignatureSpan">bl.super_.super_.prototype.</span>push (chunk, encoding)](#apidoc.element.bl.super_.super_.prototype.push)
1.  [function <span class="apidocSignatureSpan">bl.super_.super_.prototype.</span>read (n)](#apidoc.element.bl.super_.super_.prototype.read)
1.  [function <span class="apidocSignatureSpan">bl.super_.super_.prototype.</span>resume ()](#apidoc.element.bl.super_.super_.prototype.resume)
1.  [function <span class="apidocSignatureSpan">bl.super_.super_.prototype.</span>setEncoding (enc)](#apidoc.element.bl.super_.super_.prototype.setEncoding)
1.  [function <span class="apidocSignatureSpan">bl.super_.super_.prototype.</span>unpipe (dest)](#apidoc.element.bl.super_.super_.prototype.unpipe)
1.  [function <span class="apidocSignatureSpan">bl.super_.super_.prototype.</span>unshift (chunk)](#apidoc.element.bl.super_.super_.prototype.unshift)
1.  [function <span class="apidocSignatureSpan">bl.super_.super_.prototype.</span>wrap (stream)](#apidoc.element.bl.super_.super_.prototype.wrap)



# <a name="apidoc.module.bl"></a>[module bl](#apidoc.module.bl)

#### <a name="apidoc.element.bl.super_"></a>[function <span class="apidocSignatureSpan">bl.</span>super_ (options)](#apidoc.element.bl.super_)
- description and source-code
```javascript
function Duplex(options) {
  if (!(this instanceof Duplex)) return new Duplex(options);

  Readable.call(this, options);
  Writable.call(this, options);

  if (options && options.readable === false) this.readable = false;

  if (options && options.writable === false) this.writable = false;

  this.allowHalfOpen = true;
  if (options && options.allowHalfOpen === false) this.allowHalfOpen = false;

  this.once('end', onend);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.bl.super_.super_"></a>[function <span class="apidocSignatureSpan">bl.</span>super_.super_ (options)](#apidoc.element.bl.super_.super_)
- description and source-code
```javascript
function Readable(options) {
  Duplex = Duplex || require('./_stream_duplex');

  if (!(this instanceof Readable)) return new Readable(options);

  this._readableState = new ReadableState(options, this);

  // legacy
  this.readable = true;

  if (options && typeof options.read === 'function') this._read = options.read;

  Stream.call(this);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.bl.super_"></a>[module bl.super_](#apidoc.module.bl.super_)

#### <a name="apidoc.element.bl.super_.super_"></a>[function <span class="apidocSignatureSpan">bl.</span>super_ (options)](#apidoc.element.bl.super_.super_)
- description and source-code
```javascript
function Readable(options) {
  Duplex = Duplex || require('./_stream_duplex');

  if (!(this instanceof Readable)) return new Readable(options);

  this._readableState = new ReadableState(options, this);

  // legacy
  this.readable = true;

  if (options && typeof options.read === 'function') this._read = options.read;

  Stream.call(this);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.bl.super_.prototype"></a>[module bl.super_.prototype](#apidoc.module.bl.super_.prototype)

#### <a name="apidoc.element.bl.super_.prototype._write"></a>[function <span class="apidocSignatureSpan">bl.super_.prototype.</span>_write (chunk, encoding, cb)](#apidoc.element.bl.super_.prototype._write)
- description and source-code
```javascript
_write = function (chunk, encoding, cb) {
  cb(new Error('_write() is not implemented'));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.bl.super_.prototype.cork"></a>[function <span class="apidocSignatureSpan">bl.super_.prototype.</span>cork ()](#apidoc.element.bl.super_.prototype.cork)
- description and source-code
```javascript
cork = function () {
  var state = this._writableState;

  state.corked++;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.bl.super_.prototype.end"></a>[function <span class="apidocSignatureSpan">bl.super_.prototype.</span>end (chunk, encoding, cb)](#apidoc.element.bl.super_.prototype.end)
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

  if (chunk !== null && chunk !== undefined) this.write(chunk, encoding);

  // .end() fully uncorks
  if (state.corked) {
    state.corked = 1;
    this.uncork();
  }

  // ignore unnecessary end() calls.
  if (!state.ending && !state.finished) endWritable(this, state, cb);
}
```
- example usage
```shell
...
  * <a href="#toString"><code>bl.<b>toString([encoding, [ start, [ end ]]])</b></code></a>
  * <a href="#readXX"><code>bl.<b>readDoubleBE()</b></code>, <code>bl.<b>readDoubleLE()</b></code>, <code>bl.<b>readFloatBE()</b
></code>, <code>bl.<b>readFloatLE()</b></code>, <code>bl.<b>readInt32BE()</b></code>, <code>bl.<b>readInt32LE()</b></code>, <code
>bl.<b>readUInt32BE()</b></code>, <code>bl.<b>readUInt32LE()</b></code>, <code>bl.<b>readInt16BE()</b></code>, <code>bl.<b>readInt16LE
()</b></code>, <code>bl.<b>readUInt16BE()</b></code>, <code>bl.<b>readUInt16LE()</b></code>, <code>bl.<b>readInt8()</b></code>, <
code>bl.<b>readUInt8()</b></code></a>
  * <a href="#streams">Streams</a>

--------------------------------------------------------
<a name="ctor"></a>
### new BufferList([ callback | Buffer | Buffer array | BufferList | BufferList array | String ])
The constructor takes an optional callback, if supplied, the callback will be called with an error argument followed by a reference
 to the **bl** instance, when 'bl.end()' is called (i.e. from a piped stream). This is a convenient method of collecting the entire
 contents of a stream, particularly when the stream is *chunky*, such as a network stream.

Normally, no arguments are required for the constructor, but you can initialise the list by passing in a single 'Buffer' object
or an array of 'Buffer' object.

'new' is not strictly required, if you don't instantiate a new object, it will be done automatically for you so you can create a
 new instance simply with:

'''js
var bl = require('bl')
...
```

#### <a name="apidoc.element.bl.super_.prototype.setDefaultEncoding"></a>[function <span class="apidocSignatureSpan">bl.super_.prototype.</span>setDefaultEncoding (encoding)](#apidoc.element.bl.super_.prototype.setDefaultEncoding)
- description and source-code
```javascript
function setDefaultEncoding(encoding) {
  // node::ParseEncoding() requires lower case.
  if (typeof encoding === 'string') encoding = encoding.toLowerCase();
  if (!(['hex', 'utf8', 'utf-8', 'ascii', 'binary', 'base64', 'ucs2', 'ucs-2', 'utf16le', 'utf-16le', 'raw'].indexOf((encoding + '').
toLowerCase()) > -1)) throw new TypeError('Unknown encoding: ' + encoding);
  this._writableState.defaultEncoding = encoding;
  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.bl.super_.prototype.uncork"></a>[function <span class="apidocSignatureSpan">bl.super_.prototype.</span>uncork ()](#apidoc.element.bl.super_.prototype.uncork)
- description and source-code
```javascript
uncork = function () {
  var state = this._writableState;

  if (state.corked) {
    state.corked--;

    if (!state.writing && !state.corked && !state.finished && !state.bufferProcessing && state.bufferedRequest) clearBuffer(this
, state);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.bl.super_.prototype.write"></a>[function <span class="apidocSignatureSpan">bl.super_.prototype.</span>write (chunk, encoding, cb)](#apidoc.element.bl.super_.prototype.write)
- description and source-code
```javascript
write = function (chunk, encoding, cb) {
  var state = this._writableState;
  var ret = false;
  var isBuf = Buffer.isBuffer(chunk);

  if (typeof encoding === 'function') {
    cb = encoding;
    encoding = null;
  }

  if (isBuf) encoding = 'buffer';else if (!encoding) encoding = state.defaultEncoding;

  if (typeof cb !== 'function') cb = nop;

  if (state.ended) writeAfterEnd(this, cb);else if (isBuf || validChunk(this, state, chunk, cb)) {
    state.pendingcb++;
    ret = writeOrBuffer(this, state, isBuf, chunk, encoding, cb);
  }

  return ret;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.bl.super_.super_"></a>[module bl.super_.super_](#apidoc.module.bl.super_.super_)

#### <a name="apidoc.element.bl.super_.super_.super_"></a>[function <span class="apidocSignatureSpan">bl.super_.</span>super_ ()](#apidoc.element.bl.super_.super_.super_)
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

#### <a name="apidoc.element.bl.super_.super_.ReadableState"></a>[function <span class="apidocSignatureSpan">bl.super_.super_.</span>ReadableState (options, stream)](#apidoc.element.bl.super_.super_.ReadableState)
- description and source-code
```javascript
function ReadableState(options, stream) {
  Duplex = Duplex || require('./_stream_duplex');

  options = options || {};

  // object stream flag. Used to make read(n) ignore n and to
  // make all the buffer merging and length checks go away
  this.objectMode = !!options.objectMode;

  if (stream instanceof Duplex) this.objectMode = this.objectMode || !!options.readableObjectMode;

  // the point at which it stops calling _read() to fill the buffer
  // Note: 0 is a valid value, means "don't call _read preemptively ever"
  var hwm = options.highWaterMark;
  var defaultHwm = this.objectMode ? 16 : 16 * 1024;
  this.highWaterMark = hwm || hwm === 0 ? hwm : defaultHwm;

  // cast to ints.
  this.highWaterMark = ~~this.highWaterMark;

  // A linked list is used to store data chunks instead of an array because the
  // linked list can remove elements from the beginning faster than
  // array.shift()
  this.buffer = new BufferList();
  this.length = 0;
  this.pipes = null;
  this.pipesCount = 0;
  this.flowing = null;
  this.ended = false;
  this.endEmitted = false;
  this.reading = false;

  // a flag to be able to tell if the onwrite cb is called immediately,
  // or on a later tick.  We set this to true at first, because any
  // actions that shouldn't happen until "later" should generally also
  // not happen before the first write call.
  this.sync = true;

  // whenever we return null, then we set a flag to say
  // that we're awaiting a 'readable' event emission.
  this.needReadable = false;
  this.emittedReadable = false;
  this.readableListening = false;
  this.resumeScheduled = false;

  // Crypto is kind of old and crusty.  Historically, its default string
  // encoding is 'binary' so we have to make this configurable.
  // Everything else in the universe uses 'utf8', though.
  this.defaultEncoding = options.defaultEncoding || 'utf8';

  // when piping, we only care about 'readable' events that happen
  // after read()ing all the bytes and not getting any pushback.
  this.ranOut = false;

  // the number of writers that are awaiting a drain event in .pipe()s
  this.awaitDrain = 0;

  // if true, a maybeReadMore has been scheduled
  this.readingMore = false;

  this.decoder = null;
  this.encoding = null;
  if (options.encoding) {
    if (!StringDecoder) StringDecoder = require('string_decoder/').StringDecoder;
    this.decoder = new StringDecoder(options.encoding);
    this.encoding = options.encoding;
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.bl.super_.super_._fromList"></a>[function <span class="apidocSignatureSpan">bl.super_.super_.</span>_fromList (n, state)](#apidoc.element.bl.super_.super_._fromList)
- description and source-code
```javascript
function fromList(n, state) {
  // nothing buffered
  if (state.length === 0) return null;

  var ret;
  if (state.objectMode) ret = state.buffer.shift();else if (!n || n >= state.length) {
    // read it all, truncate the list
    if (state.decoder) ret = state.buffer.join('');else if (state.buffer.length === 1) ret = state.buffer.head.data;else ret = state
.buffer.concat(state.length);
    state.buffer.clear();
  } else {
    // read part of list
    ret = fromListPartial(n, state.buffer, state.decoder);
  }

  return ret;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.bl.super_.super_.prototype"></a>[module bl.super_.super_.prototype](#apidoc.module.bl.super_.super_.prototype)

#### <a name="apidoc.element.bl.super_.super_.prototype._read"></a>[function <span class="apidocSignatureSpan">bl.super_.super_.prototype.</span>_read (n)](#apidoc.element.bl.super_.super_.prototype._read)
- description and source-code
```javascript
_read = function (n) {
  this.emit('error', new Error('_read() is not implemented'));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.bl.super_.super_.prototype.addListener"></a>[function <span class="apidocSignatureSpan">bl.super_.super_.prototype.</span>addListener (ev, fn)](#apidoc.element.bl.super_.super_.prototype.addListener)
- description and source-code
```javascript
addListener = function (ev, fn) {
  var res = Stream.prototype.on.call(this, ev, fn);

  if (ev === 'data') {
    // Start flowing on next tick if stream isn't explicitly paused
    if (this._readableState.flowing !== false) this.resume();
  } else if (ev === 'readable') {
    var state = this._readableState;
    if (!state.endEmitted && !state.readableListening) {
      state.readableListening = state.needReadable = true;
      state.emittedReadable = false;
      if (!state.reading) {
        processNextTick(nReadingNextTick, this);
      } else if (state.length) {
        emitReadable(this, state);
      }
    }
  }

  return res;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.bl.super_.super_.prototype.isPaused"></a>[function <span class="apidocSignatureSpan">bl.super_.super_.prototype.</span>isPaused ()](#apidoc.element.bl.super_.super_.prototype.isPaused)
- description and source-code
```javascript
isPaused = function () {
  return this._readableState.flowing === false;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.bl.super_.super_.prototype.on"></a>[function <span class="apidocSignatureSpan">bl.super_.super_.prototype.</span>on (ev, fn)](#apidoc.element.bl.super_.super_.prototype.on)
- description and source-code
```javascript
on = function (ev, fn) {
  var res = Stream.prototype.on.call(this, ev, fn);

  if (ev === 'data') {
    // Start flowing on next tick if stream isn't explicitly paused
    if (this._readableState.flowing !== false) this.resume();
  } else if (ev === 'readable') {
    var state = this._readableState;
    if (!state.endEmitted && !state.readableListening) {
      state.readableListening = state.needReadable = true;
      state.emittedReadable = false;
      if (!state.reading) {
        processNextTick(nReadingNextTick, this);
      } else if (state.length) {
        emitReadable(this, state);
      }
    }
  }

  return res;
}
```
- example usage
```shell
...
  var piper = function piper (err) {
    if (this._callback) {
      this._callback(err)
      this._callback = null
    }
  }.bind(this)

  this.on('pipe', function onPipe (src) {
    src.on('error', piper)
  })
  this.on('unpipe', function onUnpipe (src) {
    src.removeListener('error', piper)
  })
} else {
  this.append(callback)
...
```

#### <a name="apidoc.element.bl.super_.super_.prototype.pause"></a>[function <span class="apidocSignatureSpan">bl.super_.super_.prototype.</span>pause ()](#apidoc.element.bl.super_.super_.prototype.pause)
- description and source-code
```javascript
pause = function () {
  debug('call pause flowing=%j', this._readableState.flowing);
  if (false !== this._readableState.flowing) {
    debug('pause');
    this._readableState.flowing = false;
    this.emit('pause');
  }
  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.bl.super_.super_.prototype.pipe"></a>[function <span class="apidocSignatureSpan">bl.super_.super_.prototype.</span>pipe (dest, pipeOpts)](#apidoc.element.bl.super_.super_.prototype.pipe)
- description and source-code
```javascript
pipe = function (dest, pipeOpts) {
  var src = this;
  var state = this._readableState;

  switch (state.pipesCount) {
    case 0:
      state.pipes = dest;
      break;
    case 1:
      state.pipes = [state.pipes, dest];
      break;
    default:
      state.pipes.push(dest);
      break;
  }
  state.pipesCount += 1;
  debug('pipe count=%d opts=%j', state.pipesCount, pipeOpts);

  var doEnd = (!pipeOpts || pipeOpts.end !== false) && dest !== process.stdout && dest !== process.stderr;

  var endFn = doEnd ? onend : cleanup;
  if (state.endEmitted) processNextTick(endFn);else src.once('end', endFn);

  dest.on('unpipe', onunpipe);
  function onunpipe(readable) {
    debug('onunpipe');
    if (readable === src) {
      cleanup();
    }
  }

  function onend() {
    debug('onend');
    dest.end();
  }

  // when the dest drains, it reduces the awaitDrain counter
  // on the source.  This would be more elegant with a .once()
  // handler in flow(), but adding and removing repeatedly is
  // too slow.
  var ondrain = pipeOnDrain(src);
  dest.on('drain', ondrain);

  var cleanedUp = false;
  function cleanup() {
    debug('cleanup');
    // cleanup event handlers once the pipe is broken
    dest.removeListener('close', onclose);
    dest.removeListener('finish', onfinish);
    dest.removeListener('drain', ondrain);
    dest.removeListener('error', onerror);
    dest.removeListener('unpipe', onunpipe);
    src.removeListener('end', onend);
    src.removeListener('end', cleanup);
    src.removeListener('data', ondata);

    cleanedUp = true;

    // if the reader is waiting for a drain event from this
    // specific writer, then it would cause it to never start
    // flowing again.
    // So, if this is awaiting a drain, then we just call it now.
    // If we don't know, then assume that we are waiting for one.
    if (state.awaitDrain && (!dest._writableState || dest._writableState.needDrain)) ondrain();
  }

  // If the user pushes more data while we're writing to dest then we'll end up
  // in ondata again. However, we only want to increase awaitDrain once because
  // dest will only emit one 'drain' event for the multiple writes.
  // => Introduce a guard on increasing awaitDrain.
  var increasedAwaitDrain = false;
  src.on('data', ondata);
  function ondata(chunk) {
    debug('ondata');
    increasedAwaitDrain = false;
    var ret = dest.write(chunk);
    if (false === ret && !increasedAwaitDrain) {
      // If the user unpiped during 'dest.write()', it is possible
      // to get stuck in a permanently paused state if that write
      // also returned false.
      // => Check whether 'dest' is still a piping destination.
      if ((state.pipesCount === 1 && state.pipes === dest || state.pipesCount > 1 && indexOf(state.pipes, dest) !== -1) && !cleanedUp
) {
        debug('false write response, pause', src._readableState.awaitDrain);
        src._readableState.awaitDrain++;
        increasedAwaitDrain = true;
      }
      src.pause();
    }
  }

  // if the dest has an error, then stop piping into it.
  // however, don't suppress the throwing behavior for this.
  function onerror(er) {
    debug('onerror', er);
    unpipe();
    dest.removeListener('error', onerror);
    if (EElistenerCount(dest, 'error') === 0) dest.emit('error', er);
  }

  // Make sure our error handler is attached before userland ones.
  prependListener(dest, 'error', onerror);

  // Both close and finish should trigger unpipe, but only once.
  function onclose() {
    dest.removeListener('finish', onfinish);
    unpipe();
  }
  dest.once('close', onclose);
  function onfinish() {
    debug('onfinish');
    dest.removeListener('close', onclose);
    unpipe();
  }
  dest.once('finish', onfinish);

  function unpipe() {
    debug('unpipe');
    src.unpipe(dest);
  }

  // tell the dest that it's being piped to
  dest.emit('pipe', src);

  // start the flow if it hasn't been started already.
  if (!state.flowing) {
    debug('pipe resume');
    src.resume();
  }

  return dest;
}
```
- example usage
```shell
...
Give it a callback in the constructor and use it just like **[concat-stream](https://github.com/maxogden/node-concat-stream)**:

'''js
const bl = require('bl')
    , fs = require('fs')

fs.createReadStream('README.md')
  .pipe(bl(function (err, data) { // note 'new' isn't strictly required
    // 'data' is a complete Buffer object containing the full data
    console.log(data.toString())
  }))
'''

Note that when you use the *callback* method like this, the resulting 'data' parameter is a concatenation of all 'Buffer' objects
 in the list. If you want to avoid the overhead of this concatenation (in cases of extreme performance consciousness), then avoid
 the *callback* method and just listen to ''end'' instead, like a standard Stream.
...
```

#### <a name="apidoc.element.bl.super_.super_.prototype.push"></a>[function <span class="apidocSignatureSpan">bl.super_.super_.prototype.</span>push (chunk, encoding)](#apidoc.element.bl.super_.super_.prototype.push)
- description and source-code
```javascript
push = function (chunk, encoding) {
  var state = this._readableState;

  if (!state.objectMode && typeof chunk === 'string') {
    encoding = encoding || state.defaultEncoding;
    if (encoding !== state.encoding) {
      chunk = bufferShim.from(chunk, encoding);
      encoding = '';
    }
  }

  return readableAddChunk(this, state, chunk, encoding, false);
}
```
- example usage
```shell
...
}

return this
}


BufferList.prototype._appendBuffer = function appendBuffer (buf) {
this._bufs.push(buf)
this.length += buf.length
}


BufferList.prototype._write = function _write (buf, encoding, callback) {
this._appendBuffer(buf)
...
```

#### <a name="apidoc.element.bl.super_.super_.prototype.read"></a>[function <span class="apidocSignatureSpan">bl.super_.super_.prototype.</span>read (n)](#apidoc.element.bl.super_.super_.prototype.read)
- description and source-code
```javascript
read = function (n) {
  debug('read', n);
  n = parseInt(n, 10);
  var state = this._readableState;
  var nOrig = n;

  if (n !== 0) state.emittedReadable = false;

  // if we're doing read(0) to trigger a readable event, but we
  // already have a bunch of data in the buffer, then just trigger
  // the 'readable' event and move on.
  if (n === 0 && state.needReadable && (state.length >= state.highWaterMark || state.ended)) {
    debug('read: emitReadable', state.length, state.ended);
    if (state.length === 0 && state.ended) endReadable(this);else emitReadable(this);
    return null;
  }

  n = howMuchToRead(n, state);

  // if we've ended, and we're now clear, then finish it up.
  if (n === 0 && state.ended) {
    if (state.length === 0) endReadable(this);
    return null;
  }

  // All the actual chunk generation logic needs to be
  // *below* the call to _read.  The reason is that in certain
  // synthetic stream cases, such as passthrough streams, _read
  // may be a completely synchronous operation which may change
  // the state of the read buffer, providing enough data when
  // before there was *not* enough.
  //
  // So, the steps are:
  // 1. Figure out what the state of things will be after we do
  // a read from the buffer.
  //
  // 2. If that resulting state will trigger a _read, then call _read.
  // Note that this may be asynchronous, or synchronous.  Yes, it is
  // deeply ugly to write APIs this way, but that still doesn't mean
  // that the Readable class should behave improperly, as streams are
  // designed to be sync/async agnostic.
  // Take note if the _read call is sync or async (ie, if the read call
  // has returned yet), so that we know whether or not it's safe to emit
  // 'readable' etc.
  //
  // 3. Actually pull the requested chunks out of the buffer and return.

  // if we need a readable event, then we need to do some reading.
  var doRead = state.needReadable;
  debug('need readable', doRead);

  // if we currently have less than the highWaterMark, then also read some
  if (state.length === 0 || state.length - n < state.highWaterMark) {
    doRead = true;
    debug('length less than watermark', doRead);
  }

  // however, if we've ended, then there's no point, and if we're already
  // reading, then it's unnecessary.
  if (state.ended || state.reading) {
    doRead = false;
    debug('reading or ended', doRead);
  } else if (doRead) {
    debug('do read');
    state.reading = true;
    state.sync = true;
    // if the length is currently zero, then we *need* a readable event.
    if (state.length === 0) state.needReadable = true;
    // call internal read method
    this._read(state.highWaterMark);
    state.sync = false;
    // If _read pushed data synchronously, then 'reading' will be false,
    // and we need to re-evaluate how much data we can return to the user.
    if (!state.reading) n = howMuchToRead(nOrig, state);
  }

  var ret;
  if (n > 0) ret = fromList(n, state);else ret = null;

  if (ret === null) {
    state.needReadable = true;
    n = 0;
  } else {
    state.length -= n;
  }

  if (state.length === 0) {
    // If we have nothing in the buffer, then we want to know
    // as soon as we *do* get something into the buffer.
    if (!state.ended) state.needReadable = true;

    // If we tried to read() past the EOF, then emit end on the next tick.
    if (nOrig !== n && state.ended) endReadable(this);
  }

  if (ret !== null) this.emit('data', ret);

  return ret;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.bl.super_.super_.prototype.resume"></a>[function <span class="apidocSignatureSpan">bl.super_.super_.prototype.</span>resume ()](#apidoc.element.bl.super_.super_.prototype.resume)
- description and source-code
```javascript
resume = function () {
  var state = this._readableState;
  if (!state.flowing) {
    debug('resume');
    state.flowing = true;
    resume(this, state);
  }
  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.bl.super_.super_.prototype.setEncoding"></a>[function <span class="apidocSignatureSpan">bl.super_.super_.prototype.</span>setEncoding (enc)](#apidoc.element.bl.super_.super_.prototype.setEncoding)
- description and source-code
```javascript
setEncoding = function (enc) {
  if (!StringDecoder) StringDecoder = require('string_decoder/').StringDecoder;
  this._readableState.decoder = new StringDecoder(enc);
  this._readableState.encoding = enc;
  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.bl.super_.super_.prototype.unpipe"></a>[function <span class="apidocSignatureSpan">bl.super_.super_.prototype.</span>unpipe (dest)](#apidoc.element.bl.super_.super_.prototype.unpipe)
- description and source-code
```javascript
unpipe = function (dest) {
  var state = this._readableState;

  // if we're not piping anywhere, then do nothing.
  if (state.pipesCount === 0) return this;

  // just one destination.  most common case.
  if (state.pipesCount === 1) {
    // passed in one, but it's not the right one.
    if (dest && dest !== state.pipes) return this;

    if (!dest) dest = state.pipes;

    // got a match.
    state.pipes = null;
    state.pipesCount = 0;
    state.flowing = false;
    if (dest) dest.emit('unpipe', this);
    return this;
  }

  // slow case. multiple pipe destinations.

  if (!dest) {
    // remove all.
    var dests = state.pipes;
    var len = state.pipesCount;
    state.pipes = null;
    state.pipesCount = 0;
    state.flowing = false;

    for (var i = 0; i < len; i++) {
      dests[i].emit('unpipe', this);
    }return this;
  }

  // try to find the right one.
  var index = indexOf(state.pipes, dest);
  if (index === -1) return this;

  state.pipes.splice(index, 1);
  state.pipesCount -= 1;
  if (state.pipesCount === 1) state.pipes = state.pipes[0];

  dest.emit('unpipe', this);

  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.bl.super_.super_.prototype.unshift"></a>[function <span class="apidocSignatureSpan">bl.super_.super_.prototype.</span>unshift (chunk)](#apidoc.element.bl.super_.super_.prototype.unshift)
- description and source-code
```javascript
unshift = function (chunk) {
  var state = this._readableState;
  return readableAddChunk(this, state, chunk, '', true);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.bl.super_.super_.prototype.wrap"></a>[function <span class="apidocSignatureSpan">bl.super_.super_.prototype.</span>wrap (stream)](#apidoc.element.bl.super_.super_.prototype.wrap)
- description and source-code
```javascript
wrap = function (stream) {
  var state = this._readableState;
  var paused = false;

  var self = this;
  stream.on('end', function () {
    debug('wrapped end');
    if (state.decoder && !state.ended) {
      var chunk = state.decoder.end();
      if (chunk && chunk.length) self.push(chunk);
    }

    self.push(null);
  });

  stream.on('data', function (chunk) {
    debug('wrapped data');
    if (state.decoder) chunk = state.decoder.write(chunk);

    // don't skip over falsy values in objectMode
    if (state.objectMode && (chunk === null || chunk === undefined)) return;else if (!state.objectMode && (!chunk || !chunk.length
)) return;

    var ret = self.push(chunk);
    if (!ret) {
      paused = true;
      stream.pause();
    }
  });

  // proxy all the other methods.
  // important when wrapping filters and duplexes.
  for (var i in stream) {
    if (this[i] === undefined && typeof stream[i] === 'function') {
      this[i] = function (method) {
        return function () {
          return stream[method].apply(stream, arguments);
        };
      }(i);
    }
  }

  // proxy certain important events.
  var events = ['error', 'close', 'destroy', 'pause', 'resume'];
  forEach(events, function (ev) {
    stream.on(ev, self.emit.bind(self, ev));
  });

  // when we try to consume some more bytes, simply unpause the
  // underlying stream.
  self._read = function (n) {
    debug('wrapped _read', n);
    if (paused) {
      paused = false;
      stream.resume();
    }
  };

  return self;
}
```
- example usage
```shell
n/a
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
