# api documentation for  [lunr (v1.0.0)](http://lunrjs.com)  [![npm package](https://img.shields.io/npm/v/npmdoc-lunr.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-lunr) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-lunr.svg)](https://travis-ci.org/npmdoc/node-npmdoc-lunr)
#### Simple full-text search in your browser.

[![NPM](https://nodei.co/npm/lunr.png?downloads=true)](https://www.npmjs.com/package/lunr)

[![apidoc](https://npmdoc.github.io/node-npmdoc-lunr/build/screenCapture.buildNpmdoc.browser._2Fhome_2Ftravis_2Fbuild_2Fnpmdoc_2Fnode-npmdoc-lunr_2Ftmp_2Fbuild_2Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-lunr/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-lunr/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-lunr/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Oliver Nightingale"
    },
    "bugs": {
        "url": "http://github.com/olivernn/lunr.js/issues"
    },
    "dependencies": {},
    "description": "Simple full-text search in your browser.",
    "devDependencies": {
        "dox": "0.4.4",
        "dox-template": "0.1.1",
        "phantomjs": "1.9.*",
        "uglify-js": "2.4.13"
    },
    "directories": {},
    "dist": {
        "shasum": "5c9276c92c91ac35a9241b5018d46723d92e2f5f",
        "tarball": "https://registry.npmjs.org/lunr/-/lunr-1.0.0.tgz"
    },
    "gitHead": "20789e26f3732188216d7faf6dafb0a3656f4703",
    "homepage": "http://lunrjs.com",
    "keywords": [
        "search"
    ],
    "license": "MIT",
    "main": "lunr.js",
    "maintainers": [
        {
            "name": "olivernn",
            "email": "oliver.nightingale1@gmail.com"
        }
    ],
    "name": "lunr",
    "optionalDependencies": {},
    "readme": "ERROR: No README data found!",
    "repository": {
        "type": "git",
        "url": "git+https://github.com/olivernn/lunr.js.git"
    },
    "scripts": {
        "start": "node server.js",
        "test": "make test"
    },
    "version": "1.0.0"
}
```



# <a name="apidoc.tableOfContents"></a>[table of contents](#apidoc.tableOfContents)

#### [module lunr](#apidoc.module.lunr)
1.  [function <span class="apidocSignatureSpan">lunr.</span>EventEmitter ()](#apidoc.element.lunr.EventEmitter)
1.  [function <span class="apidocSignatureSpan">lunr.</span>Index ()](#apidoc.element.lunr.Index)
1.  [function <span class="apidocSignatureSpan">lunr.</span>Pipeline ()](#apidoc.element.lunr.Pipeline)
1.  [function <span class="apidocSignatureSpan">lunr.</span>SortedSet ()](#apidoc.element.lunr.SortedSet)
1.  [function <span class="apidocSignatureSpan">lunr.</span>Store ()](#apidoc.element.lunr.Store)
1.  [function <span class="apidocSignatureSpan">lunr.</span>TokenStore ()](#apidoc.element.lunr.TokenStore)
1.  [function <span class="apidocSignatureSpan">lunr.</span>Vector ()](#apidoc.element.lunr.Vector)
1.  [function <span class="apidocSignatureSpan">lunr.</span>generateStopWordFilter (stopWords)](#apidoc.element.lunr.generateStopWordFilter)
1.  [function <span class="apidocSignatureSpan">lunr.</span>stemmer (w)](#apidoc.element.lunr.stemmer)
1.  [function <span class="apidocSignatureSpan">lunr.</span>stopWordFilter (token)](#apidoc.element.lunr.stopWordFilter)
1.  [function <span class="apidocSignatureSpan">lunr.</span>tokenizer (obj)](#apidoc.element.lunr.tokenizer)
1.  [function <span class="apidocSignatureSpan">lunr.</span>trimmer (token)](#apidoc.element.lunr.trimmer)
1.  object <span class="apidocSignatureSpan">lunr.</span>EventEmitter.prototype
1.  object <span class="apidocSignatureSpan">lunr.</span>Index.prototype
1.  object <span class="apidocSignatureSpan">lunr.</span>Pipeline.prototype
1.  object <span class="apidocSignatureSpan">lunr.</span>Pipeline.registeredFunctions
1.  object <span class="apidocSignatureSpan">lunr.</span>SortedSet.prototype
1.  object <span class="apidocSignatureSpan">lunr.</span>Store.prototype
1.  object <span class="apidocSignatureSpan">lunr.</span>TokenStore.prototype
1.  object <span class="apidocSignatureSpan">lunr.</span>Vector.prototype
1.  object <span class="apidocSignatureSpan">lunr.</span>tokenizer.registeredFunctions
1.  object <span class="apidocSignatureSpan">lunr.</span>utils
1.  string <span class="apidocSignatureSpan">lunr.</span>version

#### [module lunr.EventEmitter](#apidoc.module.lunr.EventEmitter)
1.  [function <span class="apidocSignatureSpan">lunr.</span>EventEmitter ()](#apidoc.element.lunr.EventEmitter.EventEmitter)

#### [module lunr.EventEmitter.prototype](#apidoc.module.lunr.EventEmitter.prototype)
1.  [function <span class="apidocSignatureSpan">lunr.EventEmitter.prototype.</span>addListener ()](#apidoc.element.lunr.EventEmitter.prototype.addListener)
1.  [function <span class="apidocSignatureSpan">lunr.EventEmitter.prototype.</span>emit (name)](#apidoc.element.lunr.EventEmitter.prototype.emit)
1.  [function <span class="apidocSignatureSpan">lunr.EventEmitter.prototype.</span>hasHandler (name)](#apidoc.element.lunr.EventEmitter.prototype.hasHandler)
1.  [function <span class="apidocSignatureSpan">lunr.EventEmitter.prototype.</span>removeListener (name, fn)](#apidoc.element.lunr.EventEmitter.prototype.removeListener)

#### [module lunr.Index](#apidoc.module.lunr.Index)
1.  [function <span class="apidocSignatureSpan">lunr.</span>Index ()](#apidoc.element.lunr.Index.Index)
1.  [function <span class="apidocSignatureSpan">lunr.Index.</span>load (serialisedData)](#apidoc.element.lunr.Index.load)

#### [module lunr.Index.prototype](#apidoc.module.lunr.Index.prototype)
1.  [function <span class="apidocSignatureSpan">lunr.Index.prototype.</span>add (doc, emitEvent)](#apidoc.element.lunr.Index.prototype.add)
1.  [function <span class="apidocSignatureSpan">lunr.Index.prototype.</span>documentVector (documentRef)](#apidoc.element.lunr.Index.prototype.documentVector)
1.  [function <span class="apidocSignatureSpan">lunr.Index.prototype.</span>field (fieldName, opts)](#apidoc.element.lunr.Index.prototype.field)
1.  [function <span class="apidocSignatureSpan">lunr.Index.prototype.</span>idf (term)](#apidoc.element.lunr.Index.prototype.idf)
1.  [function <span class="apidocSignatureSpan">lunr.Index.prototype.</span>off (name, fn)](#apidoc.element.lunr.Index.prototype.off)
1.  [function <span class="apidocSignatureSpan">lunr.Index.prototype.</span>on ()](#apidoc.element.lunr.Index.prototype.on)
1.  [function <span class="apidocSignatureSpan">lunr.Index.prototype.</span>ref (refName)](#apidoc.element.lunr.Index.prototype.ref)
1.  [function <span class="apidocSignatureSpan">lunr.Index.prototype.</span>remove (doc, emitEvent)](#apidoc.element.lunr.Index.prototype.remove)
1.  [function <span class="apidocSignatureSpan">lunr.Index.prototype.</span>search (query)](#apidoc.element.lunr.Index.prototype.search)
1.  [function <span class="apidocSignatureSpan">lunr.Index.prototype.</span>toJSON ()](#apidoc.element.lunr.Index.prototype.toJSON)
1.  [function <span class="apidocSignatureSpan">lunr.Index.prototype.</span>tokenizer (fn)](#apidoc.element.lunr.Index.prototype.tokenizer)
1.  [function <span class="apidocSignatureSpan">lunr.Index.prototype.</span>update (doc, emitEvent)](#apidoc.element.lunr.Index.prototype.update)
1.  [function <span class="apidocSignatureSpan">lunr.Index.prototype.</span>use (plugin)](#apidoc.element.lunr.Index.prototype.use)

#### [module lunr.Pipeline](#apidoc.module.lunr.Pipeline)
1.  [function <span class="apidocSignatureSpan">lunr.</span>Pipeline ()](#apidoc.element.lunr.Pipeline.Pipeline)
1.  [function <span class="apidocSignatureSpan">lunr.Pipeline.</span>load (serialised)](#apidoc.element.lunr.Pipeline.load)
1.  [function <span class="apidocSignatureSpan">lunr.Pipeline.</span>registerFunction (fn, label)](#apidoc.element.lunr.Pipeline.registerFunction)
1.  [function <span class="apidocSignatureSpan">lunr.Pipeline.</span>warnIfFunctionNotRegistered (fn)](#apidoc.element.lunr.Pipeline.warnIfFunctionNotRegistered)
1.  object <span class="apidocSignatureSpan">lunr.Pipeline.</span>registeredFunctions

#### [module lunr.Pipeline.prototype](#apidoc.module.lunr.Pipeline.prototype)
1.  [function <span class="apidocSignatureSpan">lunr.Pipeline.prototype.</span>add ()](#apidoc.element.lunr.Pipeline.prototype.add)
1.  [function <span class="apidocSignatureSpan">lunr.Pipeline.prototype.</span>after (existingFn, newFn)](#apidoc.element.lunr.Pipeline.prototype.after)
1.  [function <span class="apidocSignatureSpan">lunr.Pipeline.prototype.</span>before (existingFn, newFn)](#apidoc.element.lunr.Pipeline.prototype.before)
1.  [function <span class="apidocSignatureSpan">lunr.Pipeline.prototype.</span>remove (fn)](#apidoc.element.lunr.Pipeline.prototype.remove)
1.  [function <span class="apidocSignatureSpan">lunr.Pipeline.prototype.</span>reset ()](#apidoc.element.lunr.Pipeline.prototype.reset)
1.  [function <span class="apidocSignatureSpan">lunr.Pipeline.prototype.</span>run (tokens)](#apidoc.element.lunr.Pipeline.prototype.run)
1.  [function <span class="apidocSignatureSpan">lunr.Pipeline.prototype.</span>toJSON ()](#apidoc.element.lunr.Pipeline.prototype.toJSON)

#### [module lunr.Pipeline.registeredFunctions](#apidoc.module.lunr.Pipeline.registeredFunctions)
1.  [function <span class="apidocSignatureSpan">lunr.Pipeline.registeredFunctions.</span>stemmer (w)](#apidoc.element.lunr.Pipeline.registeredFunctions.stemmer)
1.  [function <span class="apidocSignatureSpan">lunr.Pipeline.registeredFunctions.</span>stopWordFilter (token)](#apidoc.element.lunr.Pipeline.registeredFunctions.stopWordFilter)
1.  [function <span class="apidocSignatureSpan">lunr.Pipeline.registeredFunctions.</span>trimmer (token)](#apidoc.element.lunr.Pipeline.registeredFunctions.trimmer)

#### [module lunr.SortedSet](#apidoc.module.lunr.SortedSet)
1.  [function <span class="apidocSignatureSpan">lunr.</span>SortedSet ()](#apidoc.element.lunr.SortedSet.SortedSet)
1.  [function <span class="apidocSignatureSpan">lunr.SortedSet.</span>load (serialisedData)](#apidoc.element.lunr.SortedSet.load)

#### [module lunr.SortedSet.prototype](#apidoc.module.lunr.SortedSet.prototype)
1.  [function <span class="apidocSignatureSpan">lunr.SortedSet.prototype.</span>add ()](#apidoc.element.lunr.SortedSet.prototype.add)
1.  [function <span class="apidocSignatureSpan">lunr.SortedSet.prototype.</span>clone ()](#apidoc.element.lunr.SortedSet.prototype.clone)
1.  [function <span class="apidocSignatureSpan">lunr.SortedSet.prototype.</span>forEach (fn, ctx)](#apidoc.element.lunr.SortedSet.prototype.forEach)
1.  [function <span class="apidocSignatureSpan">lunr.SortedSet.prototype.</span>indexOf (elem)](#apidoc.element.lunr.SortedSet.prototype.indexOf)
1.  [function <span class="apidocSignatureSpan">lunr.SortedSet.prototype.</span>intersect (otherSet)](#apidoc.element.lunr.SortedSet.prototype.intersect)
1.  [function <span class="apidocSignatureSpan">lunr.SortedSet.prototype.</span>locationFor (elem)](#apidoc.element.lunr.SortedSet.prototype.locationFor)
1.  [function <span class="apidocSignatureSpan">lunr.SortedSet.prototype.</span>map (fn, ctx)](#apidoc.element.lunr.SortedSet.prototype.map)
1.  [function <span class="apidocSignatureSpan">lunr.SortedSet.prototype.</span>toArray ()](#apidoc.element.lunr.SortedSet.prototype.toArray)
1.  [function <span class="apidocSignatureSpan">lunr.SortedSet.prototype.</span>toJSON ()](#apidoc.element.lunr.SortedSet.prototype.toJSON)
1.  [function <span class="apidocSignatureSpan">lunr.SortedSet.prototype.</span>union (otherSet)](#apidoc.element.lunr.SortedSet.prototype.union)

#### [module lunr.Store](#apidoc.module.lunr.Store)
1.  [function <span class="apidocSignatureSpan">lunr.</span>Store ()](#apidoc.element.lunr.Store.Store)
1.  [function <span class="apidocSignatureSpan">lunr.Store.</span>load (serialisedData)](#apidoc.element.lunr.Store.load)

#### [module lunr.Store.prototype](#apidoc.module.lunr.Store.prototype)
1.  [function <span class="apidocSignatureSpan">lunr.Store.prototype.</span>get (id)](#apidoc.element.lunr.Store.prototype.get)
1.  [function <span class="apidocSignatureSpan">lunr.Store.prototype.</span>has (id)](#apidoc.element.lunr.Store.prototype.has)
1.  [function <span class="apidocSignatureSpan">lunr.Store.prototype.</span>remove (id)](#apidoc.element.lunr.Store.prototype.remove)
1.  [function <span class="apidocSignatureSpan">lunr.Store.prototype.</span>set (id, tokens)](#apidoc.element.lunr.Store.prototype.set)
1.  [function <span class="apidocSignatureSpan">lunr.Store.prototype.</span>toJSON ()](#apidoc.element.lunr.Store.prototype.toJSON)

#### [module lunr.TokenStore](#apidoc.module.lunr.TokenStore)
1.  [function <span class="apidocSignatureSpan">lunr.</span>TokenStore ()](#apidoc.element.lunr.TokenStore.TokenStore)
1.  [function <span class="apidocSignatureSpan">lunr.TokenStore.</span>load (serialisedData)](#apidoc.element.lunr.TokenStore.load)

#### [module lunr.TokenStore.prototype](#apidoc.module.lunr.TokenStore.prototype)
1.  [function <span class="apidocSignatureSpan">lunr.TokenStore.prototype.</span>add (token, doc, root)](#apidoc.element.lunr.TokenStore.prototype.add)
1.  [function <span class="apidocSignatureSpan">lunr.TokenStore.prototype.</span>count (token, root)](#apidoc.element.lunr.TokenStore.prototype.count)
1.  [function <span class="apidocSignatureSpan">lunr.TokenStore.prototype.</span>expand (token, memo)](#apidoc.element.lunr.TokenStore.prototype.expand)
1.  [function <span class="apidocSignatureSpan">lunr.TokenStore.prototype.</span>get (token, root)](#apidoc.element.lunr.TokenStore.prototype.get)
1.  [function <span class="apidocSignatureSpan">lunr.TokenStore.prototype.</span>getNode (token)](#apidoc.element.lunr.TokenStore.prototype.getNode)
1.  [function <span class="apidocSignatureSpan">lunr.TokenStore.prototype.</span>has (token)](#apidoc.element.lunr.TokenStore.prototype.has)
1.  [function <span class="apidocSignatureSpan">lunr.TokenStore.prototype.</span>remove (token, ref)](#apidoc.element.lunr.TokenStore.prototype.remove)
1.  [function <span class="apidocSignatureSpan">lunr.TokenStore.prototype.</span>toJSON ()](#apidoc.element.lunr.TokenStore.prototype.toJSON)

#### [module lunr.Vector](#apidoc.module.lunr.Vector)
1.  [function <span class="apidocSignatureSpan">lunr.</span>Vector ()](#apidoc.element.lunr.Vector.Vector)
1.  [function <span class="apidocSignatureSpan">lunr.Vector.</span>Node (idx, val, next)](#apidoc.element.lunr.Vector.Node)

#### [module lunr.Vector.prototype](#apidoc.module.lunr.Vector.prototype)
1.  [function <span class="apidocSignatureSpan">lunr.Vector.prototype.</span>dot (otherVector)](#apidoc.element.lunr.Vector.prototype.dot)
1.  [function <span class="apidocSignatureSpan">lunr.Vector.prototype.</span>insert (idx, val)](#apidoc.element.lunr.Vector.prototype.insert)
1.  [function <span class="apidocSignatureSpan">lunr.Vector.prototype.</span>magnitude ()](#apidoc.element.lunr.Vector.prototype.magnitude)
1.  [function <span class="apidocSignatureSpan">lunr.Vector.prototype.</span>similarity (otherVector)](#apidoc.element.lunr.Vector.prototype.similarity)

#### [module lunr.tokenizer](#apidoc.module.lunr.tokenizer)
1.  [function <span class="apidocSignatureSpan">lunr.</span>tokenizer (obj)](#apidoc.element.lunr.tokenizer.tokenizer)
1.  [function <span class="apidocSignatureSpan">lunr.tokenizer.</span>load (label)](#apidoc.element.lunr.tokenizer.load)
1.  [function <span class="apidocSignatureSpan">lunr.tokenizer.</span>registerFunction (fn, label)](#apidoc.element.lunr.tokenizer.registerFunction)
1.  object <span class="apidocSignatureSpan">lunr.tokenizer.</span>registeredFunctions
1.  object <span class="apidocSignatureSpan">lunr.tokenizer.</span>separator
1.  string <span class="apidocSignatureSpan">lunr.tokenizer.</span>label

#### [module lunr.tokenizer.registeredFunctions](#apidoc.module.lunr.tokenizer.registeredFunctions)
1.  [function <span class="apidocSignatureSpan">lunr.tokenizer.registeredFunctions.</span>default (obj)](#apidoc.element.lunr.tokenizer.registeredFunctions.default)

#### [module lunr.utils](#apidoc.module.lunr.utils)
1.  [function <span class="apidocSignatureSpan">lunr.utils.</span>asString (obj)](#apidoc.element.lunr.utils.asString)
1.  [function <span class="apidocSignatureSpan">lunr.utils.</span>warn (message)](#apidoc.element.lunr.utils.warn)



# <a name="apidoc.module.lunr"></a>[module lunr](#apidoc.module.lunr)

#### <a name="apidoc.element.lunr.EventEmitter"></a>[function <span class="apidocSignatureSpan">lunr.</span>EventEmitter ()](#apidoc.element.lunr.EventEmitter)
- description and source-code
```javascript
EventEmitter = function () {
  this.events = {}
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.lunr.Index"></a>[function <span class="apidocSignatureSpan">lunr.</span>Index ()](#apidoc.element.lunr.Index)
- description and source-code
```javascript
Index = function () {
  this._fields = []
  this._ref = 'id'
  this.pipeline = new lunr.Pipeline
  this.documentStore = new lunr.Store
  this.tokenStore = new lunr.TokenStore
  this.corpusTokens = new lunr.SortedSet
  this.eventEmitter =  new lunr.EventEmitter
  this.tokenizerFn = lunr.tokenizer

  this._idfCache = {}

  this.on('add', 'remove', 'update', (function () {
    this._idfCache = {}
  }).bind(this))
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.lunr.Pipeline"></a>[function <span class="apidocSignatureSpan">lunr.</span>Pipeline ()](#apidoc.element.lunr.Pipeline)
- description and source-code
```javascript
Pipeline = function () {
  this._stack = []
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.lunr.SortedSet"></a>[function <span class="apidocSignatureSpan">lunr.</span>SortedSet ()](#apidoc.element.lunr.SortedSet)
- description and source-code
```javascript
SortedSet = function () {
  this.length = 0
  this.elements = []
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.lunr.Store"></a>[function <span class="apidocSignatureSpan">lunr.</span>Store ()](#apidoc.element.lunr.Store)
- description and source-code
```javascript
Store = function () {
  this.store = {}
  this.length = 0
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.lunr.TokenStore"></a>[function <span class="apidocSignatureSpan">lunr.</span>TokenStore ()](#apidoc.element.lunr.TokenStore)
- description and source-code
```javascript
TokenStore = function () {
  this.root = { docs: {} }
  this.length = 0
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.lunr.Vector"></a>[function <span class="apidocSignatureSpan">lunr.</span>Vector ()](#apidoc.element.lunr.Vector)
- description and source-code
```javascript
Vector = function () {
  this._magnitude = null
  this.list = undefined
  this.length = 0
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.lunr.generateStopWordFilter"></a>[function <span class="apidocSignatureSpan">lunr.</span>generateStopWordFilter (stopWords)](#apidoc.element.lunr.generateStopWordFilter)
- description and source-code
```javascript
generateStopWordFilter = function (stopWords) {
  var words = stopWords.reduce(function (memo, stopWord) {
    memo[stopWord] = stopWord
    return memo
  }, {})

  return function (token) {
    if (token && words[token] !== token) return token
  }
}
```
- example usage
```shell
...
 * filter then undefined will be returned.
 *
 * @module
 * @param {String} token The token to pass through the filter
 * @returns {String}
 * @see lunr.Pipeline
 */
lunr.stopWordFilter = lunr.generateStopWordFilter([
'a',
'able',
'about',
'across',
'after',
'all',
'almost',
...
```

#### <a name="apidoc.element.lunr.stemmer"></a>[function <span class="apidocSignatureSpan">lunr.</span>stemmer (w)](#apidoc.element.lunr.stemmer)
- description and source-code
```javascript
function porterStemmer(w) {
  var   stem,
    suffix,
    firstch,
    re,
    re2,
    re3,
    re4;

  if (w.length < 3) { return w; }

  firstch = w.substr(0,1);
  if (firstch == "y") {
    w = firstch.toUpperCase() + w.substr(1);
  }

  // Step 1a
  re = re_1a
  re2 = re2_1a;

  if (re.test(w)) { w = w.replace(re,"$1$2"); }
  else if (re2.test(w)) { w = w.replace(re2,"$1$2"); }

  // Step 1b
  re = re_1b;
  re2 = re2_1b;
  if (re.test(w)) {
    var fp = re.exec(w);
    re = re_mgr0;
    if (re.test(fp[1])) {
      re = re_1b_2;
      w = w.replace(re,"");
    }
  } else if (re2.test(w)) {
    var fp = re2.exec(w);
    stem = fp[1];
    re2 = re_s_v;
    if (re2.test(stem)) {
      w = stem;
      re2 = re2_1b_2;
      re3 = re3_1b_2;
      re4 = re4_1b_2;
      if (re2.test(w)) {  w = w + "e"; }
      else if (re3.test(w)) { re = re_1b_2; w = w.replace(re,""); }
      else if (re4.test(w)) { w = w + "e"; }
    }
  }

  // Step 1c - replace suffix y or Y by i if preceded by a non-vowel which is not the first letter of the word (so cry -> cri, by
 -> by, say -> say)
  re = re_1c;
  if (re.test(w)) {
    var fp = re.exec(w);
    stem = fp[1];
    w = stem + "i";
  }

  // Step 2
  re = re_2;
  if (re.test(w)) {
    var fp = re.exec(w);
    stem = fp[1];
    suffix = fp[2];
    re = re_mgr0;
    if (re.test(stem)) {
      w = stem + step2list[suffix];
    }
  }

  // Step 3
  re = re_3;
  if (re.test(w)) {
    var fp = re.exec(w);
    stem = fp[1];
    suffix = fp[2];
    re = re_mgr0;
    if (re.test(stem)) {
      w = stem + step3list[suffix];
    }
  }

  // Step 4
  re = re_4;
  re2 = re2_4;
  if (re.test(w)) {
    var fp = re.exec(w);
    stem = fp[1];
    re = re_mgr1;
    if (re.test(stem)) {
      w = stem;
    }
  } else if (re2.test(w)) {
    var fp = re2.exec(w);
    stem = fp[1] + fp[2];
    re2 = re_mgr1;
    if (re2.test(stem)) {
      w = stem;
    }
  }

  // Step 5
  re = re_5;
  if (re.test(w)) {
    var fp = re.exec(w);
    stem = fp[1];
    re = re_mgr1;
    re2 = re_meq1;
    re3 = re3_5;
    if (re.test(stem) || (re2.test(stem) && !(re3.test(stem)))) {
      w = stem;
    }
  }

  re = re_5_1;
  re2 = re_mgr1;
  if (re.test(w) && re2.test(w)) {
    re = re_1b_2;
    w = w.replace(re,"");
  }

  // and turn initial Y back to y

  if (firstch == "y") {
    w = firstch.toLowerCase() + w.substr(1);
  }

  return w;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.lunr.stopWordFilter"></a>[function <span class="apidocSignatureSpan">lunr.</span>stopWordFilter (token)](#apidoc.element.lunr.stopWordFilter)
- description and source-code
```javascript
stopWordFilter = function (token) {
  if (token && words[token] !== token) return token
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.lunr.tokenizer"></a>[function <span class="apidocSignatureSpan">lunr.</span>tokenizer (obj)](#apidoc.element.lunr.tokenizer)
- description and source-code
```javascript
tokenizer = function (obj) {
  if (!arguments.length || obj == null || obj == undefined) return []
  if (Array.isArray(obj)) return obj.map(function (t) { return lunr.utils.asString(t).toLowerCase() })

  return obj.toString().trim().toLowerCase().split(lunr.tokenizer.separator)
}
```
- example usage
```shell
...
  }

  var idx = new this

  idx._fields = serialisedData.fields
  idx._ref = serialisedData.ref

  idx.tokenizer(lunr.tokenizer.load(serialisedData.tokenizer))
  idx.documentStore = lunr.Store.load(serialisedData.documentStore)
  idx.tokenStore = lunr.TokenStore.load(serialisedData.tokenStore)
  idx.corpusTokens = lunr.SortedSet.load(serialisedData.corpusTokens)
  idx.pipeline = lunr.Pipeline.load(serialisedData.pipeline)

  return idx
}
...
```

#### <a name="apidoc.element.lunr.trimmer"></a>[function <span class="apidocSignatureSpan">lunr.</span>trimmer (token)](#apidoc.element.lunr.trimmer)
- description and source-code
```javascript
trimmer = function (token) {
  return token.replace(/^\W+/, '').replace(/\W+$/, '')
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.lunr.EventEmitter"></a>[module lunr.EventEmitter](#apidoc.module.lunr.EventEmitter)

#### <a name="apidoc.element.lunr.EventEmitter.EventEmitter"></a>[function <span class="apidocSignatureSpan">lunr.</span>EventEmitter ()](#apidoc.element.lunr.EventEmitter.EventEmitter)
- description and source-code
```javascript
EventEmitter = function () {
  this.events = {}
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.lunr.EventEmitter.prototype"></a>[module lunr.EventEmitter.prototype](#apidoc.module.lunr.EventEmitter.prototype)

#### <a name="apidoc.element.lunr.EventEmitter.prototype.addListener"></a>[function <span class="apidocSignatureSpan">lunr.EventEmitter.prototype.</span>addListener ()](#apidoc.element.lunr.EventEmitter.prototype.addListener)
- description and source-code
```javascript
addListener = function () {
  var args = Array.prototype.slice.call(arguments),
      fn = args.pop(),
      names = args

  if (typeof fn !== "function") throw new TypeError ("last argument must be a function")

  names.forEach(function (name) {
    if (!this.hasHandler(name)) this.events[name] = []
    this.events[name].push(fn)
  }, this)
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.lunr.EventEmitter.prototype.emit"></a>[function <span class="apidocSignatureSpan">lunr.EventEmitter.prototype.</span>emit (name)](#apidoc.element.lunr.EventEmitter.prototype.emit)
- description and source-code
```javascript
emit = function (name) {
  if (!this.hasHandler(name)) return

  var args = Array.prototype.slice.call(arguments, 1)

  this.events[name].forEach(function (fn) {
    fn.apply(undefined, args)
  })
}
```
- example usage
```shell
...

     tf += (tokenCount / fieldLength * field.boost)
   }

   this.tokenStore.add(token, { ref: docRef, tf: tf })
 };

 if (emitEvent) this.eventEmitter.emit('add', doc, this)
}

/**
* Removes a document from the index.
*
* To make sure documents no longer show up in search results they can be
* removed from the index using this method.
...
```

#### <a name="apidoc.element.lunr.EventEmitter.prototype.hasHandler"></a>[function <span class="apidocSignatureSpan">lunr.EventEmitter.prototype.</span>hasHandler (name)](#apidoc.element.lunr.EventEmitter.prototype.hasHandler)
- description and source-code
```javascript
hasHandler = function (name) {
  return name in this.events
}
```
- example usage
```shell
...
 var args = Array.prototype.slice.call(arguments),
     fn = args.pop(),
     names = args

 if (typeof fn !== "function") throw new TypeError ("last argument must be a function")

 names.forEach(function (name) {
   if (!this.hasHandler(name)) this.events[name] = []
   this.events[name].push(fn)
 }, this)
}

/**
* Removes a handler function from a specific event.
*
...
```

#### <a name="apidoc.element.lunr.EventEmitter.prototype.removeListener"></a>[function <span class="apidocSignatureSpan">lunr.EventEmitter.prototype.</span>removeListener (name, fn)](#apidoc.element.lunr.EventEmitter.prototype.removeListener)
- description and source-code
```javascript
removeListener = function (name, fn) {
  if (!this.hasHandler(name)) return

  var fnIndex = this.events[name].indexOf(fn)
  this.events[name].splice(fnIndex, 1)

  if (!this.events[name].length) delete this.events[name]
}
```
- example usage
```shell
...
* Removes a handler from an event being emitted by the index.
*
* @param {String} eventName The name of events to remove the function from.
* @param {Function} fn The serialised set to load.
* @memberOf Index
*/
lunr.Index.prototype.off = function (name, fn) {
 return this.eventEmitter.removeListener(name, fn)
}

/**
* Loads a previously serialised index.
*
* Issues a warning if the index being imported was serialised
* by a different version of lunr.
...
```



# <a name="apidoc.module.lunr.Index"></a>[module lunr.Index](#apidoc.module.lunr.Index)

#### <a name="apidoc.element.lunr.Index.Index"></a>[function <span class="apidocSignatureSpan">lunr.</span>Index ()](#apidoc.element.lunr.Index.Index)
- description and source-code
```javascript
Index = function () {
  this._fields = []
  this._ref = 'id'
  this.pipeline = new lunr.Pipeline
  this.documentStore = new lunr.Store
  this.tokenStore = new lunr.TokenStore
  this.corpusTokens = new lunr.SortedSet
  this.eventEmitter =  new lunr.EventEmitter
  this.tokenizerFn = lunr.tokenizer

  this._idfCache = {}

  this.on('add', 'remove', 'update', (function () {
    this._idfCache = {}
  }).bind(this))
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.lunr.Index.load"></a>[function <span class="apidocSignatureSpan">lunr.Index.</span>load (serialisedData)](#apidoc.element.lunr.Index.load)
- description and source-code
```javascript
load = function (serialisedData) {
  if (serialisedData.version !== lunr.version) {
    lunr.utils.warn('version mismatch: current ' + lunr.version + ' importing ' + serialisedData.version)
  }

  var idx = new this

  idx._fields = serialisedData.fields
  idx._ref = serialisedData.ref

  idx.tokenizer(lunr.tokenizer.load(serialisedData.tokenizer))
  idx.documentStore = lunr.Store.load(serialisedData.documentStore)
  idx.tokenStore = lunr.TokenStore.load(serialisedData.tokenStore)
  idx.corpusTokens = lunr.SortedSet.load(serialisedData.corpusTokens)
  idx.pipeline = lunr.Pipeline.load(serialisedData.pipeline)

  return idx
}
```
- example usage
```shell
...
  }

  var idx = new this

  idx._fields = serialisedData.fields
  idx._ref = serialisedData.ref

  idx.tokenizer(lunr.tokenizer.load(serialisedData.tokenizer))
  idx.documentStore = lunr.Store.load(serialisedData.documentStore)
  idx.tokenStore = lunr.TokenStore.load(serialisedData.tokenStore)
  idx.corpusTokens = lunr.SortedSet.load(serialisedData.corpusTokens)
  idx.pipeline = lunr.Pipeline.load(serialisedData.pipeline)

  return idx
}
...
```



# <a name="apidoc.module.lunr.Index.prototype"></a>[module lunr.Index.prototype](#apidoc.module.lunr.Index.prototype)

#### <a name="apidoc.element.lunr.Index.prototype.add"></a>[function <span class="apidocSignatureSpan">lunr.Index.prototype.</span>add (doc, emitEvent)](#apidoc.element.lunr.Index.prototype.add)
- description and source-code
```javascript
add = function (doc, emitEvent) {
  var docTokens = {},
      allDocumentTokens = new lunr.SortedSet,
      docRef = doc[this._ref],
      emitEvent = emitEvent === undefined ? true : emitEvent

  this._fields.forEach(function (field) {
    var fieldTokens = this.pipeline.run(this.tokenizerFn(doc[field.name]))

    docTokens[field.name] = fieldTokens

    for (var i = 0; i < fieldTokens.length; i++) {
      var token = fieldTokens[i]
      allDocumentTokens.add(token)
      this.corpusTokens.add(token)
    }
  }, this)

  this.documentStore.set(docRef, allDocumentTokens)

  for (var i = 0; i < allDocumentTokens.length; i++) {
    var token = allDocumentTokens.elements[i]
    var tf = 0;

    for (var j = 0; j < this._fields.length; j++){
      var field = this._fields[j]
      var fieldTokens = docTokens[field.name]
      var fieldLength = fieldTokens.length

      if (!fieldLength) continue

      var tokenCount = 0
      for (var k = 0; k < fieldLength; k++){
        if (fieldTokens[k] === token){
          tokenCount++
        }
      }

      tf += (tokenCount / fieldLength * field.boost)
    }

    this.tokenStore.add(token, { ref: docRef, tf: tf })
  };

  if (emitEvent) this.eventEmitter.emit('add', doc, this)
}
```
- example usage
```shell
...
'''javascript
var doc = {
    "title": "Twelfth-Night",
    "body": "If music be the food of love, play on: Give me excess of it…",
    "author": "William Shakespeare",
    "id": 1
}
idx.add(doc)
'''

Then searching is as simple:

'''javascript
idx.search("love")
'''
...
```

#### <a name="apidoc.element.lunr.Index.prototype.documentVector"></a>[function <span class="apidocSignatureSpan">lunr.Index.prototype.</span>documentVector (documentRef)](#apidoc.element.lunr.Index.prototype.documentVector)
- description and source-code
```javascript
documentVector = function (documentRef) {
  var documentTokens = this.documentStore.get(documentRef),
      documentTokensLength = documentTokens.length,
      documentVector = new lunr.Vector

  for (var i = 0; i < documentTokensLength; i++) {
    var token = documentTokens.elements[i],
        tf = this.tokenStore.get(token)[documentRef].tf,
        idf = this.idf(token)

    documentVector.insert(this.corpusTokens.indexOf(token), tf * idf)
  };

  return documentVector
}
```
- example usage
```shell
...

  var documentSet = documentSets.reduce(function (memo, set) {
    return memo.intersect(set)
  })

  return documentSet
    .map(function (ref) {
      return { ref: ref, score: queryVector.similarity(this.documentVector(ref)) }
    }, this)
    .sort(function (a, b) {
      return b.score - a.score
    })
}

/**
...
```

#### <a name="apidoc.element.lunr.Index.prototype.field"></a>[function <span class="apidocSignatureSpan">lunr.Index.prototype.</span>field (fieldName, opts)](#apidoc.element.lunr.Index.prototype.field)
- description and source-code
```javascript
field = function (fieldName, opts) {
  var opts = opts || {},
      field = { name: fieldName, boost: opts.boost || 1 }

  this._fields.push(field)
  return this
}
```
- example usage
```shell
...

## Example

A very simple search index can be created using the following:

'''javascript
var idx = lunr(function () {
    this.field('title', { boost: 10 })
    this.field('body')
})
'''

Adding documents to be indexed is as simple as:

'''javascript
...
```

#### <a name="apidoc.element.lunr.Index.prototype.idf"></a>[function <span class="apidocSignatureSpan">lunr.Index.prototype.</span>idf (term)](#apidoc.element.lunr.Index.prototype.idf)
- description and source-code
```javascript
idf = function (term) {
  var cacheKey = "@" + term
  if (Object.prototype.hasOwnProperty.call(this._idfCache, cacheKey)) return this._idfCache[cacheKey]

  var documentFrequency = this.tokenStore.count(term),
      idf = 1

  if (documentFrequency > 0) {
    idf = 1 + Math.log(this.documentStore.length / documentFrequency)
  }

  return this._idfCache[cacheKey] = idf
}
```
- example usage
```shell
...
  queryTokens
    .forEach(function (token, i, tokens) {
      var tf = 1 / tokens.length * this._fields.length * fieldBoosts,
  self = this

      var set = this.tokenStore.expand(token).reduce(function (memo, key) {
var pos = self.corpusTokens.indexOf(key),
    idf = self.idf(key),
    similarityBoost = 1,
    set = new lunr.SortedSet

// if the expanded key is not an exact match to the token then
// penalise the score for this key by how different the key is
// to the token.
if (key !== token) {
...
```

#### <a name="apidoc.element.lunr.Index.prototype.off"></a>[function <span class="apidocSignatureSpan">lunr.Index.prototype.</span>off (name, fn)](#apidoc.element.lunr.Index.prototype.off)
- description and source-code
```javascript
off = function (name, fn) {
  return this.eventEmitter.removeListener(name, fn)
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.lunr.Index.prototype.on"></a>[function <span class="apidocSignatureSpan">lunr.Index.prototype.</span>on ()](#apidoc.element.lunr.Index.prototype.on)
- description and source-code
```javascript
on = function () {
  var args = Array.prototype.slice.call(arguments)
  return this.eventEmitter.addListener.apply(this.eventEmitter, args)
}
```
- example usage
```shell
...
 this.tokenStore = new lunr.TokenStore
 this.corpusTokens = new lunr.SortedSet
 this.eventEmitter =  new lunr.EventEmitter
 this.tokenizerFn = lunr.tokenizer

 this._idfCache = {}

 this.on('add', 'remove', 'update', (function () {
   this._idfCache = {}
 }).bind(this))
}

/**
* Bind a handler to events being emitted by the index.
*
...
```

#### <a name="apidoc.element.lunr.Index.prototype.ref"></a>[function <span class="apidocSignatureSpan">lunr.Index.prototype.</span>ref (refName)](#apidoc.element.lunr.Index.prototype.ref)
- description and source-code
```javascript
ref = function (refName) {
  this._ref = refName
  return this
}
```
- example usage
```shell
...
* Example:
*
*     var idx = lunr(function () {
*       this.field('title', 10)
*       this.field('tags', 100)
*       this.field('body')
*
*       this.ref('cid')
*
*       this.pipeline.add(function () {
*         // some custom pipeline function
*       })
*
*     })
*
...
```

#### <a name="apidoc.element.lunr.Index.prototype.remove"></a>[function <span class="apidocSignatureSpan">lunr.Index.prototype.</span>remove (doc, emitEvent)](#apidoc.element.lunr.Index.prototype.remove)
- description and source-code
```javascript
remove = function (doc, emitEvent) {
  var docRef = doc[this._ref],
      emitEvent = emitEvent === undefined ? true : emitEvent

  if (!this.documentStore.has(docRef)) return

  var docTokens = this.documentStore.get(docRef)

  this.documentStore.remove(docRef)

  docTokens.forEach(function (token) {
    this.tokenStore.remove(token, docRef)
  }, this)

  if (emitEvent) this.eventEmitter.emit('remove', doc, this)
}
```
- example usage
```shell
...
  var docRef = doc[this._ref],
      emitEvent = emitEvent === undefined ? true : emitEvent

  if (!this.documentStore.has(docRef)) return

  var docTokens = this.documentStore.get(docRef)

  this.documentStore.remove(docRef)

  docTokens.forEach(function (token) {
    this.tokenStore.remove(token, docRef)
  }, this)

  if (emitEvent) this.eventEmitter.emit('remove', doc, this)
}
...
```

#### <a name="apidoc.element.lunr.Index.prototype.search"></a>[function <span class="apidocSignatureSpan">lunr.Index.prototype.</span>search (query)](#apidoc.element.lunr.Index.prototype.search)
- description and source-code
```javascript
search = function (query) {
  var queryTokens = this.pipeline.run(this.tokenizerFn(query)),
      queryVector = new lunr.Vector,
      documentSets = [],
      fieldBoosts = this._fields.reduce(function (memo, f) { return memo + f.boost }, 0)

  var hasSomeToken = queryTokens.some(function (token) {
    return this.tokenStore.has(token)
  }, this)

  if (!hasSomeToken) return []

  queryTokens
    .forEach(function (token, i, tokens) {
      var tf = 1 / tokens.length * this._fields.length * fieldBoosts,
          self = this

      var set = this.tokenStore.expand(token).reduce(function (memo, key) {
        var pos = self.corpusTokens.indexOf(key),
            idf = self.idf(key),
            similarityBoost = 1,
            set = new lunr.SortedSet

        // if the expanded key is not an exact match to the token then
        // penalise the score for this key by how different the key is
        // to the token.
        if (key !== token) {
          var diff = Math.max(3, key.length - token.length)
          similarityBoost = 1 / Math.log(diff)
        }

        // calculate the query tf-idf score for this token
        // applying an similarityBoost to ensure exact matches
        // these rank higher than expanded terms
        if (pos > -1) queryVector.insert(pos, tf * idf * similarityBoost)

        // add all the documents that have this key into a set
        // ensuring that the type of key is preserved
        var matchingDocuments = self.tokenStore.get(key),
            refs = Object.keys(matchingDocuments),
            refsLen = refs.length

        for (var i = 0; i < refsLen; i++) {
          set.add(matchingDocuments[refs[i]].ref)
        }

        return memo.union(set)
      }, new lunr.SortedSet)

      documentSets.push(set)
    }, this)

  var documentSet = documentSets.reduce(function (memo, set) {
    return memo.intersect(set)
  })

  return documentSet
    .map(function (ref) {
      return { ref: ref, score: queryVector.similarity(this.documentVector(ref)) }
    }, this)
    .sort(function (a, b) {
      return b.score - a.score
    })
}
```
- example usage
```shell
...
}
idx.add(doc)
'''

Then searching is as simple:

'''javascript
idx.search("love")
'''

This returns a list of matching documents with a score of how closely they match the search query:

'''javascript
[{
"ref": 1,
...
```

#### <a name="apidoc.element.lunr.Index.prototype.toJSON"></a>[function <span class="apidocSignatureSpan">lunr.Index.prototype.</span>toJSON ()](#apidoc.element.lunr.Index.prototype.toJSON)
- description and source-code
```javascript
toJSON = function () {
  return {
    version: lunr.version,
    fields: this._fields,
    ref: this._ref,
    tokenizer: this.tokenizerFn.label,
    documentStore: this.documentStore.toJSON(),
    tokenStore: this.tokenStore.toJSON(),
    corpusTokens: this.corpusTokens.toJSON(),
    pipeline: this.pipeline.toJSON()
  }
}
```
- example usage
```shell
...
 */
lunr.Index.prototype.toJSON = function () {
  return {
    version: lunr.version,
    fields: this._fields,
    ref: this._ref,
    tokenizer: this.tokenizerFn.label,
    documentStore: this.documentStore.toJSON(),
    tokenStore: this.tokenStore.toJSON(),
    corpusTokens: this.corpusTokens.toJSON(),
    pipeline: this.pipeline.toJSON()
  }
}

/**
...
```

#### <a name="apidoc.element.lunr.Index.prototype.tokenizer"></a>[function <span class="apidocSignatureSpan">lunr.Index.prototype.</span>tokenizer (fn)](#apidoc.element.lunr.Index.prototype.tokenizer)
- description and source-code
```javascript
tokenizer = function (fn) {
  var isRegistered = fn.label && (fn.label in lunr.tokenizer.registeredFunctions)

  if (!isRegistered) {
    lunr.utils.warn('Function is not a registered tokenizer. This may cause problems when serialising the index')
  }

  this.tokenizerFn = fn
  return this
}
```
- example usage
```shell
...
  }

  var idx = new this

  idx._fields = serialisedData.fields
  idx._ref = serialisedData.ref

  idx.tokenizer(lunr.tokenizer.load(serialisedData.tokenizer))
  idx.documentStore = lunr.Store.load(serialisedData.documentStore)
  idx.tokenStore = lunr.TokenStore.load(serialisedData.tokenStore)
  idx.corpusTokens = lunr.SortedSet.load(serialisedData.corpusTokens)
  idx.pipeline = lunr.Pipeline.load(serialisedData.pipeline)

  return idx
}
...
```

#### <a name="apidoc.element.lunr.Index.prototype.update"></a>[function <span class="apidocSignatureSpan">lunr.Index.prototype.</span>update (doc, emitEvent)](#apidoc.element.lunr.Index.prototype.update)
- description and source-code
```javascript
update = function (doc, emitEvent) {
  var emitEvent = emitEvent === undefined ? true : emitEvent

  this.remove(doc, false)
  this.add(doc, false)

  if (emitEvent) this.eventEmitter.emit('update', doc, this)
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.lunr.Index.prototype.use"></a>[function <span class="apidocSignatureSpan">lunr.Index.prototype.</span>use (plugin)](#apidoc.element.lunr.Index.prototype.use)
- description and source-code
```javascript
use = function (plugin) {
  var args = Array.prototype.slice.call(arguments, 1)
  args.unshift(this)
  plugin.apply(this, args)
}
```
- example usage
```shell
...
 *
 *     var myPlugin = function (idx, arg1, arg2) {
 *       // 'this' is the index to be extended
 *       // apply any extensions etc here.
 *     }
 *
 *     var idx = lunr(function () {
 *       this.use(myPlugin, 'arg1', 'arg2')
 *     })
 *
 * @param {Function} plugin The plugin to apply.
 * @memberOf Index
 */
lunr.Index.prototype.use = function (plugin) {
var args = Array.prototype.slice.call(arguments, 1)
...
```



# <a name="apidoc.module.lunr.Pipeline"></a>[module lunr.Pipeline](#apidoc.module.lunr.Pipeline)

#### <a name="apidoc.element.lunr.Pipeline.Pipeline"></a>[function <span class="apidocSignatureSpan">lunr.</span>Pipeline ()](#apidoc.element.lunr.Pipeline.Pipeline)
- description and source-code
```javascript
Pipeline = function () {
  this._stack = []
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.lunr.Pipeline.load"></a>[function <span class="apidocSignatureSpan">lunr.Pipeline.</span>load (serialised)](#apidoc.element.lunr.Pipeline.load)
- description and source-code
```javascript
load = function (serialised) {
  var pipeline = new lunr.Pipeline

  serialised.forEach(function (fnName) {
    var fn = lunr.Pipeline.registeredFunctions[fnName]

    if (fn) {
      pipeline.add(fn)
    } else {
      throw new Error('Cannot load un-registered function: ' + fnName)
    }
  })

  return pipeline
}
```
- example usage
```shell
...
  }

  var idx = new this

  idx._fields = serialisedData.fields
  idx._ref = serialisedData.ref

  idx.tokenizer(lunr.tokenizer.load(serialisedData.tokenizer))
  idx.documentStore = lunr.Store.load(serialisedData.documentStore)
  idx.tokenStore = lunr.TokenStore.load(serialisedData.tokenStore)
  idx.corpusTokens = lunr.SortedSet.load(serialisedData.corpusTokens)
  idx.pipeline = lunr.Pipeline.load(serialisedData.pipeline)

  return idx
}
...
```

#### <a name="apidoc.element.lunr.Pipeline.registerFunction"></a>[function <span class="apidocSignatureSpan">lunr.Pipeline.</span>registerFunction (fn, label)](#apidoc.element.lunr.Pipeline.registerFunction)
- description and source-code
```javascript
registerFunction = function (fn, label) {
  if (label in this.registeredFunctions) {
    lunr.utils.warn('Overwriting existing registered function: ' + label)
  }

  fn.label = label
  lunr.Pipeline.registeredFunctions[fn.label] = fn
}
```
- example usage
```shell
...

   return w;
 };

 return porterStemmer;
})();

lunr.Pipeline.registerFunction(lunr.stemmer, 'stemmer')
/*!
* lunr.stopWordFilter
* Copyright (C) 2017 Oliver Nightingale
*/

/**
* lunr.generateStopWordFilter builds a stopWordFilter function from the provided
...
```

#### <a name="apidoc.element.lunr.Pipeline.warnIfFunctionNotRegistered"></a>[function <span class="apidocSignatureSpan">lunr.Pipeline.</span>warnIfFunctionNotRegistered (fn)](#apidoc.element.lunr.Pipeline.warnIfFunctionNotRegistered)
- description and source-code
```javascript
warnIfFunctionNotRegistered = function (fn) {
  var isRegistered = fn.label && (fn.label in this.registeredFunctions)

  if (!isRegistered) {
    lunr.utils.warn('Function is not registered with pipeline. This may cause problems when serialising the index.\n', fn)
  }
}
```
- example usage
```shell
...
* @param {Function} functions Any number of functions to add to the pipeline.
* @memberOf Pipeline
*/
lunr.Pipeline.prototype.add = function () {
 var fns = Array.prototype.slice.call(arguments)

 fns.forEach(function (fn) {
   lunr.Pipeline.warnIfFunctionNotRegistered(fn)
   this._stack.push(fn)
 }, this)
}

/**
* Adds a single function after a function that already exists in the
* pipeline.
...
```



# <a name="apidoc.module.lunr.Pipeline.prototype"></a>[module lunr.Pipeline.prototype](#apidoc.module.lunr.Pipeline.prototype)

#### <a name="apidoc.element.lunr.Pipeline.prototype.add"></a>[function <span class="apidocSignatureSpan">lunr.Pipeline.prototype.</span>add ()](#apidoc.element.lunr.Pipeline.prototype.add)
- description and source-code
```javascript
add = function () {
  var fns = Array.prototype.slice.call(arguments)

  fns.forEach(function (fn) {
    lunr.Pipeline.warnIfFunctionNotRegistered(fn)
    this._stack.push(fn)
  }, this)
}
```
- example usage
```shell
...
'''javascript
var doc = {
    "title": "Twelfth-Night",
    "body": "If music be the food of love, play on: Give me excess of it…",
    "author": "William Shakespeare",
    "id": 1
}
idx.add(doc)
'''

Then searching is as simple:

'''javascript
idx.search("love")
'''
...
```

#### <a name="apidoc.element.lunr.Pipeline.prototype.after"></a>[function <span class="apidocSignatureSpan">lunr.Pipeline.prototype.</span>after (existingFn, newFn)](#apidoc.element.lunr.Pipeline.prototype.after)
- description and source-code
```javascript
after = function (existingFn, newFn) {
  lunr.Pipeline.warnIfFunctionNotRegistered(newFn)

  var pos = this._stack.indexOf(existingFn)
  if (pos == -1) {
    throw new Error('Cannot find existingFn')
  }

  pos = pos + 1
  this._stack.splice(pos, 0, newFn)
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.lunr.Pipeline.prototype.before"></a>[function <span class="apidocSignatureSpan">lunr.Pipeline.prototype.</span>before (existingFn, newFn)](#apidoc.element.lunr.Pipeline.prototype.before)
- description and source-code
```javascript
before = function (existingFn, newFn) {
  lunr.Pipeline.warnIfFunctionNotRegistered(newFn)

  var pos = this._stack.indexOf(existingFn)
  if (pos == -1) {
    throw new Error('Cannot find existingFn')
  }

  this._stack.splice(pos, 0, newFn)
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.lunr.Pipeline.prototype.remove"></a>[function <span class="apidocSignatureSpan">lunr.Pipeline.prototype.</span>remove (fn)](#apidoc.element.lunr.Pipeline.prototype.remove)
- description and source-code
```javascript
remove = function (fn) {
  var pos = this._stack.indexOf(fn)
  if (pos == -1) {
    return
  }

  this._stack.splice(pos, 1)
}
```
- example usage
```shell
...
  var docRef = doc[this._ref],
      emitEvent = emitEvent === undefined ? true : emitEvent

  if (!this.documentStore.has(docRef)) return

  var docTokens = this.documentStore.get(docRef)

  this.documentStore.remove(docRef)

  docTokens.forEach(function (token) {
    this.tokenStore.remove(token, docRef)
  }, this)

  if (emitEvent) this.eventEmitter.emit('remove', doc, this)
}
...
```

#### <a name="apidoc.element.lunr.Pipeline.prototype.reset"></a>[function <span class="apidocSignatureSpan">lunr.Pipeline.prototype.</span>reset ()](#apidoc.element.lunr.Pipeline.prototype.reset)
- description and source-code
```javascript
reset = function () {
  this._stack = []
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.lunr.Pipeline.prototype.run"></a>[function <span class="apidocSignatureSpan">lunr.Pipeline.prototype.</span>run (tokens)](#apidoc.element.lunr.Pipeline.prototype.run)
- description and source-code
```javascript
run = function (tokens) {
  var out = [],
      tokenLength = tokens.length,
      stackLength = this._stack.length

  for (var i = 0; i < tokenLength; i++) {
    var token = tokens[i]

    for (var j = 0; j < stackLength; j++) {
      token = this._stack[j](token, i, tokens)
      if (token === void 0 || token === '') break
    };

    if (token !== void 0 && token !== '') out.push(token)
  };

  return out
}
```
- example usage
```shell
...
lunr.Index.prototype.add = function (doc, emitEvent) {
  var docTokens = {},
  allDocumentTokens = new lunr.SortedSet,
  docRef = doc[this._ref],
  emitEvent = emitEvent === undefined ? true : emitEvent

  this._fields.forEach(function (field) {
var fieldTokens = this.pipeline.run(this.tokenizerFn(doc[field.name]))

docTokens[field.name] = fieldTokens

for (var i = 0; i < fieldTokens.length; i++) {
  var token = fieldTokens[i]
  allDocumentTokens.add(token)
  this.corpusTokens.add(token)
...
```

#### <a name="apidoc.element.lunr.Pipeline.prototype.toJSON"></a>[function <span class="apidocSignatureSpan">lunr.Pipeline.prototype.</span>toJSON ()](#apidoc.element.lunr.Pipeline.prototype.toJSON)
- description and source-code
```javascript
toJSON = function () {
  return this._stack.map(function (fn) {
    lunr.Pipeline.warnIfFunctionNotRegistered(fn)

    return fn.label
  })
}
```
- example usage
```shell
...
 */
lunr.Index.prototype.toJSON = function () {
  return {
    version: lunr.version,
    fields: this._fields,
    ref: this._ref,
    tokenizer: this.tokenizerFn.label,
    documentStore: this.documentStore.toJSON(),
    tokenStore: this.tokenStore.toJSON(),
    corpusTokens: this.corpusTokens.toJSON(),
    pipeline: this.pipeline.toJSON()
  }
}

/**
...
```



# <a name="apidoc.module.lunr.Pipeline.registeredFunctions"></a>[module lunr.Pipeline.registeredFunctions](#apidoc.module.lunr.Pipeline.registeredFunctions)

#### <a name="apidoc.element.lunr.Pipeline.registeredFunctions.stemmer"></a>[function <span class="apidocSignatureSpan">lunr.Pipeline.registeredFunctions.</span>stemmer (w)](#apidoc.element.lunr.Pipeline.registeredFunctions.stemmer)
- description and source-code
```javascript
function porterStemmer(w) {
  var   stem,
    suffix,
    firstch,
    re,
    re2,
    re3,
    re4;

  if (w.length < 3) { return w; }

  firstch = w.substr(0,1);
  if (firstch == "y") {
    w = firstch.toUpperCase() + w.substr(1);
  }

  // Step 1a
  re = re_1a
  re2 = re2_1a;

  if (re.test(w)) { w = w.replace(re,"$1$2"); }
  else if (re2.test(w)) { w = w.replace(re2,"$1$2"); }

  // Step 1b
  re = re_1b;
  re2 = re2_1b;
  if (re.test(w)) {
    var fp = re.exec(w);
    re = re_mgr0;
    if (re.test(fp[1])) {
      re = re_1b_2;
      w = w.replace(re,"");
    }
  } else if (re2.test(w)) {
    var fp = re2.exec(w);
    stem = fp[1];
    re2 = re_s_v;
    if (re2.test(stem)) {
      w = stem;
      re2 = re2_1b_2;
      re3 = re3_1b_2;
      re4 = re4_1b_2;
      if (re2.test(w)) {  w = w + "e"; }
      else if (re3.test(w)) { re = re_1b_2; w = w.replace(re,""); }
      else if (re4.test(w)) { w = w + "e"; }
    }
  }

  // Step 1c - replace suffix y or Y by i if preceded by a non-vowel which is not the first letter of the word (so cry -> cri, by
 -> by, say -> say)
  re = re_1c;
  if (re.test(w)) {
    var fp = re.exec(w);
    stem = fp[1];
    w = stem + "i";
  }

  // Step 2
  re = re_2;
  if (re.test(w)) {
    var fp = re.exec(w);
    stem = fp[1];
    suffix = fp[2];
    re = re_mgr0;
    if (re.test(stem)) {
      w = stem + step2list[suffix];
    }
  }

  // Step 3
  re = re_3;
  if (re.test(w)) {
    var fp = re.exec(w);
    stem = fp[1];
    suffix = fp[2];
    re = re_mgr0;
    if (re.test(stem)) {
      w = stem + step3list[suffix];
    }
  }

  // Step 4
  re = re_4;
  re2 = re2_4;
  if (re.test(w)) {
    var fp = re.exec(w);
    stem = fp[1];
    re = re_mgr1;
    if (re.test(stem)) {
      w = stem;
    }
  } else if (re2.test(w)) {
    var fp = re2.exec(w);
    stem = fp[1] + fp[2];
    re2 = re_mgr1;
    if (re2.test(stem)) {
      w = stem;
    }
  }

  // Step 5
  re = re_5;
  if (re.test(w)) {
    var fp = re.exec(w);
    stem = fp[1];
    re = re_mgr1;
    re2 = re_meq1;
    re3 = re3_5;
    if (re.test(stem) || (re2.test(stem) && !(re3.test(stem)))) {
      w = stem;
    }
  }

  re = re_5_1;
  re2 = re_mgr1;
  if (re.test(w) && re2.test(w)) {
    re = re_1b_2;
    w = w.replace(re,"");
  }

  // and turn initial Y back to y

  if (firstch == "y") {
    w = firstch.toLowerCase() + w.substr(1);
  }

  return w;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.lunr.Pipeline.registeredFunctions.stopWordFilter"></a>[function <span class="apidocSignatureSpan">lunr.Pipeline.registeredFunctions.</span>stopWordFilter (token)](#apidoc.element.lunr.Pipeline.registeredFunctions.stopWordFilter)
- description and source-code
```javascript
stopWordFilter = function (token) {
  if (token && words[token] !== token) return token
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.lunr.Pipeline.registeredFunctions.trimmer"></a>[function <span class="apidocSignatureSpan">lunr.Pipeline.registeredFunctions.</span>trimmer (token)](#apidoc.element.lunr.Pipeline.registeredFunctions.trimmer)
- description and source-code
```javascript
trimmer = function (token) {
  return token.replace(/^\W+/, '').replace(/\W+$/, '')
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.lunr.SortedSet"></a>[module lunr.SortedSet](#apidoc.module.lunr.SortedSet)

#### <a name="apidoc.element.lunr.SortedSet.SortedSet"></a>[function <span class="apidocSignatureSpan">lunr.</span>SortedSet ()](#apidoc.element.lunr.SortedSet.SortedSet)
- description and source-code
```javascript
SortedSet = function () {
  this.length = 0
  this.elements = []
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.lunr.SortedSet.load"></a>[function <span class="apidocSignatureSpan">lunr.SortedSet.</span>load (serialisedData)](#apidoc.element.lunr.SortedSet.load)
- description and source-code
```javascript
load = function (serialisedData) {
  var set = new this

  set.elements = serialisedData
  set.length = serialisedData.length

  return set
}
```
- example usage
```shell
...
  }

  var idx = new this

  idx._fields = serialisedData.fields
  idx._ref = serialisedData.ref

  idx.tokenizer(lunr.tokenizer.load(serialisedData.tokenizer))
  idx.documentStore = lunr.Store.load(serialisedData.documentStore)
  idx.tokenStore = lunr.TokenStore.load(serialisedData.tokenStore)
  idx.corpusTokens = lunr.SortedSet.load(serialisedData.corpusTokens)
  idx.pipeline = lunr.Pipeline.load(serialisedData.pipeline)

  return idx
}
...
```



# <a name="apidoc.module.lunr.SortedSet.prototype"></a>[module lunr.SortedSet.prototype](#apidoc.module.lunr.SortedSet.prototype)

#### <a name="apidoc.element.lunr.SortedSet.prototype.add"></a>[function <span class="apidocSignatureSpan">lunr.SortedSet.prototype.</span>add ()](#apidoc.element.lunr.SortedSet.prototype.add)
- description and source-code
```javascript
add = function () {
  var i, element

  for (i = 0; i < arguments.length; i++) {
    element = arguments[i]
    if (~this.indexOf(element)) continue
    this.elements.splice(this.locationFor(element), 0, element)
  }

  this.length = this.elements.length
}
```
- example usage
```shell
...
'''javascript
var doc = {
    "title": "Twelfth-Night",
    "body": "If music be the food of love, play on: Give me excess of it…",
    "author": "William Shakespeare",
    "id": 1
}
idx.add(doc)
'''

Then searching is as simple:

'''javascript
idx.search("love")
'''
...
```

#### <a name="apidoc.element.lunr.SortedSet.prototype.clone"></a>[function <span class="apidocSignatureSpan">lunr.SortedSet.prototype.</span>clone ()](#apidoc.element.lunr.SortedSet.prototype.clone)
- description and source-code
```javascript
clone = function () {
  var clone = new lunr.SortedSet

  clone.elements = this.toArray()
  clone.length = clone.elements.length

  return clone
}
```
- example usage
```shell
...

  if (this.length >= otherSet.length) {
    longSet = this, shortSet = otherSet
  } else {
    longSet = otherSet, shortSet = this
  }

  unionSet = longSet.clone()

  for(var i = 0, shortSetElements = shortSet.toArray(); i < shortSetElements.length; i++){
    unionSet.add(shortSetElements[i])
  }

  return unionSet
}
...
```

#### <a name="apidoc.element.lunr.SortedSet.prototype.forEach"></a>[function <span class="apidocSignatureSpan">lunr.SortedSet.prototype.</span>forEach (fn, ctx)](#apidoc.element.lunr.SortedSet.prototype.forEach)
- description and source-code
```javascript
forEach = function (fn, ctx) {
  return this.elements.forEach(fn, ctx)
}
```
- example usage
```shell
...
lunr.EventEmitter.prototype.addListener = function () {
 var args = Array.prototype.slice.call(arguments),
     fn = args.pop(),
     names = args

 if (typeof fn !== "function") throw new TypeError ("last argument must be a function")

 names.forEach(function (name) {
   if (!this.hasHandler(name)) this.events[name] = []
   this.events[name].push(fn)
 }, this)
}

/**
* Removes a handler function from a specific event.
...
```

#### <a name="apidoc.element.lunr.SortedSet.prototype.indexOf"></a>[function <span class="apidocSignatureSpan">lunr.SortedSet.prototype.</span>indexOf (elem)](#apidoc.element.lunr.SortedSet.prototype.indexOf)
- description and source-code
```javascript
indexOf = function (elem) {
  var start = 0,
      end = this.elements.length,
      sectionLength = end - start,
      pivot = start + Math.floor(sectionLength / 2),
      pivotElem = this.elements[pivot]

  while (sectionLength > 1) {
    if (pivotElem === elem) return pivot

    if (pivotElem < elem) start = pivot
    if (pivotElem > elem) end = pivot

    sectionLength = end - start
    pivot = start + Math.floor(sectionLength / 2)
    pivotElem = this.elements[pivot]
  }

  if (pivotElem === elem) return pivot

  return -1
}
```
- example usage
```shell
...
* @param {String} eventName The name of the event to remove this function from.
* @param {Function} fn The function to remove from an event.
* @memberOf EventEmitter
*/
lunr.EventEmitter.prototype.removeListener = function (name, fn) {
 if (!this.hasHandler(name)) return

 var fnIndex = this.events[name].indexOf(fn)
 this.events[name].splice(fnIndex, 1)

 if (!this.events[name].length) delete this.events[name]
}

/**
* Calls all functions bound to the given event.
...
```

#### <a name="apidoc.element.lunr.SortedSet.prototype.intersect"></a>[function <span class="apidocSignatureSpan">lunr.SortedSet.prototype.</span>intersect (otherSet)](#apidoc.element.lunr.SortedSet.prototype.intersect)
- description and source-code
```javascript
intersect = function (otherSet) {
  var intersectSet = new lunr.SortedSet,
      i = 0, j = 0,
      a_len = this.length, b_len = otherSet.length,
      a = this.elements, b = otherSet.elements

  while (true) {
    if (i > a_len - 1 || j > b_len - 1) break

    if (a[i] === b[j]) {
      intersectSet.add(a[i])
      i++, j++
      continue
    }

    if (a[i] < b[j]) {
      i++
      continue
    }

    if (a[i] > b[j]) {
      j++
      continue
    }
  };

  return intersectSet
}
```
- example usage
```shell
...
      return memo.union(set)
    }, new lunr.SortedSet)

    documentSets.push(set)
  }, this)

var documentSet = documentSets.reduce(function (memo, set) {
  return memo.intersect(set)
})

return documentSet
  .map(function (ref) {
    return { ref: ref, score: queryVector.similarity(this.documentVector(ref)) }
  }, this)
  .sort(function (a, b) {
...
```

#### <a name="apidoc.element.lunr.SortedSet.prototype.locationFor"></a>[function <span class="apidocSignatureSpan">lunr.SortedSet.prototype.</span>locationFor (elem)](#apidoc.element.lunr.SortedSet.prototype.locationFor)
- description and source-code
```javascript
locationFor = function (elem) {
  var start = 0,
      end = this.elements.length,
      sectionLength = end - start,
      pivot = start + Math.floor(sectionLength / 2),
      pivotElem = this.elements[pivot]

  while (sectionLength > 1) {
    if (pivotElem < elem) start = pivot
    if (pivotElem > elem) end = pivot

    sectionLength = end - start
    pivot = start + Math.floor(sectionLength / 2)
    pivotElem = this.elements[pivot]
  }

  if (pivotElem > elem) return pivot
  if (pivotElem < elem) return pivot + 1
}
```
- example usage
```shell
...
*/
lunr.SortedSet.prototype.add = function () {
 var i, element

 for (i = 0; i < arguments.length; i++) {
   element = arguments[i]
   if (~this.indexOf(element)) continue
   this.elements.splice(this.locationFor(element), 0, element)
 }

 this.length = this.elements.length
}

/**
* Converts this sorted set into an array.
...
```

#### <a name="apidoc.element.lunr.SortedSet.prototype.map"></a>[function <span class="apidocSignatureSpan">lunr.SortedSet.prototype.</span>map (fn, ctx)](#apidoc.element.lunr.SortedSet.prototype.map)
- description and source-code
```javascript
map = function (fn, ctx) {
  return this.elements.map(fn, ctx)
}
```
- example usage
```shell
...
* @module
* @param {String} obj The string to convert into tokens
* @see lunr.tokenizer.separator
* @returns {Array}
*/
lunr.tokenizer = function (obj) {
 if (!arguments.length || obj == null || obj == undefined) return []
 if (Array.isArray(obj)) return obj.map(function (t) { return lunr.utils.asString(t).toLowerCase() })

 return obj.toString().trim().toLowerCase().split(lunr.tokenizer.separator)
}

/**
* The sperator used to split a string into tokens. Override this property to change the behaviour of
* 'lunr.tokenizer' behaviour when tokenizing strings. By default this splits on whitespace and hyphens.
...
```

#### <a name="apidoc.element.lunr.SortedSet.prototype.toArray"></a>[function <span class="apidocSignatureSpan">lunr.SortedSet.prototype.</span>toArray ()](#apidoc.element.lunr.SortedSet.prototype.toArray)
- description and source-code
```javascript
toArray = function () {
  return this.elements.slice()
}
```
- example usage
```shell
...
*
* @returns {lunr.SortedSet}
* @memberOf SortedSet
*/
lunr.SortedSet.prototype.clone = function () {
 var clone = new lunr.SortedSet

 clone.elements = this.toArray()
 clone.length = clone.elements.length

 return clone
}

/**
* Creates a new lunr.SortedSet that contains the elements in the union
...
```

#### <a name="apidoc.element.lunr.SortedSet.prototype.toJSON"></a>[function <span class="apidocSignatureSpan">lunr.SortedSet.prototype.</span>toJSON ()](#apidoc.element.lunr.SortedSet.prototype.toJSON)
- description and source-code
```javascript
toJSON = function () {
  return this.toArray()
}
```
- example usage
```shell
...
 */
lunr.Index.prototype.toJSON = function () {
  return {
    version: lunr.version,
    fields: this._fields,
    ref: this._ref,
    tokenizer: this.tokenizerFn.label,
    documentStore: this.documentStore.toJSON(),
    tokenStore: this.tokenStore.toJSON(),
    corpusTokens: this.corpusTokens.toJSON(),
    pipeline: this.pipeline.toJSON()
  }
}

/**
...
```

#### <a name="apidoc.element.lunr.SortedSet.prototype.union"></a>[function <span class="apidocSignatureSpan">lunr.SortedSet.prototype.</span>union (otherSet)](#apidoc.element.lunr.SortedSet.prototype.union)
- description and source-code
```javascript
union = function (otherSet) {
  var longSet, shortSet, unionSet

  if (this.length >= otherSet.length) {
    longSet = this, shortSet = otherSet
  } else {
    longSet = otherSet, shortSet = this
  }

  unionSet = longSet.clone()

  for(var i = 0, shortSetElements = shortSet.toArray(); i < shortSetElements.length; i++){
    unionSet.add(shortSetElements[i])
  }

  return unionSet
}
```
- example usage
```shell
...
          refs = Object.keys(matchingDocuments),
          refsLen = refs.length

      for (var i = 0; i < refsLen; i++) {
        set.add(matchingDocuments[refs[i]].ref)
      }

      return memo.union(set)
    }, new lunr.SortedSet)

    documentSets.push(set)
  }, this)

var documentSet = documentSets.reduce(function (memo, set) {
  return memo.intersect(set)
...
```



# <a name="apidoc.module.lunr.Store"></a>[module lunr.Store](#apidoc.module.lunr.Store)

#### <a name="apidoc.element.lunr.Store.Store"></a>[function <span class="apidocSignatureSpan">lunr.</span>Store ()](#apidoc.element.lunr.Store.Store)
- description and source-code
```javascript
Store = function () {
  this.store = {}
  this.length = 0
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.lunr.Store.load"></a>[function <span class="apidocSignatureSpan">lunr.Store.</span>load (serialisedData)](#apidoc.element.lunr.Store.load)
- description and source-code
```javascript
load = function (serialisedData) {
  var store = new this

  store.length = serialisedData.length
  store.store = Object.keys(serialisedData.store).reduce(function (memo, key) {
    memo[key] = lunr.SortedSet.load(serialisedData.store[key])
    return memo
  }, {})

  return store
}
```
- example usage
```shell
...
  }

  var idx = new this

  idx._fields = serialisedData.fields
  idx._ref = serialisedData.ref

  idx.tokenizer(lunr.tokenizer.load(serialisedData.tokenizer))
  idx.documentStore = lunr.Store.load(serialisedData.documentStore)
  idx.tokenStore = lunr.TokenStore.load(serialisedData.tokenStore)
  idx.corpusTokens = lunr.SortedSet.load(serialisedData.corpusTokens)
  idx.pipeline = lunr.Pipeline.load(serialisedData.pipeline)

  return idx
}
...
```



# <a name="apidoc.module.lunr.Store.prototype"></a>[module lunr.Store.prototype](#apidoc.module.lunr.Store.prototype)

#### <a name="apidoc.element.lunr.Store.prototype.get"></a>[function <span class="apidocSignatureSpan">lunr.Store.prototype.</span>get (id)](#apidoc.element.lunr.Store.prototype.get)
- description and source-code
```javascript
get = function (id) {
  return this.store[id]
}
```
- example usage
```shell
...
 */
lunr.Index.prototype.remove = function (doc, emitEvent) {
var docRef = doc[this._ref],
    emitEvent = emitEvent === undefined ? true : emitEvent

if (!this.documentStore.has(docRef)) return

var docTokens = this.documentStore.get(docRef)

this.documentStore.remove(docRef)

docTokens.forEach(function (token) {
  this.tokenStore.remove(token, docRef)
}, this)
...
```

#### <a name="apidoc.element.lunr.Store.prototype.has"></a>[function <span class="apidocSignatureSpan">lunr.Store.prototype.</span>has (id)](#apidoc.element.lunr.Store.prototype.has)
- description and source-code
```javascript
has = function (id) {
  return id in this.store
}
```
- example usage
```shell
...
 * @param {Boolean} emitEvent Whether to emit remove events, defaults to true
 * @memberOf Index
 */
lunr.Index.prototype.remove = function (doc, emitEvent) {
var docRef = doc[this._ref],
    emitEvent = emitEvent === undefined ? true : emitEvent

if (!this.documentStore.has(docRef)) return

var docTokens = this.documentStore.get(docRef)

this.documentStore.remove(docRef)

docTokens.forEach(function (token) {
  this.tokenStore.remove(token, docRef)
...
```

#### <a name="apidoc.element.lunr.Store.prototype.remove"></a>[function <span class="apidocSignatureSpan">lunr.Store.prototype.</span>remove (id)](#apidoc.element.lunr.Store.prototype.remove)
- description and source-code
```javascript
remove = function (id) {
  if (!this.has(id)) return

  delete this.store[id]
  this.length--
}
```
- example usage
```shell
...
  var docRef = doc[this._ref],
      emitEvent = emitEvent === undefined ? true : emitEvent

  if (!this.documentStore.has(docRef)) return

  var docTokens = this.documentStore.get(docRef)

  this.documentStore.remove(docRef)

  docTokens.forEach(function (token) {
    this.tokenStore.remove(token, docRef)
  }, this)

  if (emitEvent) this.eventEmitter.emit('remove', doc, this)
}
...
```

#### <a name="apidoc.element.lunr.Store.prototype.set"></a>[function <span class="apidocSignatureSpan">lunr.Store.prototype.</span>set (id, tokens)](#apidoc.element.lunr.Store.prototype.set)
- description and source-code
```javascript
set = function (id, tokens) {
  if (!this.has(id)) this.length++
  this.store[id] = tokens
}
```
- example usage
```shell
...
for (var i = 0; i < fieldTokens.length; i++) {
  var token = fieldTokens[i]
  allDocumentTokens.add(token)
  this.corpusTokens.add(token)
}
  }, this)

  this.documentStore.set(docRef, allDocumentTokens)

  for (var i = 0; i < allDocumentTokens.length; i++) {
var token = allDocumentTokens.elements[i]
var tf = 0;

for (var j = 0; j < this._fields.length; j++){
  var field = this._fields[j]
...
```

#### <a name="apidoc.element.lunr.Store.prototype.toJSON"></a>[function <span class="apidocSignatureSpan">lunr.Store.prototype.</span>toJSON ()](#apidoc.element.lunr.Store.prototype.toJSON)
- description and source-code
```javascript
toJSON = function () {
  return {
    store: this.store,
    length: this.length
  }
}
```
- example usage
```shell
...
 */
lunr.Index.prototype.toJSON = function () {
  return {
    version: lunr.version,
    fields: this._fields,
    ref: this._ref,
    tokenizer: this.tokenizerFn.label,
    documentStore: this.documentStore.toJSON(),
    tokenStore: this.tokenStore.toJSON(),
    corpusTokens: this.corpusTokens.toJSON(),
    pipeline: this.pipeline.toJSON()
  }
}

/**
...
```



# <a name="apidoc.module.lunr.TokenStore"></a>[module lunr.TokenStore](#apidoc.module.lunr.TokenStore)

#### <a name="apidoc.element.lunr.TokenStore.TokenStore"></a>[function <span class="apidocSignatureSpan">lunr.</span>TokenStore ()](#apidoc.element.lunr.TokenStore.TokenStore)
- description and source-code
```javascript
TokenStore = function () {
  this.root = { docs: {} }
  this.length = 0
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.lunr.TokenStore.load"></a>[function <span class="apidocSignatureSpan">lunr.TokenStore.</span>load (serialisedData)](#apidoc.element.lunr.TokenStore.load)
- description and source-code
```javascript
load = function (serialisedData) {
  var store = new this

  store.root = serialisedData.root
  store.length = serialisedData.length

  return store
}
```
- example usage
```shell
...
  }

  var idx = new this

  idx._fields = serialisedData.fields
  idx._ref = serialisedData.ref

  idx.tokenizer(lunr.tokenizer.load(serialisedData.tokenizer))
  idx.documentStore = lunr.Store.load(serialisedData.documentStore)
  idx.tokenStore = lunr.TokenStore.load(serialisedData.tokenStore)
  idx.corpusTokens = lunr.SortedSet.load(serialisedData.corpusTokens)
  idx.pipeline = lunr.Pipeline.load(serialisedData.pipeline)

  return idx
}
...
```



# <a name="apidoc.module.lunr.TokenStore.prototype"></a>[module lunr.TokenStore.prototype](#apidoc.module.lunr.TokenStore.prototype)

#### <a name="apidoc.element.lunr.TokenStore.prototype.add"></a>[function <span class="apidocSignatureSpan">lunr.TokenStore.prototype.</span>add (token, doc, root)](#apidoc.element.lunr.TokenStore.prototype.add)
- description and source-code
```javascript
add = function (token, doc, root) {
  var root = root || this.root,
      key = token.charAt(0),
      rest = token.slice(1)

  if (!(key in root)) root[key] = {docs: {}}

  if (rest.length === 0) {
    root[key].docs[doc.ref] = doc
    this.length += 1
    return
  } else {
    return this.add(rest, doc, root[key])
  }
}
```
- example usage
```shell
...
'''javascript
var doc = {
    "title": "Twelfth-Night",
    "body": "If music be the food of love, play on: Give me excess of it…",
    "author": "William Shakespeare",
    "id": 1
}
idx.add(doc)
'''

Then searching is as simple:

'''javascript
idx.search("love")
'''
...
```

#### <a name="apidoc.element.lunr.TokenStore.prototype.count"></a>[function <span class="apidocSignatureSpan">lunr.TokenStore.prototype.</span>count (token, root)](#apidoc.element.lunr.TokenStore.prototype.count)
- description and source-code
```javascript
count = function (token, root) {
  return Object.keys(this.get(token, root)).length
}
```
- example usage
```shell
...
 * @private
 * @memberOf Index
 */
lunr.Index.prototype.idf = function (term) {
var cacheKey = "@" + term
if (Object.prototype.hasOwnProperty.call(this._idfCache, cacheKey)) return this._idfCache[cacheKey]

var documentFrequency = this.tokenStore.count(term),
    idf = 1

if (documentFrequency > 0) {
  idf = 1 + Math.log(this.documentStore.length / documentFrequency)
}

return this._idfCache[cacheKey] = idf
...
```

#### <a name="apidoc.element.lunr.TokenStore.prototype.expand"></a>[function <span class="apidocSignatureSpan">lunr.TokenStore.prototype.</span>expand (token, memo)](#apidoc.element.lunr.TokenStore.prototype.expand)
- description and source-code
```javascript
expand = function (token, memo) {
  var root = this.getNode(token),
      docs = root.docs || {},
      memo = memo || []

  if (Object.keys(docs).length) memo.push(token)

  Object.keys(root)
    .forEach(function (key) {
      if (key === 'docs') return

      memo.concat(this.expand(token + key, memo))
    }, this)

  return memo
}
```
- example usage
```shell
...
  if (!hasSomeToken) return []

  queryTokens
    .forEach(function (token, i, tokens) {
      var tf = 1 / tokens.length * this._fields.length * fieldBoosts,
  self = this

      var set = this.tokenStore.expand(token).reduce(function (memo, key) {
var pos = self.corpusTokens.indexOf(key),
    idf = self.idf(key),
    similarityBoost = 1,
    set = new lunr.SortedSet

// if the expanded key is not an exact match to the token then
// penalise the score for this key by how different the key is
...
```

#### <a name="apidoc.element.lunr.TokenStore.prototype.get"></a>[function <span class="apidocSignatureSpan">lunr.TokenStore.prototype.</span>get (token, root)](#apidoc.element.lunr.TokenStore.prototype.get)
- description and source-code
```javascript
get = function (token, root) {
  return this.getNode(token, root).docs || {}
}
```
- example usage
```shell
...
 */
lunr.Index.prototype.remove = function (doc, emitEvent) {
var docRef = doc[this._ref],
    emitEvent = emitEvent === undefined ? true : emitEvent

if (!this.documentStore.has(docRef)) return

var docTokens = this.documentStore.get(docRef)

this.documentStore.remove(docRef)

docTokens.forEach(function (token) {
  this.tokenStore.remove(token, docRef)
}, this)
...
```

#### <a name="apidoc.element.lunr.TokenStore.prototype.getNode"></a>[function <span class="apidocSignatureSpan">lunr.TokenStore.prototype.</span>getNode (token)](#apidoc.element.lunr.TokenStore.prototype.getNode)
- description and source-code
```javascript
getNode = function (token) {
  if (!token) return {}

  var node = this.root

  for (var i = 0; i < token.length; i++) {
    if (!node[token.charAt(i)]) return {}

    node = node[token.charAt(i)]
  }

  return node
}
```
- example usage
```shell
...
 *
 * @param {String} token The token to get the documents for.
 * @param {Object} root An optional node at which to start.
 * @returns {Object}
 * @memberOf TokenStore
 */
lunr.TokenStore.prototype.get = function (token, root) {
  return this.getNode(token, root).docs || {}
}

lunr.TokenStore.prototype.count = function (token, root) {
  return Object.keys(this.get(token, root)).length
}

/**
...
```

#### <a name="apidoc.element.lunr.TokenStore.prototype.has"></a>[function <span class="apidocSignatureSpan">lunr.TokenStore.prototype.</span>has (token)](#apidoc.element.lunr.TokenStore.prototype.has)
- description and source-code
```javascript
has = function (token) {
  if (!token) return false

  var node = this.root

  for (var i = 0; i < token.length; i++) {
    if (!node[token.charAt(i)]) return false

    node = node[token.charAt(i)]
  }

  return true
}
```
- example usage
```shell
...
 * @param {Boolean} emitEvent Whether to emit remove events, defaults to true
 * @memberOf Index
 */
lunr.Index.prototype.remove = function (doc, emitEvent) {
var docRef = doc[this._ref],
    emitEvent = emitEvent === undefined ? true : emitEvent

if (!this.documentStore.has(docRef)) return

var docTokens = this.documentStore.get(docRef)

this.documentStore.remove(docRef)

docTokens.forEach(function (token) {
  this.tokenStore.remove(token, docRef)
...
```

#### <a name="apidoc.element.lunr.TokenStore.prototype.remove"></a>[function <span class="apidocSignatureSpan">lunr.TokenStore.prototype.</span>remove (token, ref)](#apidoc.element.lunr.TokenStore.prototype.remove)
- description and source-code
```javascript
remove = function (token, ref) {
  if (!token) return
  var node = this.root

  for (var i = 0; i < token.length; i++) {
    if (!(token.charAt(i) in node)) return
    node = node[token.charAt(i)]
  }

  delete node.docs[ref]
}
```
- example usage
```shell
...
  var docRef = doc[this._ref],
      emitEvent = emitEvent === undefined ? true : emitEvent

  if (!this.documentStore.has(docRef)) return

  var docTokens = this.documentStore.get(docRef)

  this.documentStore.remove(docRef)

  docTokens.forEach(function (token) {
    this.tokenStore.remove(token, docRef)
  }, this)

  if (emitEvent) this.eventEmitter.emit('remove', doc, this)
}
...
```

#### <a name="apidoc.element.lunr.TokenStore.prototype.toJSON"></a>[function <span class="apidocSignatureSpan">lunr.TokenStore.prototype.</span>toJSON ()](#apidoc.element.lunr.TokenStore.prototype.toJSON)
- description and source-code
```javascript
toJSON = function () {
  return {
    root: this.root,
    length: this.length
  }
}
```
- example usage
```shell
...
 */
lunr.Index.prototype.toJSON = function () {
  return {
    version: lunr.version,
    fields: this._fields,
    ref: this._ref,
    tokenizer: this.tokenizerFn.label,
    documentStore: this.documentStore.toJSON(),
    tokenStore: this.tokenStore.toJSON(),
    corpusTokens: this.corpusTokens.toJSON(),
    pipeline: this.pipeline.toJSON()
  }
}

/**
...
```



# <a name="apidoc.module.lunr.Vector"></a>[module lunr.Vector](#apidoc.module.lunr.Vector)

#### <a name="apidoc.element.lunr.Vector.Vector"></a>[function <span class="apidocSignatureSpan">lunr.</span>Vector ()](#apidoc.element.lunr.Vector.Vector)
- description and source-code
```javascript
Vector = function () {
  this._magnitude = null
  this.list = undefined
  this.length = 0
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.lunr.Vector.Node"></a>[function <span class="apidocSignatureSpan">lunr.Vector.</span>Node (idx, val, next)](#apidoc.element.lunr.Vector.Node)
- description and source-code
```javascript
Node = function (idx, val, next) {
  this.idx = idx
  this.val = val
  this.next = next
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.lunr.Vector.prototype"></a>[module lunr.Vector.prototype](#apidoc.module.lunr.Vector.prototype)

#### <a name="apidoc.element.lunr.Vector.prototype.dot"></a>[function <span class="apidocSignatureSpan">lunr.Vector.prototype.</span>dot (otherVector)](#apidoc.element.lunr.Vector.prototype.dot)
- description and source-code
```javascript
dot = function (otherVector) {
  var node = this.list,
      otherNode = otherVector.list,
      dotProduct = 0

  while (node && otherNode) {
    if (node.idx < otherNode.idx) {
      node = node.next
    } else if (node.idx > otherNode.idx) {
      otherNode = otherNode.next
    } else {
      dotProduct += node.val * otherNode.val
      node = node.next
      otherNode = otherNode.next
    }
  }

  return dotProduct
}
```
- example usage
```shell
...
 *
 * @param {lunr.Vector} otherVector The other vector to calculate the
 * similarity with.
 * @returns {Number}
 * @memberOf Vector
 */
lunr.Vector.prototype.similarity = function (otherVector) {
  return this.dot(otherVector) / (this.magnitude() * otherVector.magnitude())
}
/*!
 * lunr.SortedSet
 * Copyright (C) 2017 Oliver Nightingale
 */

/**
...
```

#### <a name="apidoc.element.lunr.Vector.prototype.insert"></a>[function <span class="apidocSignatureSpan">lunr.Vector.prototype.</span>insert (idx, val)](#apidoc.element.lunr.Vector.prototype.insert)
- description and source-code
```javascript
insert = function (idx, val) {
  this._magnitude = undefined;
  var list = this.list

  if (!list) {
    this.list = new lunr.Vector.Node (idx, val, list)
    return this.length++
  }

  if (idx < list.idx) {
    this.list = new lunr.Vector.Node (idx, val, list)
    return this.length++
  }

  var prev = list,
      next = list.next

  while (next != undefined) {
    if (idx < next.idx) {
      prev.next = new lunr.Vector.Node (idx, val, next)
      return this.length++
    }

    prev = next, next = next.next
  }

  prev.next = new lunr.Vector.Node (idx, val, next)
  return this.length++
}
```
- example usage
```shell
...
  var diff = Math.max(3, key.length - token.length)
  similarityBoost = 1 / Math.log(diff)
}

// calculate the query tf-idf score for this token
// applying an similarityBoost to ensure exact matches
// these rank higher than expanded terms
if (pos > -1) queryVector.insert(pos, tf * idf * similarityBoost)

// add all the documents that have this key into a set
// ensuring that the type of key is preserved
var matchingDocuments = self.tokenStore.get(key),
    refs = Object.keys(matchingDocuments),
    refsLen = refs.length
...
```

#### <a name="apidoc.element.lunr.Vector.prototype.magnitude"></a>[function <span class="apidocSignatureSpan">lunr.Vector.prototype.</span>magnitude ()](#apidoc.element.lunr.Vector.prototype.magnitude)
- description and source-code
```javascript
magnitude = function () {
  if (this._magnitude) return this._magnitude
  var node = this.list,
      sumOfSquares = 0,
      val

  while (node) {
    val = node.val
    sumOfSquares += val * val
    node = node.next
  }

  return this._magnitude = Math.sqrt(sumOfSquares)
}
```
- example usage
```shell
...
 *
 * @param {lunr.Vector} otherVector The other vector to calculate the
 * similarity with.
 * @returns {Number}
 * @memberOf Vector
 */
lunr.Vector.prototype.similarity = function (otherVector) {
  return this.dot(otherVector) / (this.magnitude() * otherVector.magnitude())
}
/*!
 * lunr.SortedSet
 * Copyright (C) 2017 Oliver Nightingale
 */

/**
...
```

#### <a name="apidoc.element.lunr.Vector.prototype.similarity"></a>[function <span class="apidocSignatureSpan">lunr.Vector.prototype.</span>similarity (otherVector)](#apidoc.element.lunr.Vector.prototype.similarity)
- description and source-code
```javascript
similarity = function (otherVector) {
  return this.dot(otherVector) / (this.magnitude() * otherVector.magnitude())
}
```
- example usage
```shell
...

  var documentSet = documentSets.reduce(function (memo, set) {
    return memo.intersect(set)
  })

  return documentSet
    .map(function (ref) {
      return { ref: ref, score: queryVector.similarity(this.documentVector(ref)) }
    }, this)
    .sort(function (a, b) {
      return b.score - a.score
    })
}

/**
...
```



# <a name="apidoc.module.lunr.tokenizer"></a>[module lunr.tokenizer](#apidoc.module.lunr.tokenizer)

#### <a name="apidoc.element.lunr.tokenizer.tokenizer"></a>[function <span class="apidocSignatureSpan">lunr.</span>tokenizer (obj)](#apidoc.element.lunr.tokenizer.tokenizer)
- description and source-code
```javascript
tokenizer = function (obj) {
  if (!arguments.length || obj == null || obj == undefined) return []
  if (Array.isArray(obj)) return obj.map(function (t) { return lunr.utils.asString(t).toLowerCase() })

  return obj.toString().trim().toLowerCase().split(lunr.tokenizer.separator)
}
```
- example usage
```shell
...
  }

  var idx = new this

  idx._fields = serialisedData.fields
  idx._ref = serialisedData.ref

  idx.tokenizer(lunr.tokenizer.load(serialisedData.tokenizer))
  idx.documentStore = lunr.Store.load(serialisedData.documentStore)
  idx.tokenStore = lunr.TokenStore.load(serialisedData.tokenStore)
  idx.corpusTokens = lunr.SortedSet.load(serialisedData.corpusTokens)
  idx.pipeline = lunr.Pipeline.load(serialisedData.pipeline)

  return idx
}
...
```

#### <a name="apidoc.element.lunr.tokenizer.load"></a>[function <span class="apidocSignatureSpan">lunr.tokenizer.</span>load (label)](#apidoc.element.lunr.tokenizer.load)
- description and source-code
```javascript
load = function (label) {
  var fn = this.registeredFunctions[label]

  if (!fn) {
    throw new Error('Cannot load un-registered function: ' + label)
  }

  return fn
}
```
- example usage
```shell
...
  }

  var idx = new this

  idx._fields = serialisedData.fields
  idx._ref = serialisedData.ref

  idx.tokenizer(lunr.tokenizer.load(serialisedData.tokenizer))
  idx.documentStore = lunr.Store.load(serialisedData.documentStore)
  idx.tokenStore = lunr.TokenStore.load(serialisedData.tokenStore)
  idx.corpusTokens = lunr.SortedSet.load(serialisedData.corpusTokens)
  idx.pipeline = lunr.Pipeline.load(serialisedData.pipeline)

  return idx
}
...
```

#### <a name="apidoc.element.lunr.tokenizer.registerFunction"></a>[function <span class="apidocSignatureSpan">lunr.tokenizer.</span>registerFunction (fn, label)](#apidoc.element.lunr.tokenizer.registerFunction)
- description and source-code
```javascript
registerFunction = function (fn, label) {
  if (label in this.registeredFunctions) {
    lunr.utils.warn('Overwriting existing tokenizer: ' + label)
  }

  fn.label = label
  this.registeredFunctions[label] = fn
}
```
- example usage
```shell
...

   return w;
 };

 return porterStemmer;
})();

lunr.Pipeline.registerFunction(lunr.stemmer, 'stemmer')
/*!
* lunr.stopWordFilter
* Copyright (C) 2017 Oliver Nightingale
*/

/**
* lunr.generateStopWordFilter builds a stopWordFilter function from the provided
...
```



# <a name="apidoc.module.lunr.tokenizer.registeredFunctions"></a>[module lunr.tokenizer.registeredFunctions](#apidoc.module.lunr.tokenizer.registeredFunctions)

#### <a name="apidoc.element.lunr.tokenizer.registeredFunctions.default"></a>[function <span class="apidocSignatureSpan">lunr.tokenizer.registeredFunctions.</span>default (obj)](#apidoc.element.lunr.tokenizer.registeredFunctions.default)
- description and source-code
```javascript
default = function (obj) {
  if (!arguments.length || obj == null || obj == undefined) return []
  if (Array.isArray(obj)) return obj.map(function (t) { return lunr.utils.asString(t).toLowerCase() })

  return obj.toString().trim().toLowerCase().split(lunr.tokenizer.separator)
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.lunr.utils"></a>[module lunr.utils](#apidoc.module.lunr.utils)

#### <a name="apidoc.element.lunr.utils.asString"></a>[function <span class="apidocSignatureSpan">lunr.utils.</span>asString (obj)](#apidoc.element.lunr.utils.asString)
- description and source-code
```javascript
asString = function (obj) {
  if (obj === void 0 || obj === null) {
    return ""
  } else {
    return obj.toString()
  }
}
```
- example usage
```shell
...
* @module
* @param {String} obj The string to convert into tokens
* @see lunr.tokenizer.separator
* @returns {Array}
*/
lunr.tokenizer = function (obj) {
 if (!arguments.length || obj == null || obj == undefined) return []
 if (Array.isArray(obj)) return obj.map(function (t) { return lunr.utils.asString(t).toLowerCase() })

 return obj.toString().trim().toLowerCase().split(lunr.tokenizer.separator)
}

/**
* The sperator used to split a string into tokens. Override this property to change the behaviour of
* 'lunr.tokenizer' behaviour when tokenizing strings. By default this splits on whitespace and hyphens.
...
```

#### <a name="apidoc.element.lunr.utils.warn"></a>[function <span class="apidocSignatureSpan">lunr.utils.</span>warn (message)](#apidoc.element.lunr.utils.warn)
- description and source-code
```javascript
warn = function (message) {
  if (global.console && console.warn) {
    console.warn(message)
  }
}
```
- example usage
```shell
...
*
* @param {String} message The message to be printed.
* @memberOf Utils
*/
lunr.utils.warn = (function (global) {
 return function (message) {
   if (global.console && console.warn) {
     console.warn(message)
   }
 }
})(this)

/**
* Convert an object to a string.
*
...
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
