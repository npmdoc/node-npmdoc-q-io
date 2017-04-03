# api documentation for  [q-io (v1.13.2)](http://github.com/kriskowal/q-io/)  [![npm package](https://img.shields.io/npm/v/npmdoc-q-io.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-q-io) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-q-io.svg)](https://travis-ci.org/npmdoc/node-npmdoc-q-io)
#### IO using Q promises

[![NPM](https://nodei.co/npm/q-io.png?downloads=true)](https://www.npmjs.com/package/q-io)

[![apidoc](https://npmdoc.github.io/node-npmdoc-q-io/build/screenCapture.buildNpmdoc.browser._2Fhome_2Ftravis_2Fbuild_2Fnpmdoc_2Fnode-npmdoc-q-io_2Ftmp_2Fbuild_2Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-q-io/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-q-io/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-q-io/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Kris Kowal",
        "email": "kris@cixar.com",
        "url": "http://github.com/kriskowal/"
    },
    "bugs": {
        "url": "http://github.com/kriskowal/q-io/issues"
    },
    "contributors": [
        {
            "name": "Montage Studio"
        },
        {
            "name": "Stuart Knightley"
        },
        {
            "name": "Jean-romain Prevost"
        },
        {
            "name": "Andreas Pizsa",
            "url": "http://github.com/AndreasPizsa/"
        }
    ],
    "dependencies": {
        "collections": "^0.2.0",
        "mime": "^1.2.11",
        "mimeparse": "^0.1.4",
        "q": "^1.0.1",
        "qs": "^1.2.1",
        "url2": "^0.0.0"
    },
    "description": "IO using Q promises",
    "devDependencies": {
        "cover": "^0.2.8",
        "jasmine-node": "^1.7",
        "jshint": "^0.9.1",
        "opener": "^1.3"
    },
    "directories": {},
    "dist": {
        "shasum": "eea130d481ddb5e1aa1bc5a66855f7391d06f003",
        "tarball": "https://registry.npmjs.org/q-io/-/q-io-1.13.2.tgz"
    },
    "engines": {
        "node": ">=0.6.0"
    },
    "gitHead": "e282c3b7d0e1c1046265930842c6a16693b928d6",
    "homepage": "http://github.com/kriskowal/q-io/",
    "license": "MIT",
    "maintainers": [
        {
            "name": "arikon",
            "email": "peimei@ya.ru"
        },
        {
            "name": "gagern",
            "email": "Martin.vGagern@gmx.net"
        },
        {
            "name": "kriskowal",
            "email": "kris.kowal@cixar.com"
        }
    ],
    "name": "q-io",
    "optionalDependencies": {},
    "readme": "ERROR: No README data found!",
    "repository": {
        "type": "git",
        "url": "git+ssh://git@github.com/kriskowal/q-io.git"
    },
    "scripts": {
        "cover": "cover run jasmine-node spec && cover report html && opener cover_html/index.html",
        "lint": "jshint q.js",
        "test": "jasmine-node spec",
        "test-browser": "opener spec/q-spec.html"
    },
    "version": "1.13.2"
}
```



# <a name="apidoc.tableOfContents"></a>[table of contents](#apidoc.tableOfContents)

#### [module q-io](#apidoc.module.q-io)
1.  [function <span class="apidocSignatureSpan">q-io.</span>buffer_stream (chunks, charset)](#apidoc.element.q-io.buffer_stream)
1.  [function <span class="apidocSignatureSpan">q-io.</span>chain (end)](#apidoc.element.q-io.chain)
1.  [function <span class="apidocSignatureSpan">q-io.</span>reader (_stream, charset)](#apidoc.element.q-io.reader)
1.  object <span class="apidocSignatureSpan">q-io.</span>buffer_stream.prototype
1.  object <span class="apidocSignatureSpan">q-io.</span>chain.prototype
1.  object <span class="apidocSignatureSpan">q-io.</span>content
1.  object <span class="apidocSignatureSpan">q-io.</span>cookie
1.  object <span class="apidocSignatureSpan">q-io.</span>decorators
1.  object <span class="apidocSignatureSpan">q-io.</span>deprecate
1.  object <span class="apidocSignatureSpan">q-io.</span>fs
1.  object <span class="apidocSignatureSpan">q-io.</span>fs2http
1.  object <span class="apidocSignatureSpan">q-io.</span>fs_boot
1.  object <span class="apidocSignatureSpan">q-io.</span>fs_common
1.  object <span class="apidocSignatureSpan">q-io.</span>html
1.  object <span class="apidocSignatureSpan">q-io.</span>http
1.  object <span class="apidocSignatureSpan">q-io.</span>http_apps
1.  object <span class="apidocSignatureSpan">q-io.</span>http_cookie
1.  object <span class="apidocSignatureSpan">q-io.</span>json
1.  object <span class="apidocSignatureSpan">q-io.</span>negotiate
1.  object <span class="apidocSignatureSpan">q-io.</span>proxy
1.  object <span class="apidocSignatureSpan">q-io.</span>redirect
1.  object <span class="apidocSignatureSpan">q-io.</span>route
1.  object <span class="apidocSignatureSpan">q-io.</span>status

#### [module q-io.buffer_stream](#apidoc.module.q-io.buffer_stream)
1.  [function <span class="apidocSignatureSpan">q-io.</span>buffer_stream (chunks, charset)](#apidoc.element.q-io.buffer_stream.buffer_stream)

#### [module q-io.buffer_stream.prototype](#apidoc.module.q-io.buffer_stream.prototype)
1.  [function <span class="apidocSignatureSpan">q-io.buffer_stream.prototype.</span>close ()](#apidoc.element.q-io.buffer_stream.prototype.close)
1.  [function <span class="apidocSignatureSpan">q-io.buffer_stream.prototype.</span>destroy ()](#apidoc.element.q-io.buffer_stream.prototype.destroy)
1.  [function <span class="apidocSignatureSpan">q-io.buffer_stream.prototype.</span>forEach (write, thisp)](#apidoc.element.q-io.buffer_stream.prototype.forEach)
1.  [function <span class="apidocSignatureSpan">q-io.buffer_stream.prototype.</span>read ()](#apidoc.element.q-io.buffer_stream.prototype.read)
1.  [function <span class="apidocSignatureSpan">q-io.buffer_stream.prototype.</span>write (chunk)](#apidoc.element.q-io.buffer_stream.prototype.write)

#### [module q-io.chain](#apidoc.module.q-io.chain)
1.  [function <span class="apidocSignatureSpan">q-io.</span>chain (end)](#apidoc.element.q-io.chain.chain)

#### [module q-io.chain.prototype](#apidoc.module.q-io.chain.prototype)
1.  [function <span class="apidocSignatureSpan">q-io.chain.prototype.</span>use (App)](#apidoc.element.q-io.chain.prototype.use)

#### [module q-io.content](#apidoc.module.q-io.content)
1.  [function <span class="apidocSignatureSpan">q-io.</span>content (content, contentType, status)](#apidoc.element.q-io.content.content)
1.  [function <span class="apidocSignatureSpan">q-io.content.</span>Content (body, contentType, status)](#apidoc.element.q-io.content.Content)
1.  [function <span class="apidocSignatureSpan">q-io.content.</span>ContentRequest (app)](#apidoc.element.q-io.content.ContentRequest)
1.  [function <span class="apidocSignatureSpan">q-io.content.</span>Inspect (app)](#apidoc.element.q-io.content.Inspect)
1.  [function <span class="apidocSignatureSpan">q-io.content.</span>ParseQuery (app)](#apidoc.element.q-io.content.ParseQuery)
1.  [function <span class="apidocSignatureSpan">q-io.content.</span>ok (content, contentType, status)](#apidoc.element.q-io.content.ok)

#### [module q-io.cookie](#apidoc.module.q-io.cookie)
1.  [function <span class="apidocSignatureSpan">q-io.cookie.</span>CookieJar (app)](#apidoc.element.q-io.cookie.CookieJar)

#### [module q-io.decorators](#apidoc.module.q-io.decorators)
1.  [function <span class="apidocSignatureSpan">q-io.decorators.</span>Date (app, present)](#apidoc.element.q-io.decorators.Date)
1.  [function <span class="apidocSignatureSpan">q-io.decorators.</span>Debug (app)](#apidoc.element.q-io.decorators.Debug)
1.  [function <span class="apidocSignatureSpan">q-io.decorators.</span>Decorators (decorators, app)](#apidoc.element.q-io.decorators.Decorators)
1.  [function <span class="apidocSignatureSpan">q-io.decorators.</span>Error (app, debug)](#apidoc.element.q-io.decorators.Error)
1.  [function <span class="apidocSignatureSpan">q-io.decorators.</span>Headers (app, headers)](#apidoc.element.q-io.decorators.Headers)
1.  [function <span class="apidocSignatureSpan">q-io.decorators.</span>Log (app, log, stamp)](#apidoc.element.q-io.decorators.Log)
1.  [function <span class="apidocSignatureSpan">q-io.decorators.</span>Normalize (app)](#apidoc.element.q-io.decorators.Normalize)
1.  [function <span class="apidocSignatureSpan">q-io.decorators.</span>Permanent (app, future)](#apidoc.element.q-io.decorators.Permanent)
1.  [function <span class="apidocSignatureSpan">q-io.decorators.</span>Time (app)](#apidoc.element.q-io.decorators.Time)

#### [module q-io.deprecate](#apidoc.module.q-io.deprecate)
1.  [function <span class="apidocSignatureSpan">q-io.deprecate.</span>deprecateMethod (scope, deprecatedFunction, name, alternative)](#apidoc.element.q-io.deprecate.deprecateMethod)
1.  [function <span class="apidocSignatureSpan">q-io.deprecate.</span>deprecationWarning (name, alternative, stackTraceLimit)](#apidoc.element.q-io.deprecate.deprecationWarning)

#### [module q-io.fs](#apidoc.module.q-io.fs)
1.  [function <span class="apidocSignatureSpan">q-io.fs.</span>Mock (files, workingDirectory)](#apidoc.element.q-io.fs.Mock)
1.  [function <span class="apidocSignatureSpan">q-io.fs.</span>Root (outer, root)](#apidoc.element.q-io.fs.Root)
1.  [function <span class="apidocSignatureSpan">q-io.fs.</span>SEPARATORS_RE ()](#apidoc.element.q-io.fs.SEPARATORS_RE)
1.  [function <span class="apidocSignatureSpan">q-io.fs.</span>Stats (nodeStat)](#apidoc.element.q-io.fs.Stats)
1.  [function <span class="apidocSignatureSpan">q-io.fs.</span>absolute (path)](#apidoc.element.q-io.fs.absolute)
1.  [function <span class="apidocSignatureSpan">q-io.fs.</span>append (path, content, flags, charset, options)](#apidoc.element.q-io.fs.append)
1.  [function <span class="apidocSignatureSpan">q-io.fs.</span>base (path, extension)](#apidoc.element.q-io.fs.base)
1.  [function <span class="apidocSignatureSpan">q-io.fs.</span>canonical (path)](#apidoc.element.q-io.fs.canonical)
1.  [function <span class="apidocSignatureSpan">q-io.fs.</span>chmod (path, mode)](#apidoc.element.q-io.fs.chmod)
1.  [function <span class="apidocSignatureSpan">q-io.fs.</span>chown (path, uid, gid)](#apidoc.element.q-io.fs.chown)
1.  [function <span class="apidocSignatureSpan">q-io.fs.</span>contains (parent, child)](#apidoc.element.q-io.fs.contains)
1.  [function <span class="apidocSignatureSpan">q-io.fs.</span>copy (source, target)](#apidoc.element.q-io.fs.copy)
1.  [function <span class="apidocSignatureSpan">q-io.fs.</span>copyTree (source, target)](#apidoc.element.q-io.fs.copyTree)
1.  [function <span class="apidocSignatureSpan">q-io.fs.</span>directory (path)](#apidoc.element.q-io.fs.directory)
1.  [function <span class="apidocSignatureSpan">q-io.fs.</span>exists (path)](#apidoc.element.q-io.fs.exists)
1.  [function <span class="apidocSignatureSpan">q-io.fs.</span>extension (path)](#apidoc.element.q-io.fs.extension)
1.  [function <span class="apidocSignatureSpan">q-io.fs.</span>isAbsolute (path)](#apidoc.element.q-io.fs.isAbsolute)
1.  [function <span class="apidocSignatureSpan">q-io.fs.</span>isDirectory (path)](#apidoc.element.q-io.fs.isDirectory)
1.  [function <span class="apidocSignatureSpan">q-io.fs.</span>isFile (path)](#apidoc.element.q-io.fs.isFile)
1.  [function <span class="apidocSignatureSpan">q-io.fs.</span>isRelative (path)](#apidoc.element.q-io.fs.isRelative)
1.  [function <span class="apidocSignatureSpan">q-io.fs.</span>isRoot (first)](#apidoc.element.q-io.fs.isRoot)
1.  [function <span class="apidocSignatureSpan">q-io.fs.</span>isSymbolicLink (path)](#apidoc.element.q-io.fs.isSymbolicLink)
1.  [function <span class="apidocSignatureSpan">q-io.fs.</span>join ()](#apidoc.element.q-io.fs.join)
1.  [function <span class="apidocSignatureSpan">q-io.fs.</span>lastAccessed (path)](#apidoc.element.q-io.fs.lastAccessed)
1.  [function <span class="apidocSignatureSpan">q-io.fs.</span>lastModified (path)](#apidoc.element.q-io.fs.lastModified)
1.  [function <span class="apidocSignatureSpan">q-io.fs.</span>link (source, target)](#apidoc.element.q-io.fs.link)
1.  [function <span class="apidocSignatureSpan">q-io.fs.</span>list ()](#apidoc.element.q-io.fs.list)
1.  [function <span class="apidocSignatureSpan">q-io.fs.</span>listDirectoryTree (path)](#apidoc.element.q-io.fs.listDirectoryTree)
1.  [function <span class="apidocSignatureSpan">q-io.fs.</span>listTree (basePath, guard)](#apidoc.element.q-io.fs.listTree)
1.  [function <span class="apidocSignatureSpan">q-io.fs.</span>makeDirectory (path, mode)](#apidoc.element.q-io.fs.makeDirectory)
1.  [function <span class="apidocSignatureSpan">q-io.fs.</span>makeTree (path, mode)](#apidoc.element.q-io.fs.makeTree)
1.  [function <span class="apidocSignatureSpan">q-io.fs.</span>merge (fss)](#apidoc.element.q-io.fs.merge)
1.  [function <span class="apidocSignatureSpan">q-io.fs.</span>mock (path)](#apidoc.element.q-io.fs.mock)
1.  [function <span class="apidocSignatureSpan">q-io.fs.</span>move (source, target)](#apidoc.element.q-io.fs.move)
1.  [function <span class="apidocSignatureSpan">q-io.fs.</span>normal ()](#apidoc.element.q-io.fs.normal)
1.  [function <span class="apidocSignatureSpan">q-io.fs.</span>open ()](#apidoc.element.q-io.fs.open)
1.  [function <span class="apidocSignatureSpan">q-io.fs.</span>read (path, flags, charset, options)](#apidoc.element.q-io.fs.read)
1.  [function <span class="apidocSignatureSpan">q-io.fs.</span>readLink (path)](#apidoc.element.q-io.fs.readLink)
1.  [function <span class="apidocSignatureSpan">q-io.fs.</span>relative (source, target)](#apidoc.element.q-io.fs.relative)
1.  [function <span class="apidocSignatureSpan">q-io.fs.</span>relativeFromDirectory (source, target)](#apidoc.element.q-io.fs.relativeFromDirectory)
1.  [function <span class="apidocSignatureSpan">q-io.fs.</span>relativeFromFile (source, target)](#apidoc.element.q-io.fs.relativeFromFile)
1.  [function <span class="apidocSignatureSpan">q-io.fs.</span>remove (path)](#apidoc.element.q-io.fs.remove)
1.  [function <span class="apidocSignatureSpan">q-io.fs.</span>removeDirectory (path)](#apidoc.element.q-io.fs.removeDirectory)
1.  [function <span class="apidocSignatureSpan">q-io.fs.</span>removeTree (path)](#apidoc.element.q-io.fs.removeTree)
1.  [function <span class="apidocSignatureSpan">q-io.fs.</span>rename (source, target)](#apidoc.element.q-io.fs.rename)
1.  [function <span class="apidocSignatureSpan">q-io.fs.</span>reroot (path)](#apidoc.element.q-io.fs.reroot)
1.  [function <span class="apidocSignatureSpan">q-io.fs.</span>resolve ()](#apidoc.element.q-io.fs.resolve)
1.  [function <span class="apidocSignatureSpan">q-io.fs.</span>root (path)](#apidoc.element.q-io.fs.root)
1.  [function <span class="apidocSignatureSpan">q-io.fs.</span>split (path)](#apidoc.element.q-io.fs.split)
1.  [function <span class="apidocSignatureSpan">q-io.fs.</span>stat (path)](#apidoc.element.q-io.fs.stat)
1.  [function <span class="apidocSignatureSpan">q-io.fs.</span>statFd (fd)](#apidoc.element.q-io.fs.statFd)
1.  [function <span class="apidocSignatureSpan">q-io.fs.</span>statLink (path)](#apidoc.element.q-io.fs.statLink)
1.  [function <span class="apidocSignatureSpan">q-io.fs.</span>symbolicCopy (source, target, type)](#apidoc.element.q-io.fs.symbolicCopy)
1.  [function <span class="apidocSignatureSpan">q-io.fs.</span>symbolicLink (target, relative, type)](#apidoc.element.q-io.fs.symbolicLink)
1.  [function <span class="apidocSignatureSpan">q-io.fs.</span>toObject (path)](#apidoc.element.q-io.fs.toObject)
1.  [function <span class="apidocSignatureSpan">q-io.fs.</span>write (path, content, flags, charset, options)](#apidoc.element.q-io.fs.write)
1.  string <span class="apidocSignatureSpan">q-io.fs.</span>ROOT
1.  string <span class="apidocSignatureSpan">q-io.fs.</span>SEPARATOR

#### [module q-io.fs2http](#apidoc.module.q-io.fs2http)
1.  [function <span class="apidocSignatureSpan">q-io.fs2http.</span>Client (fs)](#apidoc.element.q-io.fs2http.Client)
1.  [function <span class="apidocSignatureSpan">q-io.fs2http.</span>read (request, qualifier)](#apidoc.element.q-io.fs2http.read)
1.  [function <span class="apidocSignatureSpan">q-io.fs2http.</span>request (request)](#apidoc.element.q-io.fs2http.request)

#### [module q-io.fs_boot](#apidoc.module.q-io.fs_boot)
1.  [function <span class="apidocSignatureSpan">q-io.fs_boot.</span>SEPARATORS_RE ()](#apidoc.element.q-io.fs_boot.SEPARATORS_RE)
1.  [function <span class="apidocSignatureSpan">q-io.fs_boot.</span>base (path, extension)](#apidoc.element.q-io.fs_boot.base)
1.  [function <span class="apidocSignatureSpan">q-io.fs_boot.</span>directory (path)](#apidoc.element.q-io.fs_boot.directory)
1.  [function <span class="apidocSignatureSpan">q-io.fs_boot.</span>extension (path)](#apidoc.element.q-io.fs_boot.extension)
1.  [function <span class="apidocSignatureSpan">q-io.fs_boot.</span>isAbsolute (path)](#apidoc.element.q-io.fs_boot.isAbsolute)
1.  [function <span class="apidocSignatureSpan">q-io.fs_boot.</span>isRelative (path)](#apidoc.element.q-io.fs_boot.isRelative)
1.  [function <span class="apidocSignatureSpan">q-io.fs_boot.</span>isRoot (first)](#apidoc.element.q-io.fs_boot.isRoot)
1.  [function <span class="apidocSignatureSpan">q-io.fs_boot.</span>join ()](#apidoc.element.q-io.fs_boot.join)
1.  [function <span class="apidocSignatureSpan">q-io.fs_boot.</span>normal ()](#apidoc.element.q-io.fs_boot.normal)
1.  [function <span class="apidocSignatureSpan">q-io.fs_boot.</span>resolve ()](#apidoc.element.q-io.fs_boot.resolve)
1.  [function <span class="apidocSignatureSpan">q-io.fs_boot.</span>root (path)](#apidoc.element.q-io.fs_boot.root)
1.  [function <span class="apidocSignatureSpan">q-io.fs_boot.</span>split (path)](#apidoc.element.q-io.fs_boot.split)
1.  string <span class="apidocSignatureSpan">q-io.fs_boot.</span>ROOT
1.  string <span class="apidocSignatureSpan">q-io.fs_boot.</span>SEPARATOR

#### [module q-io.fs_common](#apidoc.module.q-io.fs_common)
1.  [function <span class="apidocSignatureSpan">q-io.fs_common.</span>update (exports, workingDirectory)](#apidoc.element.q-io.fs_common.update)

#### [module q-io.html](#apidoc.module.q-io.html)
1.  [function <span class="apidocSignatureSpan">q-io.html.</span>HandleHtmlFragmentResponses (app, handleHtmlFragmentResponse)](#apidoc.element.q-io.html.HandleHtmlFragmentResponses)
1.  [function <span class="apidocSignatureSpan">q-io.html.</span>escapeHtml (text)](#apidoc.element.q-io.html.escapeHtml)
1.  [function <span class="apidocSignatureSpan">q-io.html.</span>handleHtmlFragmentResponse (response)](#apidoc.element.q-io.html.handleHtmlFragmentResponse)

#### [module q-io.http](#apidoc.module.q-io.http)
1.  [function <span class="apidocSignatureSpan">q-io.http.</span>ClientResponse (_response, charset)](#apidoc.element.q-io.http.ClientResponse)
1.  [function <span class="apidocSignatureSpan">q-io.http.</span>Server (respond)](#apidoc.element.q-io.http.Server)
1.  [function <span class="apidocSignatureSpan">q-io.http.</span>ServerRequest (_request, ssl)](#apidoc.element.q-io.http.ServerRequest)
1.  [function <span class="apidocSignatureSpan">q-io.http.</span>ServerResponse (_response, ssl)](#apidoc.element.q-io.http.ServerResponse)
1.  [function <span class="apidocSignatureSpan">q-io.http.</span>normalizeRequest (request)](#apidoc.element.q-io.http.normalizeRequest)
1.  [function <span class="apidocSignatureSpan">q-io.http.</span>normalizeResponse (response)](#apidoc.element.q-io.http.normalizeResponse)
1.  [function <span class="apidocSignatureSpan">q-io.http.</span>read (request, qualifier)](#apidoc.element.q-io.http.read)
1.  [function <span class="apidocSignatureSpan">q-io.http.</span>request (request)](#apidoc.element.q-io.http.request)

#### [module q-io.http_apps](#apidoc.module.q-io.http_apps)
1.  [function <span class="apidocSignatureSpan">q-io.http_apps.</span>Branch (paths, notFound)](#apidoc.element.q-io.http_apps.Branch)
1.  [function <span class="apidocSignatureSpan">q-io.http_apps.</span>Cap (app, notFound)](#apidoc.element.q-io.http_apps.Cap)
1.  [function <span class="apidocSignatureSpan">q-io.http_apps.</span>Chain (end)](#apidoc.element.q-io.http_apps.Chain)
1.  [function <span class="apidocSignatureSpan">q-io.http_apps.</span>Charset (types, notAcceptable)](#apidoc.element.q-io.http_apps.Charset)
1.  [function <span class="apidocSignatureSpan">q-io.http_apps.</span>Content (body, contentType, status)](#apidoc.element.q-io.http_apps.Content)
1.  [function <span class="apidocSignatureSpan">q-io.http_apps.</span>ContentRequest (app)](#apidoc.element.q-io.http_apps.ContentRequest)
1.  [function <span class="apidocSignatureSpan">q-io.http_apps.</span>ContentType (types, notAcceptable)](#apidoc.element.q-io.http_apps.ContentType)
1.  [function <span class="apidocSignatureSpan">q-io.http_apps.</span>CookieJar (app)](#apidoc.element.q-io.http_apps.CookieJar)
1.  [function <span class="apidocSignatureSpan">q-io.http_apps.</span>Date (app, present)](#apidoc.element.q-io.http_apps.Date)
1.  [function <span class="apidocSignatureSpan">q-io.http_apps.</span>Debug (app)](#apidoc.element.q-io.http_apps.Debug)
1.  [function <span class="apidocSignatureSpan">q-io.http_apps.</span>Decorators (decorators, app)](#apidoc.element.q-io.http_apps.Decorators)
1.  [function <span class="apidocSignatureSpan">q-io.http_apps.</span>DirectoryIndex (app, indexFile)](#apidoc.element.q-io.http_apps.DirectoryIndex)
1.  [function <span class="apidocSignatureSpan">q-io.http_apps.</span>Encoding (types, notAcceptable)](#apidoc.element.q-io.http_apps.Encoding)
1.  [function <span class="apidocSignatureSpan">q-io.http_apps.</span>Error (app, debug)](#apidoc.element.q-io.http_apps.Error)
1.  [function <span class="apidocSignatureSpan">q-io.http_apps.</span>File (path, contentType)](#apidoc.element.q-io.http_apps.File)
1.  [function <span class="apidocSignatureSpan">q-io.http_apps.</span>FileTree (root, options)](#apidoc.element.q-io.http_apps.FileTree)
1.  [function <span class="apidocSignatureSpan">q-io.http_apps.</span>HandleHtmlFragmentResponses (app, handleHtmlFragmentResponse)](#apidoc.element.q-io.http_apps.HandleHtmlFragmentResponses)
1.  [function <span class="apidocSignatureSpan">q-io.http_apps.</span>HandleJsonResponses (app, reviver, tab)](#apidoc.element.q-io.http_apps.HandleJsonResponses)
1.  [function <span class="apidocSignatureSpan">q-io.http_apps.</span>Headers (app, headers)](#apidoc.element.q-io.http_apps.Headers)
1.  [function <span class="apidocSignatureSpan">q-io.http_apps.</span>Host (appForHost, notAcceptable)](#apidoc.element.q-io.http_apps.Host)
1.  [function <span class="apidocSignatureSpan">q-io.http_apps.</span>Inspect (app)](#apidoc.element.q-io.http_apps.Inspect)
1.  [function <span class="apidocSignatureSpan">q-io.http_apps.</span>Json (app, reviver, tabs)](#apidoc.element.q-io.http_apps.Json)
1.  [function <span class="apidocSignatureSpan">q-io.http_apps.</span>JsonRequest (app, badRequest)](#apidoc.element.q-io.http_apps.JsonRequest)
1.  [function <span class="apidocSignatureSpan">q-io.http_apps.</span>Language (types, notAcceptable)](#apidoc.element.q-io.http_apps.Language)
1.  [function <span class="apidocSignatureSpan">q-io.http_apps.</span>ListDirectories (app, listDirectory)](#apidoc.element.q-io.http_apps.ListDirectories)
1.  [function <span class="apidocSignatureSpan">q-io.http_apps.</span>Log (app, log, stamp)](#apidoc.element.q-io.http_apps.Log)
1.  [function <span class="apidocSignatureSpan">q-io.http_apps.</span>Method (methods, methodNotAllowed)](#apidoc.element.q-io.http_apps.Method)
1.  [function <span class="apidocSignatureSpan">q-io.http_apps.</span>Normalize (app)](#apidoc.element.q-io.http_apps.Normalize)
1.  [function <span class="apidocSignatureSpan">q-io.http_apps.</span>ParseQuery (app)](#apidoc.element.q-io.http_apps.ParseQuery)
1.  [function <span class="apidocSignatureSpan">q-io.http_apps.</span>Permanent (app, future)](#apidoc.element.q-io.http_apps.Permanent)
1.  [function <span class="apidocSignatureSpan">q-io.http_apps.</span>PermanentRedirect (location, status, tree)](#apidoc.element.q-io.http_apps.PermanentRedirect)
1.  [function <span class="apidocSignatureSpan">q-io.http_apps.</span>PermanentRedirectTree (location, status)](#apidoc.element.q-io.http_apps.PermanentRedirectTree)
1.  [function <span class="apidocSignatureSpan">q-io.http_apps.</span>Proxy (app)](#apidoc.element.q-io.http_apps.Proxy)
1.  [function <span class="apidocSignatureSpan">q-io.http_apps.</span>ProxyTree (url)](#apidoc.element.q-io.http_apps.ProxyTree)
1.  [function <span class="apidocSignatureSpan">q-io.http_apps.</span>Redirect (location, status, tree)](#apidoc.element.q-io.http_apps.Redirect)
1.  [function <span class="apidocSignatureSpan">q-io.http_apps.</span>RedirectTrap (app, maxRedirects)](#apidoc.element.q-io.http_apps.RedirectTrap)
1.  [function <span class="apidocSignatureSpan">q-io.http_apps.</span>RedirectTree (location, status)](#apidoc.element.q-io.http_apps.RedirectTree)
1.  [function <span class="apidocSignatureSpan">q-io.http_apps.</span>Select (select)](#apidoc.element.q-io.http_apps.Select)
1.  [function <span class="apidocSignatureSpan">q-io.http_apps.</span>Tap (app, tap)](#apidoc.element.q-io.http_apps.Tap)
1.  [function <span class="apidocSignatureSpan">q-io.http_apps.</span>TemporaryRedirect (location, status, tree)](#apidoc.element.q-io.http_apps.TemporaryRedirect)
1.  [function <span class="apidocSignatureSpan">q-io.http_apps.</span>TemporaryRedirectTree (location, status)](#apidoc.element.q-io.http_apps.TemporaryRedirectTree)
1.  [function <span class="apidocSignatureSpan">q-io.http_apps.</span>Time (app)](#apidoc.element.q-io.http_apps.Time)
1.  [function <span class="apidocSignatureSpan">q-io.http_apps.</span>Trap (app, trap)](#apidoc.element.q-io.http_apps.Trap)
1.  [function <span class="apidocSignatureSpan">q-io.http_apps.</span>appForStatus (status)](#apidoc.element.q-io.http_apps.appForStatus)
1.  [function <span class="apidocSignatureSpan">q-io.http_apps.</span>badRequest (request)](#apidoc.element.q-io.http_apps.badRequest)
1.  [function <span class="apidocSignatureSpan">q-io.http_apps.</span>content (content, contentType, status)](#apidoc.element.q-io.http_apps.content)
1.  [function <span class="apidocSignatureSpan">q-io.http_apps.</span>directory (request, path)](#apidoc.element.q-io.http_apps.directory)
1.  [function <span class="apidocSignatureSpan">q-io.http_apps.</span>escapeHtml (text)](#apidoc.element.q-io.http_apps.escapeHtml)
1.  [function <span class="apidocSignatureSpan">q-io.http_apps.</span>etag (stat)](#apidoc.element.q-io.http_apps.etag)
1.  [function <span class="apidocSignatureSpan">q-io.http_apps.</span>file (request, path, contentType, fs)](#apidoc.element.q-io.http_apps.file)
1.  [function <span class="apidocSignatureSpan">q-io.http_apps.</span>handleHtmlFragmentResponse (response)](#apidoc.element.q-io.http_apps.handleHtmlFragmentResponse)
1.  [function <span class="apidocSignatureSpan">q-io.http_apps.</span>handleJsonResponse (response, revivier, tab)](#apidoc.element.q-io.http_apps.handleJsonResponse)
1.  [function <span class="apidocSignatureSpan">q-io.http_apps.</span>htmlResponseForStatus (request, status, message, addendum)](#apidoc.element.q-io.http_apps.htmlResponseForStatus)
1.  [function <span class="apidocSignatureSpan">q-io.http_apps.</span>isRedirect (response)](#apidoc.element.q-io.http_apps.isRedirect)
1.  [function <span class="apidocSignatureSpan">q-io.http_apps.</span>json (content, reviver, tabs)](#apidoc.element.q-io.http_apps.json)
1.  [function <span class="apidocSignatureSpan">q-io.http_apps.</span>listDirectory (request, response)](#apidoc.element.q-io.http_apps.listDirectory)
1.  [function <span class="apidocSignatureSpan">q-io.http_apps.</span>listDirectoryData (request, response)](#apidoc.element.q-io.http_apps.listDirectoryData)
1.  [function <span class="apidocSignatureSpan">q-io.http_apps.</span>listDirectoryHtmlFragment (request, response)](#apidoc.element.q-io.http_apps.listDirectoryHtmlFragment)
1.  [function <span class="apidocSignatureSpan">q-io.http_apps.</span>listDirectoryJson (request, response)](#apidoc.element.q-io.http_apps.listDirectoryJson)
1.  [function <span class="apidocSignatureSpan">q-io.http_apps.</span>listDirectoryMarkdown (request, response)](#apidoc.element.q-io.http_apps.listDirectoryMarkdown)
1.  [function <span class="apidocSignatureSpan">q-io.http_apps.</span>listDirectoryText (request, response)](#apidoc.element.q-io.http_apps.listDirectoryText)
1.  [function <span class="apidocSignatureSpan">q-io.http_apps.</span>methodNotAllowed (request)](#apidoc.element.q-io.http_apps.methodNotAllowed)
1.  [function <span class="apidocSignatureSpan">q-io.http_apps.</span>negotiate (request, types, header)](#apidoc.element.q-io.http_apps.negotiate)
1.  [function <span class="apidocSignatureSpan">q-io.http_apps.</span>noLanguage (request)](#apidoc.element.q-io.http_apps.noLanguage)
1.  [function <span class="apidocSignatureSpan">q-io.http_apps.</span>notAcceptable (request)](#apidoc.element.q-io.http_apps.notAcceptable)
1.  [function <span class="apidocSignatureSpan">q-io.http_apps.</span>notFound (request)](#apidoc.element.q-io.http_apps.notFound)
1.  [function <span class="apidocSignatureSpan">q-io.http_apps.</span>ok (content, contentType, status)](#apidoc.element.q-io.http_apps.ok)
1.  [function <span class="apidocSignatureSpan">q-io.http_apps.</span>permanentRedirect (request, location, status)](#apidoc.element.q-io.http_apps.permanentRedirect)
1.  [function <span class="apidocSignatureSpan">q-io.http_apps.</span>permanentRedirectTree (request, location, status)](#apidoc.element.q-io.http_apps.permanentRedirectTree)
1.  [function <span class="apidocSignatureSpan">q-io.http_apps.</span>redirect (request, location, status, tree)](#apidoc.element.q-io.http_apps.redirect)
1.  [function <span class="apidocSignatureSpan">q-io.http_apps.</span>redirectHtml (request, location, status)](#apidoc.element.q-io.http_apps.redirectHtml)
1.  [function <span class="apidocSignatureSpan">q-io.http_apps.</span>redirectText (request, location, status)](#apidoc.element.q-io.http_apps.redirectText)
1.  [function <span class="apidocSignatureSpan">q-io.http_apps.</span>redirectTree (request, location, status)](#apidoc.element.q-io.http_apps.redirectTree)
1.  [function <span class="apidocSignatureSpan">q-io.http_apps.</span>responseForStatus (request, status, addendum)](#apidoc.element.q-io.http_apps.responseForStatus)
1.  [function <span class="apidocSignatureSpan">q-io.http_apps.</span>statusWithNoEntityBody (status)](#apidoc.element.q-io.http_apps.statusWithNoEntityBody)
1.  [function <span class="apidocSignatureSpan">q-io.http_apps.</span>temporaryRedirect (request, location, status)](#apidoc.element.q-io.http_apps.temporaryRedirect)
1.  [function <span class="apidocSignatureSpan">q-io.http_apps.</span>temporaryRedirectTree (request, location, status)](#apidoc.element.q-io.http_apps.temporaryRedirectTree)
1.  [function <span class="apidocSignatureSpan">q-io.http_apps.</span>textResponseForStatus (request, status, message, addendum)](#apidoc.element.q-io.http_apps.textResponseForStatus)
1.  object <span class="apidocSignatureSpan">q-io.http_apps.</span>statusCodes
1.  object <span class="apidocSignatureSpan">q-io.http_apps.</span>statusMessages

#### [module q-io.http_cookie](#apidoc.module.q-io.http_cookie)
1.  [function <span class="apidocSignatureSpan">q-io.http_cookie.</span>parse (cookie, date)](#apidoc.element.q-io.http_cookie.parse)
1.  [function <span class="apidocSignatureSpan">q-io.http_cookie.</span>stringify (key, value, options)](#apidoc.element.q-io.http_cookie.stringify)

#### [module q-io.json](#apidoc.module.q-io.json)
1.  [function <span class="apidocSignatureSpan">q-io.</span>json (content, reviver, tabs)](#apidoc.element.q-io.json.json)
1.  [function <span class="apidocSignatureSpan">q-io.json.</span>HandleJsonResponses (app, reviver, tab)](#apidoc.element.q-io.json.HandleJsonResponses)
1.  [function <span class="apidocSignatureSpan">q-io.json.</span>Json (app, reviver, tabs)](#apidoc.element.q-io.json.Json)
1.  [function <span class="apidocSignatureSpan">q-io.json.</span>JsonRequest (app, badRequest)](#apidoc.element.q-io.json.JsonRequest)
1.  [function <span class="apidocSignatureSpan">q-io.json.</span>handleJsonResponse (response, revivier, tab)](#apidoc.element.q-io.json.handleJsonResponse)

#### [module q-io.negotiate](#apidoc.module.q-io.negotiate)
1.  [function <span class="apidocSignatureSpan">q-io.</span>negotiate (request, types, header)](#apidoc.element.q-io.negotiate.negotiate)
1.  [function <span class="apidocSignatureSpan">q-io.negotiate.</span>Charset (types, notAcceptable)](#apidoc.element.q-io.negotiate.Charset)
1.  [function <span class="apidocSignatureSpan">q-io.negotiate.</span>ContentType (types, notAcceptable)](#apidoc.element.q-io.negotiate.ContentType)
1.  [function <span class="apidocSignatureSpan">q-io.negotiate.</span>Encoding (types, notAcceptable)](#apidoc.element.q-io.negotiate.Encoding)
1.  [function <span class="apidocSignatureSpan">q-io.negotiate.</span>Host (appForHost, notAcceptable)](#apidoc.element.q-io.negotiate.Host)
1.  [function <span class="apidocSignatureSpan">q-io.negotiate.</span>Language (types, notAcceptable)](#apidoc.element.q-io.negotiate.Language)
1.  [function <span class="apidocSignatureSpan">q-io.negotiate.</span>Method (methods, methodNotAllowed)](#apidoc.element.q-io.negotiate.Method)
1.  [function <span class="apidocSignatureSpan">q-io.negotiate.</span>Select (select)](#apidoc.element.q-io.negotiate.Select)

#### [module q-io.proxy](#apidoc.module.q-io.proxy)
1.  [function <span class="apidocSignatureSpan">q-io.proxy.</span>Proxy (app)](#apidoc.element.q-io.proxy.Proxy)
1.  [function <span class="apidocSignatureSpan">q-io.proxy.</span>ProxyTree (url)](#apidoc.element.q-io.proxy.ProxyTree)

#### [module q-io.reader](#apidoc.module.q-io.reader)
1.  [function <span class="apidocSignatureSpan">q-io.</span>reader (_stream, charset)](#apidoc.element.q-io.reader.reader)
1.  [function <span class="apidocSignatureSpan">q-io.reader.</span>join (buffers)](#apidoc.element.q-io.reader.join)
1.  [function <span class="apidocSignatureSpan">q-io.reader.</span>read (stream, charset)](#apidoc.element.q-io.reader.read)

#### [module q-io.redirect](#apidoc.module.q-io.redirect)
1.  [function <span class="apidocSignatureSpan">q-io.</span>redirect (request, location, status, tree)](#apidoc.element.q-io.redirect.redirect)
1.  [function <span class="apidocSignatureSpan">q-io.redirect.</span>PermanentRedirect (location, status, tree)](#apidoc.element.q-io.redirect.PermanentRedirect)
1.  [function <span class="apidocSignatureSpan">q-io.redirect.</span>PermanentRedirectTree (location, status)](#apidoc.element.q-io.redirect.PermanentRedirectTree)
1.  [function <span class="apidocSignatureSpan">q-io.redirect.</span>Redirect (location, status, tree)](#apidoc.element.q-io.redirect.Redirect)
1.  [function <span class="apidocSignatureSpan">q-io.redirect.</span>RedirectTrap (app, maxRedirects)](#apidoc.element.q-io.redirect.RedirectTrap)
1.  [function <span class="apidocSignatureSpan">q-io.redirect.</span>RedirectTree (location, status)](#apidoc.element.q-io.redirect.RedirectTree)
1.  [function <span class="apidocSignatureSpan">q-io.redirect.</span>TemporaryRedirect (location, status, tree)](#apidoc.element.q-io.redirect.TemporaryRedirect)
1.  [function <span class="apidocSignatureSpan">q-io.redirect.</span>TemporaryRedirectTree (location, status)](#apidoc.element.q-io.redirect.TemporaryRedirectTree)
1.  [function <span class="apidocSignatureSpan">q-io.redirect.</span>isRedirect (response)](#apidoc.element.q-io.redirect.isRedirect)
1.  [function <span class="apidocSignatureSpan">q-io.redirect.</span>permanentRedirect (request, location, status)](#apidoc.element.q-io.redirect.permanentRedirect)
1.  [function <span class="apidocSignatureSpan">q-io.redirect.</span>permanentRedirectTree (request, location, status)](#apidoc.element.q-io.redirect.permanentRedirectTree)
1.  [function <span class="apidocSignatureSpan">q-io.redirect.</span>redirectHtml (request, location, status)](#apidoc.element.q-io.redirect.redirectHtml)
1.  [function <span class="apidocSignatureSpan">q-io.redirect.</span>redirectText (request, location, status)](#apidoc.element.q-io.redirect.redirectText)
1.  [function <span class="apidocSignatureSpan">q-io.redirect.</span>redirectTree (request, location, status)](#apidoc.element.q-io.redirect.redirectTree)
1.  [function <span class="apidocSignatureSpan">q-io.redirect.</span>temporaryRedirect (request, location, status)](#apidoc.element.q-io.redirect.temporaryRedirect)
1.  [function <span class="apidocSignatureSpan">q-io.redirect.</span>temporaryRedirectTree (request, location, status)](#apidoc.element.q-io.redirect.temporaryRedirectTree)

#### [module q-io.route](#apidoc.module.q-io.route)
1.  [function <span class="apidocSignatureSpan">q-io.route.</span>Branch (paths, notFound)](#apidoc.element.q-io.route.Branch)
1.  [function <span class="apidocSignatureSpan">q-io.route.</span>Cap (app, notFound)](#apidoc.element.q-io.route.Cap)
1.  [function <span class="apidocSignatureSpan">q-io.route.</span>FirstFound (cascade)](#apidoc.element.q-io.route.FirstFound)
1.  [function <span class="apidocSignatureSpan">q-io.route.</span>Tap (app, tap)](#apidoc.element.q-io.route.Tap)
1.  [function <span class="apidocSignatureSpan">q-io.route.</span>Trap (app, trap)](#apidoc.element.q-io.route.Trap)

#### [module q-io.status](#apidoc.module.q-io.status)
1.  [function <span class="apidocSignatureSpan">q-io.status.</span>appForStatus (status)](#apidoc.element.q-io.status.appForStatus)
1.  [function <span class="apidocSignatureSpan">q-io.status.</span>badRequest (request)](#apidoc.element.q-io.status.badRequest)
1.  [function <span class="apidocSignatureSpan">q-io.status.</span>htmlResponseForStatus (request, status, message, addendum)](#apidoc.element.q-io.status.htmlResponseForStatus)
1.  [function <span class="apidocSignatureSpan">q-io.status.</span>methodNotAllowed (request)](#apidoc.element.q-io.status.methodNotAllowed)
1.  [function <span class="apidocSignatureSpan">q-io.status.</span>noLanguage (request)](#apidoc.element.q-io.status.noLanguage)
1.  [function <span class="apidocSignatureSpan">q-io.status.</span>notAcceptable (request)](#apidoc.element.q-io.status.notAcceptable)
1.  [function <span class="apidocSignatureSpan">q-io.status.</span>notFound (request)](#apidoc.element.q-io.status.notFound)
1.  [function <span class="apidocSignatureSpan">q-io.status.</span>responseForStatus (request, status, addendum)](#apidoc.element.q-io.status.responseForStatus)
1.  [function <span class="apidocSignatureSpan">q-io.status.</span>statusWithNoEntityBody (status)](#apidoc.element.q-io.status.statusWithNoEntityBody)
1.  [function <span class="apidocSignatureSpan">q-io.status.</span>textResponseForStatus (request, status, message, addendum)](#apidoc.element.q-io.status.textResponseForStatus)
1.  object <span class="apidocSignatureSpan">q-io.status.</span>statusCodes
1.  object <span class="apidocSignatureSpan">q-io.status.</span>statusMessages



# <a name="apidoc.module.q-io"></a>[module q-io](#apidoc.module.q-io)

#### <a name="apidoc.element.q-io.buffer_stream"></a>[function <span class="apidocSignatureSpan">q-io.</span>buffer_stream (chunks, charset)](#apidoc.element.q-io.buffer_stream)
- description and source-code
```javascript
function BufferStream(chunks, charset) {
    if (!(this instanceof BufferStream)) {
        return new BufferStream(chunks, charset);
    }
    if (!chunks) {
        chunks = [];
    } else if (!Array.isArray(chunks)) {
        chunks = [chunks];
    }
    this._charset = charset;
    this._chunks = chunks;
    this._close = Q.defer();
    this.closed = this._close.promise;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.q-io.chain"></a>[function <span class="apidocSignatureSpan">q-io.</span>chain (end)](#apidoc.element.q-io.chain)
- description and source-code
```javascript
function Chain(end) {
    var self = Object.create(Chain.prototype);
    self.end = end || function (next) {
        return next;
    };
    return self;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.q-io.reader"></a>[function <span class="apidocSignatureSpan">q-io.</span>reader (_stream, charset)](#apidoc.element.q-io.reader)
- description and source-code
```javascript
function Reader(_stream, charset) {
    var self = Object.create(Reader.prototype);

    if (charset && _stream.setEncoding) // TODO complain about inconsistency
        _stream.setEncoding(charset);

    var begin = Q.defer();
    var end = Q.defer();

    _stream.on("error", function (reason) {
        begin.reject(reason);
    });

    var chunks = [];
    var receiver;

    _stream.on("end", function () {
        begin.resolve(self);
        end.resolve()
    });

    _stream.on("data", function (chunk) {
        begin.resolve(self);
        if (receiver) {
            receiver(chunk);
        } else {
            chunks.push(chunk);
        }
    });

    function slurp() {
        var result;
        if (charset) {
            result = chunks.join("");
        } else {
            result = self.constructor.join(chunks);
        }
        chunks.splice(0, chunks.length);
        return result;
    }

<span class="apidocCodeCommentSpan">    /***
     * Reads all of the remaining data from the stream.
     * @returns {Promise * String} a promise for a String
     * containing the entirety the remaining stream.
     */
</span>    self.read = function () {
        receiver = undefined;
        var deferred = Q.defer();
        Q.done(end.promise, function () {
            deferred.resolve(slurp());
        });
        return deferred.promise;
    };

    /***
     * Reads and writes all of the remaining data from the
     * stream in chunks.
     * @param {Function(Promise * String)} write a function
     * to be called on each chunk of input from this stream.
     * @returns {Promise * Undefined} a promise that will
     * be resolved when the input is depleted.
     */
    self.forEach = function (write) {
        if (chunks && chunks.length)
            write(slurp());
        receiver = write;
        return Q.when(end.promise, function () {
            receiver = undefined;
        });
    };

    self.close = function () {
        _stream.destroy();
    };

    self.node = _stream;

    return begin.promise;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.q-io.buffer_stream"></a>[module q-io.buffer_stream](#apidoc.module.q-io.buffer_stream)

#### <a name="apidoc.element.q-io.buffer_stream.buffer_stream"></a>[function <span class="apidocSignatureSpan">q-io.</span>buffer_stream (chunks, charset)](#apidoc.element.q-io.buffer_stream.buffer_stream)
- description and source-code
```javascript
function BufferStream(chunks, charset) {
    if (!(this instanceof BufferStream)) {
        return new BufferStream(chunks, charset);
    }
    if (!chunks) {
        chunks = [];
    } else if (!Array.isArray(chunks)) {
        chunks = [chunks];
    }
    this._charset = charset;
    this._chunks = chunks;
    this._close = Q.defer();
    this.closed = this._close.promise;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.q-io.buffer_stream.prototype"></a>[module q-io.buffer_stream.prototype](#apidoc.module.q-io.buffer_stream.prototype)

#### <a name="apidoc.element.q-io.buffer_stream.prototype.close"></a>[function <span class="apidocSignatureSpan">q-io.buffer_stream.prototype.</span>close ()](#apidoc.element.q-io.buffer_stream.prototype.close)
- description and source-code
```javascript
close = function () {
    this._close.resolve();
    return Q.resolve();
}
```
- example usage
```shell
...
        }
    } else if (content instanceof Buffer) {
        flags += "b";
    }
    options.flags = flags;
    return Q.when(self.open(path, options), function (stream) {
        return Q.when(stream.write(content), function () {
            return stream.close();
        });
    });
};

/**
 * Append content to the end of a file.
 * @param {String} path    Path to the file.
...
```

#### <a name="apidoc.element.q-io.buffer_stream.prototype.destroy"></a>[function <span class="apidocSignatureSpan">q-io.buffer_stream.prototype.</span>destroy ()](#apidoc.element.q-io.buffer_stream.prototype.destroy)
- description and source-code
```javascript
destroy = function () {
    this._close.resolve();
    return Q.resolve();
}
```
- example usage
```shell
...
        receiver = write;
        return Q.when(end.promise, function () {
            receiver = undefined;
        });
    };

    self.close = function () {
        _stream.destroy();
    };

    self.node = _stream;

    return begin.promise;
}
...
```

#### <a name="apidoc.element.q-io.buffer_stream.prototype.forEach"></a>[function <span class="apidocSignatureSpan">q-io.buffer_stream.prototype.</span>forEach (write, thisp)](#apidoc.element.q-io.buffer_stream.prototype.forEach)
- description and source-code
```javascript
forEach = function (write, thisp) {
    var self = this;
    var chunks = self._chunks;
    return Q.fcall(function () {
        chunks.splice(0, chunks.length).forEach(write, thisp);
    });
}
```
- example usage
```shell
...
this.closed = this._close.promise;
}

BufferStream.prototype.forEach = function (write, thisp) {
var self = this;
var chunks = self._chunks;
return Q.fcall(function () {
    chunks.splice(0, chunks.length).forEach(write, thisp);
});
};

BufferStream.prototype.read = function () {
var result;
result = Reader.join(this._chunks);
if (this._charset) {
...
```

#### <a name="apidoc.element.q-io.buffer_stream.prototype.read"></a>[function <span class="apidocSignatureSpan">q-io.buffer_stream.prototype.</span>read ()](#apidoc.element.q-io.buffer_stream.prototype.read)
- description and source-code
```javascript
read = function () {
    var result;
    result = Reader.join(this._chunks);
    if (this._charset) {
        result = result.toString(this._charset);
    }
    return Q.resolve(result);
}
```
- example usage
```shell
...
into memory.  It returns a promise for the whole file contents.  By
default, 'read' provides a string decoded from UTF-8.  With the bytewise
mode flag, provides a 'Buffer'.

The options argument is identical to that of 'open'.

'''javascript
return FS.read(__filename, "b")
.then(function (content) {
    // ...
})
'''

'''javascript
return FS.read(__filename, {
...
```

#### <a name="apidoc.element.q-io.buffer_stream.prototype.write"></a>[function <span class="apidocSignatureSpan">q-io.buffer_stream.prototype.</span>write (chunk)](#apidoc.element.q-io.buffer_stream.prototype.write)
- description and source-code
```javascript
write = function (chunk) {
    if (this._charset) {
        chunk = new Buffer(String(chunk), this._charset);
    } else {
        if (!(chunk instanceof Buffer)) {
            throw new Error("Can't write strings to buffer stream without a charset: " + chunk);
        }
    }
    this._chunks.push(chunk);
    return Q.resolve();
}
```
- example usage
```shell
...
'write' is a shortcut for opening a file and writing its entire content
from a single string or buffer.

The options are identical to that of 'open', but the "w" flag is
implied, and the "b" flag is implied if the content is a buffer.

'''javascript
return FS.write("hello.txt", "Hello, World!\n")
.then(function () {
    return FS.read("hello.txt")
})
.then(function (hello) {
    expect(hello).toBe("Hello, World!\n")
})
'''
...
```



# <a name="apidoc.module.q-io.chain"></a>[module q-io.chain](#apidoc.module.q-io.chain)

#### <a name="apidoc.element.q-io.chain.chain"></a>[function <span class="apidocSignatureSpan">q-io.</span>chain (end)](#apidoc.element.q-io.chain.chain)
- description and source-code
```javascript
function Chain(end) {
    var self = Object.create(Chain.prototype);
    self.end = end || function (next) {
        return next;
    };
    return self;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.q-io.chain.prototype"></a>[module q-io.chain.prototype](#apidoc.module.q-io.chain.prototype)

#### <a name="apidoc.element.q-io.chain.prototype.use"></a>[function <span class="apidocSignatureSpan">q-io.chain.prototype.</span>use (App)](#apidoc.element.q-io.chain.prototype.use)
- description and source-code
```javascript
use = function (App) {
    if (!App) throw new Error("App is not defined after " + this.app);
    var args = Array.prototype.slice.call(arguments, 1);
    var self = this;
    this.end = (function (End) {
        return function Self(next) {
            if (self.end !== Self && !next) throw new Error("App chain is broken after " + App);
            return End(App.apply(null, [next].concat(args)));
        };
    })(this.end);
    this.app = App;
    return this;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.q-io.content"></a>[module q-io.content](#apidoc.module.q-io.content)

#### <a name="apidoc.element.q-io.content.content"></a>[function <span class="apidocSignatureSpan">q-io.</span>content (content, contentType, status)](#apidoc.element.q-io.content.content)
- description and source-code
```javascript
content = function (content, contentType, status) {
    status = status || 200;
    content = content || "";
    if (typeof content === "string") {
        content = [content];
    }
    contentType = contentType || "text/plain";
    return {
        "status": status,
        "headers": {
            "content-type": contentType
        },
        "body": content
    };
}
```
- example usage
```shell
...
* response body
* @param {String} contentType
* @param {Number} status
* @returns {App} a Q-JSGI app
*/
exports.Content = function (body, contentType, status) {
   return function () {
       return exports.content(body, contentType, status);
   };
};

/**
* Returns a Q-JSGI response with the given content.
* @param {Body} content (optional) defaults to '[""]'
* @param {String} contentType (optional) defaults to '"text/plain"'
...
```

#### <a name="apidoc.element.q-io.content.Content"></a>[function <span class="apidocSignatureSpan">q-io.content.</span>Content (body, contentType, status)](#apidoc.element.q-io.content.Content)
- description and source-code
```javascript
Content = function (body, contentType, status) {
    return function () {
        return exports.content(body, contentType, status);
    };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.q-io.content.ContentRequest"></a>[function <span class="apidocSignatureSpan">q-io.content.</span>ContentRequest (app)](#apidoc.element.q-io.content.ContentRequest)
- description and source-code
```javascript
ContentRequest = function (app) {
    return function (request, response) {
        return Q.when(request.body.read(), function (body) {
            return app(body, request, response);
        });
    };
}
```
- example usage
```shell
...
 * @param {Function(Request, Object):Response} app
 * @param {App} badRequest
 * @returns {App}
 */
exports.JsonRequest = function (app, badRequest) {
if (!badRequest)
    badRequest = Status.badRequest;
return Content.ContentRequest(function (content, request, response) {
    try {
        var object = JSON.parse(content);
    } catch (error) {
        return badRequest(request, error);
    }
    return app(object, request, response);
});
...
```

#### <a name="apidoc.element.q-io.content.Inspect"></a>[function <span class="apidocSignatureSpan">q-io.content.</span>Inspect (app)](#apidoc.element.q-io.content.Inspect)
- description and source-code
```javascript
Inspect = function (app) {
    return Negotiate.Method({"GET": function (request, response) {
        return Q.when(app(request, response), function (object) {
            return {
                status: 200,
                headers: {
                    "content-type": "text/plain"
                },
                body: [inspect(object)]
            }
        });
    }});
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.q-io.content.ParseQuery"></a>[function <span class="apidocSignatureSpan">q-io.content.</span>ParseQuery (app)](#apidoc.element.q-io.content.ParseQuery)
- description and source-code
```javascript
ParseQuery = function (app) {
    return function (request, response) {
        request.query = QS.parse(URL.parse(request.url).query || "");
        return app(request, response);
    };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.q-io.content.ok"></a>[function <span class="apidocSignatureSpan">q-io.content.</span>ok (content, contentType, status)](#apidoc.element.q-io.content.ok)
- description and source-code
```javascript
ok = function (content, contentType, status) {
    status = status || 200;
    content = content || "";
    if (typeof content === "string") {
        content = [content];
    }
    contentType = contentType || "text/plain";
    return {
        "status": status,
        "headers": {
            "content-type": contentType
        },
        "body": content
    };
}
```
- example usage
```shell
...
*/
exports.json = function (content, reviver, tabs) {
   try {
       var json = JSON.stringify(content, reviver, tabs);
   } catch (exception) {
       return Q.reject(exception);
   }
   return Content.ok([json], "application/json");
};

/**
* @param {Function(Request, Object):Response} app
* @param {App} badRequest
* @returns {App}
*/
...
```



# <a name="apidoc.module.q-io.cookie"></a>[module q-io.cookie](#apidoc.module.q-io.cookie)

#### <a name="apidoc.element.q-io.cookie.CookieJar"></a>[function <span class="apidocSignatureSpan">q-io.cookie.</span>CookieJar (app)](#apidoc.element.q-io.cookie.CookieJar)
- description and source-code
```javascript
CookieJar = function (app) {
    var hostCookies = {}; // to {} of pathCookies to [] of cookies
    return function (request) {

        if (!request.headers.host) {
            throw new Error("Requests must have a host header");
        }
        var hosts = allHostsContaining(request.headers.host);

        var now = new Date();

        // delete expired cookies
        for (var host in hostCookies) {
            var pathCookies = hostCookies[host];
            for (var path in pathCookies) {
                var cookies = pathCookies[path];
                for (var name in cookies) {
                    var cookie = cookies[name];
                    if (cookie.expires && cookie.expires > now) {
                        delete cookie[name];
                    }
                }
            }
        }

        // collect applicable cookies
        var requestCookies = concat(
            Object.keys(hostCookies)
            .map(function (host) {
                if (!hostContains(host, request.headers.host)) {
                    return [];
                }
                var pathCookies = hostCookies[host];
                return concat(
                    Object.keys(pathCookies)
                    .map(function (path) {
                        if (!pathContains(path, request.path))
                            return [];
                        var cookies = pathCookies[path];
                        return (
                            Object.keys(cookies)
                            .map(function (name) {
                                return cookies[name];
                            })
                            .filter(function (cookie) {
                                return cookie.secure ?
                                    request.ssl :
                                    true;
                            })
                        );
                    })
                )
            })
        );

        if (requestCookies.length) {
            request.headers["cookie"] = (
                requestCookies
                .map(function (cookie) {
                    return Cookie.stringify(
                        cookie.key,
                        cookie.value
                    );
                })
                .join("; ")
            );
        }

        return Q.when(app.apply(this, arguments), function (response) {
            response.headers = response.headers || {};
            if (response.headers["set-cookie"]) {
                var host = request.headers.host;
                var hostParts = splitHost(host);
                var hostname = hostParts[0];
                var requestHost = ipRe.test(hostname) ? host : "." + host;
                // normalize to array
                if (!Array.isArray(response.headers["set-cookie"])) {
                    response.headers["set-cookie"] = [response.headers["set-cookie"]];
                }
                response.headers["set-cookie"].forEach(function (cookie) {
                    var date = response.headers["date"] ?
                        new Date(response.headers["date"]) :
                        new Date();
                    cookie = Cookie.parse(cookie, date);
                    // ignore illegal host
                    if (cookie.host && !hostContains(requestHost, cookie.host))
                        delete cookie.host;
                    var host = requestHost || cookie.host;
                    var path = cookie.path || "/";
                    var pathCookies = hostCookies[host] = hostCookies[host] || {};
                    var cookies = pathCookies[path] = pathCookies[path] || {};
                    cookies[cookie.key] = cookie;
                })
                delete response.headers["set-cookie"];
            }

            return response;
        });

    };
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.q-io.decorators"></a>[module q-io.decorators](#apidoc.module.q-io.decorators)

#### <a name="apidoc.element.q-io.decorators.Date"></a>[function <span class="apidocSignatureSpan">q-io.decorators.</span>Date (app, present)](#apidoc.element.q-io.decorators.Date)
- description and source-code
```javascript
Date = function (app, present) {
    present = present || function () {
        return new Date();
    };
    return RouteApps.Trap(app, function (response, request) {
        response.headers["date"] = "" + present();
    });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.q-io.decorators.Debug"></a>[function <span class="apidocSignatureSpan">q-io.decorators.</span>Debug (app)](#apidoc.element.q-io.decorators.Debug)
- description and source-code
```javascript
Debug = function (app) {
    return exports.Error(app, true);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.q-io.decorators.Decorators"></a>[function <span class="apidocSignatureSpan">q-io.decorators.</span>Decorators (decorators, app)](#apidoc.element.q-io.decorators.Decorators)
- description and source-code
```javascript
Decorators = function (decorators, app) {
    decorators.reversed().forEach(function (Middleware) {
        app = Middleware(app);
    });
    return app;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.q-io.decorators.Error"></a>[function <span class="apidocSignatureSpan">q-io.decorators.</span>Error (app, debug)](#apidoc.element.q-io.decorators.Error)
- description and source-code
```javascript
Error = function (app, debug) {
    return function (request, response) {
        return Q.when(app(request, response), null, function (error) {
            if (!debug)
                error = undefined;
            return StatusApps.responseForStatus(request, 500, error && error.stack || error);
        });
    };
}
```
- example usage
```shell
...
               error = undefined;
           return StatusApps.responseForStatus(request, 500, error && error.stack || error);
       });
   };
};

exports.Debug = function (app) {
   return exports.Error(app, true);
};

/**
* Decorates a Q-JSGI application such that all requests and responses
* are logged.
*
* @param {App} app
...
```

#### <a name="apidoc.element.q-io.decorators.Headers"></a>[function <span class="apidocSignatureSpan">q-io.decorators.</span>Headers (app, headers)](#apidoc.element.q-io.decorators.Headers)
- description and source-code
```javascript
Headers = function (app, headers) {
    return function (request, response) {
        return Q.when(app(request, response), function (response) {
            if (response && response.headers) {
                Object.keys(headers).forEach(function (key) {
                    if (!(key in response.headers)) {
                        response.headers[key] = headers[key];
                    }
                });
            }
            return response;
        });
    };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.q-io.decorators.Log"></a>[function <span class="apidocSignatureSpan">q-io.decorators.</span>Log (app, log, stamp)](#apidoc.element.q-io.decorators.Log)
- description and source-code
```javascript
Log = function (app, log, stamp) {
    log = log || console.log;
    stamp = stamp || function (message) {
        return new Date().toISOString() + " " + message;
    };
    return function (request, response) {
        var remoteHost =
            request.remoteHost + ":" +
            request.remotePort;
        var requestLine =
            request.method + " " +
            request.path + " " +
            "HTTP/" + request.version.join(".");
        log(stamp(
            remoteHost + " " +
            "-->     " +
            requestLine
        ));
        return Q.when(app(request, response), function (response) {
            if (response) {
                log(stamp(
                    remoteHost + " " +
                    "<== " +
                    response.status + " " +
                    requestLine + " " +
                    (response.headers["content-length"] || "-")
                ));
            } else {
                log(stamp(
                    remoteHost + " " +
                    "... " +
                    "... " +
                    requestLine + " (response undefined / presumed streaming)"
                ));
            }
            return response;
        }, function (reason) {
            log(stamp(
                remoteHost + " " +
                "!!!     " +
                requestLine + " " +
                (reason && reason.message || reason)
            ));
            return Q.reject(reason);
        });
    };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.q-io.decorators.Normalize"></a>[function <span class="apidocSignatureSpan">q-io.decorators.</span>Normalize (app)](#apidoc.element.q-io.decorators.Normalize)
- description and source-code
```javascript
Normalize = function (app) {
    return function (request, response) {
        var request = HTTP.normalizeRequest(request);
        return Q.when(app(request, response), function (response) {
            return HTTP.normalizeResponse(response);
        });
    };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.q-io.decorators.Permanent"></a>[function <span class="apidocSignatureSpan">q-io.decorators.</span>Permanent (app, future)](#apidoc.element.q-io.decorators.Permanent)
- description and source-code
```javascript
Permanent = function (app, future) {
    future = future || function () {
        return new Date(new Date().getTime() + farFuture);
    };
    app = RouteApps.Tap(app, function (request, response) {
        request.permanent = future;
    });
    app = RouteApps.Trap(app, function (response, request) {
        response.headers["expires"] = "" + future();
    });
    return app;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.q-io.decorators.Time"></a>[function <span class="apidocSignatureSpan">q-io.decorators.</span>Time (app)](#apidoc.element.q-io.decorators.Time)
- description and source-code
```javascript
Time = function (app) {
    return function (request, response) {
        var start = new Date();
        return Q.when(app(request, response), function (response) {
            var stop = new Date();
            if (response && response.headers) {
                response.headers["x-response-time"] = "" + (stop - start);
            }
            return response;
        });
    };
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.q-io.deprecate"></a>[module q-io.deprecate](#apidoc.module.q-io.deprecate)

#### <a name="apidoc.element.q-io.deprecate.deprecateMethod"></a>[function <span class="apidocSignatureSpan">q-io.deprecate.</span>deprecateMethod (scope, deprecatedFunction, name, alternative)](#apidoc.element.q-io.deprecate.deprecateMethod)
- description and source-code
```javascript
function deprecate(scope, deprecatedFunction, name, alternative) {
    var deprecationWrapper = function () {
        // stackTraceLimit = 3 // deprecationWarning + deprecate + caller of the deprecated method
        deprecationWarning(name, alternative, 3);
        return deprecatedFunction.apply(scope ? scope : this, arguments);
    };
    deprecationWrapper.deprecatedFunction = deprecatedFunction;
    return deprecationWrapper;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.q-io.deprecate.deprecationWarning"></a>[function <span class="apidocSignatureSpan">q-io.deprecate.</span>deprecationWarning (name, alternative, stackTraceLimit)](#apidoc.element.q-io.deprecate.deprecationWarning)
- description and source-code
```javascript
function deprecationWarning(name, alternative, stackTraceLimit) {
    if (stackTraceLimit) {
        var depth = Error.stackTraceLimit;
        Error.stackTraceLimit = stackTraceLimit;
    }
    if (typeof console !== "undefined" && typeof console.warn === "function") {
        var stack = (stackTraceLimit ? new Error("").stack : "") ;
        if(alternative) {
            console.warn(name + " is deprecated, use " + alternative + " instead.", stack);
        } else {
            //name is a complete message
            console.warn(name, stack);
        }
    }
    if (stackTraceLimit) {
        Error.stackTraceLimit = depth;
    }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.q-io.fs"></a>[module q-io.fs](#apidoc.module.q-io.fs)

#### <a name="apidoc.element.q-io.fs.Mock"></a>[function <span class="apidocSignatureSpan">q-io.fs.</span>Mock (files, workingDirectory)](#apidoc.element.q-io.fs.Mock)
- description and source-code
```javascript
function MockFs(files, workingDirectory) {
    if (!(this instanceof MockFs)) {
        return new MockFs(files, workingDirectory);
    }
    this._root = new DirectoryNode(this, "/");

    function init() {
        // construct a file tree
    }

    Common.update(this, function () {
        return workingDirectory;
    });

    workingDirectory = workingDirectory || this.ROOT;
    if (files) {
        this._init(files);
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.q-io.fs.Root"></a>[function <span class="apidocSignatureSpan">q-io.fs.</span>Root (outer, root)](#apidoc.element.q-io.fs.Root)
- description and source-code
```javascript
function RootFs(outer, root) {
    var inner = Object.create(BOOT);

    function attenuate(path) {

        // the machinations of projecting a path inside a
        // subroot
        var actual;
        // if it's absolute, we want the path relative to
        // the root of the inner file system
        if (outer.isAbsolute(path)) {
            actual = outer.relativeFromDirectory(outer.ROOT, path);
        } else {
            actual = path;
        }
        // we join the path onto the root of the inner file
        // system so that parent references from the root
        // return to the root, emulating standard unix
        // behavior
        actual = outer.join(outer.ROOT, actual);
        // then we reconstruct the path relative to the
        // inner root
        actual = outer.relativeFromDirectory(outer.ROOT, actual);
        // and rejoin it on the outer root
        actual = outer.join(root, actual);
        // and find the corresponding real path
        return outer.canonical(actual)
        .then(function (actual) {
            return actual;
        }, function () {
            return actual;
        }).then(function (actual) {
            // and verify that the outer canonical path is
            // actually inside the inner canonical path, to
            // prevent break-outs
            if (outer.contains(root, actual)) {
                return {
                    "inner": outer.join(outer.ROOT, outer.relativeFromDirectory(root, actual)),
                    "outer": actual
                };
            } else {
                return Q.reject("Can't find: " + JSON.stringify(path));
            }
        });
    }

    function workingDirectory() {
        return outer.ROOT;
    }

    COMMON.update(inner, workingDirectory);

    inner.list = function (path) {
        return attenuate(path).then(function (path) {
            return outer.list(path.outer);
        }).then(null, function (reason) {
            return Q.reject("Can't list " + JSON.stringify(path));
        });
    };

    inner.open = function (path, flags, charset) {
        return attenuate(path).then(function (path) {
            return outer.open(path.outer, flags, charset);
        }).then(null, function (reason) {
            return Q.reject("Can't open " + JSON.stringify(path));
        });
    };

    inner.stat = function (path) {
        return attenuate(path).then(function (path) {
            return outer.stat(path.outer);
        }).then(null, function (reason) {
            return Q.reject("Can't stat " + JSON.stringify(path));
        });
    };

    inner.statLink = function (path) {
        return attenuate(path).then(function (path) {
            return outer.statLink(path.outer);
        }).then(null, function (reason) {
            return Q.reject("Can't statLink " + JSON.stringify(path));
        });
    };

    inner.canonical = function (path) {
        return attenuate(path).then(function (path) {
            return path.inner;
        }).then(null, function (reason) {
            return Q.reject("Can't find canonical of " + JSON.stringify(path));
        });
    };

    inner.makeDirectory = function (path) {
        return attenuate(path).then(function (path) {
            return outer.makeDirectory(path.outer);
        }).catch(function (error) {
            throw new Error("Can't make directory " + JSON.stringify(path));
        });
    };

    inner.removeDirectory = function (path) {
        return attenuate(path).then(function (path) {
            return outer.removeDirectory(path.outer);
        }).catch(function (error) {
            throw new Error("Can't remove directory " + JSON.stringify(path));
        });
    };

    inner.remove = function (path) {
        return attenuate(path).then(function (path) {
            return outer.remove(path.outer);
        }).catch(function (error) {
            throw new Error("Can't remove " + JSON.stringify(path));
        });
    };

    inner.makeTree = function (path) {
        return attenuate(path).then(function (path) {
            return outer.makeT ...
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.q-io.fs.SEPARATORS_RE"></a>[function <span class="apidocSignatureSpan">q-io.fs.</span>SEPARATORS_RE ()](#apidoc.element.q-io.fs.SEPARATORS_RE)
- description and source-code
```javascript
SEPARATORS_RE = function () {
    if (
        separatorCached !== exports.SEPARATOR ||
        altSeparatorCached !== exports.ALT_SEPARATOR
    ) {
        separatorCached = exports.SEPARATOR;
        altSeparatorCached = exports.ALT_SEPARATOR;
        separatorReCached = new RegExp("[" +
            (separatorCached || "").replace(/[-[\]{}()*+?.\\^$|,#\s]/g, "\\$&") +
            (altSeparatorCached || "").replace(/[-[\]{}()*+?.\\^$|,#\s]/g, "\\$&") +
        "]", "g");
    }
    return separatorReCached;
}
```
- example usage
```shell
...
 * file system, indicated by an empty string on Unix, and a
 * drive letter followed by a colon on Windows.
 * @returns {Array * String}
 */
exports.split = function (path) {
var parts;
try {
    parts = String(path).split(exports.SEPARATORS_RE());
} catch (exception) {
    throw new Error("Cannot split " + (typeof path) + ", " + JSON.stringify(path));
}
// this special case helps isAbsolute
// distinguish an empty path from an absolute path
// "" -> [] NOT [""]
if (parts.length === 1 && parts[0] === "")
...
```

#### <a name="apidoc.element.q-io.fs.Stats"></a>[function <span class="apidocSignatureSpan">q-io.fs.</span>Stats (nodeStat)](#apidoc.element.q-io.fs.Stats)
- description and source-code
```javascript
function Stats(nodeStat) {
    this.node = nodeStat;
    this.size = nodeStat.size;
}
```
- example usage
```shell
...
    var done = Q.defer();
    try {
        FS.stat(path, function (error, stat) {
            if (error) {
                error.message = "Can't stat " + JSON.stringify(path) + ": " + error;
                done.reject(error);
            } else {
                done.resolve(new self.Stats(stat));
            }
        });
    } catch (error) {
        done.reject(error);
    }
    return done.promise;
};
...
```

#### <a name="apidoc.element.q-io.fs.absolute"></a>[function <span class="apidocSignatureSpan">q-io.fs.</span>absolute (path)](#apidoc.element.q-io.fs.absolute)
- description and source-code
```javascript
absolute = function (path) {
    if (this.isAbsolute(path))
        return this.normal(path);
    return this.join(workingDirectory(), path);
}
```
- example usage
```shell
...

/**
* @returns {String} the Unix root path or corresponding
* Windows drive for a given path.
*/
exports.root = function (path) {
   if (!exports.isAbsolute(path))
       path = require("./fs").absolute(path);
   var parts = exports.split(path);
   return exports.join(parts[0], "");
};

/**
* @returns {String} the parent directory of the given path.
*/
...
```

#### <a name="apidoc.element.q-io.fs.append"></a>[function <span class="apidocSignatureSpan">q-io.fs.</span>append (path, content, flags, charset, options)](#apidoc.element.q-io.fs.append)
- description and source-code
```javascript
append = function (path, content, flags, charset, options) {
    var self = this;
    if (typeof flags === "object") {
        options = flags;
    } else if (typeof charset === "object") {
        options = charset;
        options.flags = flags;
    } else {
        options = options || {};
        options.flags = flags;
        options.charset = charset;
    }
    flags = options.flags || "a";
    if (content instanceof Buffer) {
        flags += "b";
    }
    options.flags = flags;
    return Q.when(self.open(path, options), function (stream) {
        return Q.when(stream.write(content), function () {
            return stream.close();
        });
    });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.q-io.fs.base"></a>[function <span class="apidocSignatureSpan">q-io.fs.</span>base (path, extension)](#apidoc.element.q-io.fs.base)
- description and source-code
```javascript
base = function (path, extension) {
    var base = path.split(exports.SEPARATORS_RE()).pop();
    if (extension)
        base = base.replace(
            new RegExp(regExpEscape(extension) + "$"),
            ""
        );
    return base;
}
```
- example usage
```shell
...
};

/**
 * @returns {String} the extension (e.g., 'txt') of the file
 * at the given path.
 */
exports.extension = function (path) {
    path = exports.base(path);
    path = path.replace(/^\.*/, "");
    var index = path.lastIndexOf(".");
    return index <= 0 ? "" : path.substring(index);
};

})(typeof exports !== "undefined" ? exports : FS_BOOT = {});
...
```

#### <a name="apidoc.element.q-io.fs.canonical"></a>[function <span class="apidocSignatureSpan">q-io.fs.</span>canonical (path)](#apidoc.element.q-io.fs.canonical)
- description and source-code
```javascript
canonical = function (path) {
    var result = Q.defer();
    FS.realpath(path, function (error, canonicalPath) {
        if (error) {
            error.message = "Can't get canonical path of " + JSON.stringify(path) + " by way of C realpath: " + error.message;
            result.reject(error);
        } else {
            result.resolve(canonicalPath);
        }
    });
    return result.promise;
}
```
- example usage
```shell
...
actual = outer.join(outer.ROOT, actual);
// then we reconstruct the path relative to the
// inner root
actual = outer.relativeFromDirectory(outer.ROOT, actual);
// and rejoin it on the outer root
actual = outer.join(root, actual);
// and find the corresponding real path
return outer.canonical(actual)
.then(function (actual) {
    return actual;
}, function () {
    return actual;
}).then(function (actual) {
    // and verify that the outer canonical path is
    // actually inside the inner canonical path, to
...
```

#### <a name="apidoc.element.q-io.fs.chmod"></a>[function <span class="apidocSignatureSpan">q-io.fs.</span>chmod (path, mode)](#apidoc.element.q-io.fs.chmod)
- description and source-code
```javascript
chmod = function (path, mode) {
    path = String(path);
    mode = String(mode);
    var done = Q.defer();
    try {
        FS.chmod(path, mode, function (error) {
            if (error) {
                error.message = "Can't chmod (change permissions mode) of " + JSON.stringify(path) + " to (octal number) " + mode
.toString(8) + ": " + error.message;
                done.reject(error);
            } else {
                done.resolve();
            }
        });
    } catch (error) {
        done.reject(error);
    }
    return done.promise;
}
```
- example usage
```shell
...
};

exports.chmod = function (path, mode) {
path = String(path);
mode = String(mode);
var done = Q.defer();
try {
    FS.chmod(path, mode, function (error) {
        if (error) {
            error.message = "Can't chmod (change permissions mode) of " + JSON.stringify(path) + " to (octal number) " + mode.toString
(8) + ": " + error.message;
            done.reject(error);
        } else {
            done.resolve();
        }
    });
...
```

#### <a name="apidoc.element.q-io.fs.chown"></a>[function <span class="apidocSignatureSpan">q-io.fs.</span>chown (path, uid, gid)](#apidoc.element.q-io.fs.chown)
- description and source-code
```javascript
chown = function (path, uid, gid) {
    path = String(path);
    var done = Q.defer();
    try {
        FS.chown(path, uid, gid, function (error) {
            if (error) {
                error.message = "Can't chown (change owner) of " + JSON.stringify(path) + " to user " + JSON.stringify(uid) + "
and group " + JSON.stringify(gid) + ": " + error.message;
                done.reject(error);
            } else {
                done.resolve();
            }
        });
    } catch (error) {
        done.reject(error);
    }
    return done.promise;
}
```
- example usage
```shell
...
return done.promise;
};

exports.chown = function (path, uid, gid) {
path = String(path);
var done = Q.defer();
try {
    FS.chown(path, uid, gid, function (error) {
        if (error) {
            error.message = "Can't chown (change owner) of " + JSON.stringify(path) + " to user " + JSON.stringify(uid) + " and
group " + JSON.stringify(gid) + ": " + error.message;
            done.reject(error);
        } else {
            done.resolve();
        }
    });
...
```

#### <a name="apidoc.element.q-io.fs.contains"></a>[function <span class="apidocSignatureSpan">q-io.fs.</span>contains (parent, child)](#apidoc.element.q-io.fs.contains)
- description and source-code
```javascript
contains = function (parent, child) {
    var i, ii;
    parent = this.absolute(parent);
    child = this.absolute(child);
    parent = parent.split(this.SEPARATORS_RE());
    child = child.split(this.SEPARATORS_RE());
    if (parent.length === 2 && parent[1] === "")
        parent.pop();
    if (parent.length > child.length)
        return false;
    for (i = 0, ii = parent.length; i < ii; i++) {
        if (parent[i] !== child[i])
            break;
    }
    return i == ii;
}
```
- example usage
```shell
...
    return actual;
}, function () {
    return actual;
}).then(function (actual) {
    // and verify that the outer canonical path is
    // actually inside the inner canonical path, to
    // prevent break-outs
    if (outer.contains(root, actual)) {
        return {
            "inner": outer.join(outer.ROOT, outer.relativeFromDirectory(root, actual)),
            "outer": actual
        };
    } else {
        return Q.reject("Can't find: " + JSON.stringify(path));
    }
...
```

#### <a name="apidoc.element.q-io.fs.copy"></a>[function <span class="apidocSignatureSpan">q-io.fs.</span>copy (source, target)](#apidoc.element.q-io.fs.copy)
- description and source-code
```javascript
copy = function (source, target) {
    var self = this;
    return Q.when(self.stat(source), function (stat) {
        var mode = stat.node.mode;
        return Q.all([
            self.open(source, {flags: "rb"}),
            self.open(target, {flags: "wb", mode: mode})
        ]);
    })
    .spread(function (reader, writer) {
        return Q.when(reader.forEach(function (block) {
            return writer.write(block);
        }), function () {
            return Q.all([
                reader.close(),
                writer.close()
            ]);
        });
    });
}
```
- example usage
```shell
...
    });
};

exports.copyTree = function (source, target) {
    var self = this;
    return Q.when(self.stat(source), function (stat) {
        if (stat.isFile()) {
            return self.copy(source, target);
        } else if (stat.isDirectory()) {
            return self.exists(target).then(function (targetExists) {
                function copySubTree() {
                    return Q.when(self.list(source), function (list) {
                        return Q.all(list.map(function (child) {
                            return self.copyTree(
                                self.join(source, child),
...
```

#### <a name="apidoc.element.q-io.fs.copyTree"></a>[function <span class="apidocSignatureSpan">q-io.fs.</span>copyTree (source, target)](#apidoc.element.q-io.fs.copyTree)
- description and source-code
```javascript
copyTree = function (source, target) {
    var self = this;
    return Q.when(self.stat(source), function (stat) {
        if (stat.isFile()) {
            return self.copy(source, target);
        } else if (stat.isDirectory()) {
            return self.exists(target).then(function (targetExists) {
                function copySubTree() {
                    return Q.when(self.list(source), function (list) {
                        return Q.all(list.map(function (child) {
                            return self.copyTree(
                                self.join(source, child),
                                self.join(target, child)
                            );
                        }));
                    });
                }
                if (targetExists) {
                    return copySubTree();
                } else {
                    return Q.when(self.makeDirectory(target, stat.node.mode), copySubTree);
                }
            });
        } else if (stat.isSymbolicLink()) {
            // TODO copy the link and type with readPath (but what about
            // Windows junction type?)
            return self.symbolicCopy(source, target);
        }
    });
}
```
- example usage
```shell
...
};

exports.move = function (source, target) {
    var self = this;
    return this.rename(source, target)
    .catch(function (error) {
        if (error.crossDevice) {
            return self.copyTree(source, target)
            .then(function () {
                return self.removeTree(source);
            });
        } else {
            throw error;
        }
    });
...
```

#### <a name="apidoc.element.q-io.fs.directory"></a>[function <span class="apidocSignatureSpan">q-io.fs.</span>directory (path)](#apidoc.element.q-io.fs.directory)
- description and source-code
```javascript
directory = function (path) {
    path = exports.normal(path);
    var absolute = exports.isAbsolute(path);
    var parts = exports.split(path);
    // XXX needs to be sensitive to the root for
    // Windows compatibility
    if (parts.length) {
        if (parts[parts.length - 1] == "..") {
            parts.push("..");
        } else {
            parts.pop();
        }
    } else {
        parts.unshift("..");
    }
    return parts.join(exports.SEPARATOR) || (
        exports.isRelative(path) ?
        "" : exports.ROOT
    );
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.q-io.fs.exists"></a>[function <span class="apidocSignatureSpan">q-io.fs.</span>exists (path)](#apidoc.element.q-io.fs.exists)
- description and source-code
```javascript
exists = function (path) {
    return Q.when(this.stat(path), function () {
        return true;
    }, function () {
        return false;
    });
}
```
- example usage
```shell
...

    exports.copyTree = function (source, target) {
var self = this;
return Q.when(self.stat(source), function (stat) {
    if (stat.isFile()) {
        return self.copy(source, target);
    } else if (stat.isDirectory()) {
        return self.exists(target).then(function (targetExists) {
            function copySubTree() {
                return Q.when(self.list(source), function (list) {
                    return Q.all(list.map(function (child) {
                        return self.copyTree(
                            self.join(source, child),
                            self.join(target, child)
                        );
...
```

#### <a name="apidoc.element.q-io.fs.extension"></a>[function <span class="apidocSignatureSpan">q-io.fs.</span>extension (path)](#apidoc.element.q-io.fs.extension)
- description and source-code
```javascript
extension = function (path) {
    path = exports.base(path);
    path = path.replace(/^\.*/, "");
    var index = path.lastIndexOf(".");
    return index <= 0 ? "" : path.substring(index);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.q-io.fs.isAbsolute"></a>[function <span class="apidocSignatureSpan">q-io.fs.</span>isAbsolute (path)](#apidoc.element.q-io.fs.isAbsolute)
- description and source-code
```javascript
isAbsolute = function (path) {
    // for absolute paths on any operating system,
    // the first path component always determines
    // whether it is relative or absolute.  On Unix,
    // it is empty, so ["", "foo"].join("/") == "/foo",
    // "/foo".split("/") == ["", "foo"].
    var parts = exports.split(path);
    // split("") == [].  "" is not absolute.
    // split("/") == ["", ""] is absolute.
    // split(?) == [""] does not occur.
    if (parts.length == 0)
        return false;
    return exports.isRoot(parts[0]);
}
```
- example usage
```shell
...
var children = [];
var leaf = "";
for (var i = 0; i < arguments.length; i++) {
    var path = String(arguments[i]);
    if (path == "")
        continue;
    var parts = path.split(exports.SEPARATORS_RE());
    if (exports.isAbsolute(path)) {
        root = parts.shift() + exports.SEPARATOR;
        parents = [];
        children = [];
    }
    leaf = parts.pop();
    if (leaf == "." || leaf == "..") {
        parts.push(leaf);
...
```

#### <a name="apidoc.element.q-io.fs.isDirectory"></a>[function <span class="apidocSignatureSpan">q-io.fs.</span>isDirectory (path)](#apidoc.element.q-io.fs.isDirectory)
- description and source-code
```javascript
isDirectory = function (path) {
    return Q.when(this.stat(path), function (stat) {
        return stat.isDirectory();
    }, function (reason) {
        return false;
    });
}
```
- example usage
```shell
...
};

exports.copyTree = function (source, target) {
    var self = this;
    return Q.when(self.stat(source), function (stat) {
        if (stat.isFile()) {
            return self.copy(source, target);
        } else if (stat.isDirectory()) {
            return self.exists(target).then(function (targetExists) {
                function copySubTree() {
                    return Q.when(self.list(source), function (list) {
                        return Q.all(list.map(function (child) {
                            return self.copyTree(
                                self.join(source, child),
                                self.join(target, child)
...
```

#### <a name="apidoc.element.q-io.fs.isFile"></a>[function <span class="apidocSignatureSpan">q-io.fs.</span>isFile (path)](#apidoc.element.q-io.fs.isFile)
- description and source-code
```javascript
isFile = function (path) {
    return Q.when(this.stat(path), function (stat) {
        return stat.isFile();
    }, function (reason) {
        return false;
    });
}
```
- example usage
```shell
...
        });
    });
};

exports.copyTree = function (source, target) {
    var self = this;
    return Q.when(self.stat(source), function (stat) {
        if (stat.isFile()) {
            return self.copy(source, target);
        } else if (stat.isDirectory()) {
            return self.exists(target).then(function (targetExists) {
                function copySubTree() {
                    return Q.when(self.list(source), function (list) {
                        return Q.all(list.map(function (child) {
                            return self.copyTree(
...
```

#### <a name="apidoc.element.q-io.fs.isRelative"></a>[function <span class="apidocSignatureSpan">q-io.fs.</span>isRelative (path)](#apidoc.element.q-io.fs.isRelative)
- description and source-code
```javascript
isRelative = function (path) {
    return !exports.isAbsolute(path);
}
```
- example usage
```shell
...
       } else {
           parts.pop();
       }
   } else {
       parts.unshift("..");
   }
   return parts.join(exports.SEPARATOR) || (
       exports.isRelative(path) ?
       "" : exports.ROOT
   );
};

/**
* @returns {String} the last component of a path, without
* the given extension if the extension is provided and
...
```

#### <a name="apidoc.element.q-io.fs.isRoot"></a>[function <span class="apidocSignatureSpan">q-io.fs.</span>isRoot (first)](#apidoc.element.q-io.fs.isRoot)
- description and source-code
```javascript
isRoot = function (first) {
    if (exports.SEPARATOR === "\\") {
        return /[a-zA-Z]:$/.test(first);
    } else {
        return first == "";
    }
}
```
- example usage
```shell
...
    // "/foo".split("/") == ["", "foo"].
    var parts = exports.split(path);
    // split("") == [].  "" is not absolute.
    // split("/") == ["", ""] is absolute.
    // split(?) == [""] does not occur.
    if (parts.length == 0)
        return false;
    return exports.isRoot(parts[0]);
};

/**
 * @returns {Boolean} whether the given path does not begin
 * at the root of the file system or a drive letter.
 */
exports.isRelative = function (path) {
...
```

#### <a name="apidoc.element.q-io.fs.isSymbolicLink"></a>[function <span class="apidocSignatureSpan">q-io.fs.</span>isSymbolicLink (path)](#apidoc.element.q-io.fs.isSymbolicLink)
- description and source-code
```javascript
isSymbolicLink = function (path) {
    return Q.when(this.statLink(path), function (stat) {
        return stat.isSymbolicLink();
    }, function (reason) {
        return false;
    });
}
```
- example usage
```shell
...
                }
                if (targetExists) {
                    return copySubTree();
                } else {
                    return Q.when(self.makeDirectory(target, stat.node.mode), copySubTree);
                }
            });
        } else if (stat.isSymbolicLink()) {
            // TODO copy the link and type with readPath (but what about
            // Windows junction type?)
            return self.symbolicCopy(source, target);
        }
    });
};
...
```

#### <a name="apidoc.element.q-io.fs.join"></a>[function <span class="apidocSignatureSpan">q-io.fs.</span>join ()](#apidoc.element.q-io.fs.join)
- description and source-code
```javascript
join = function () {
    if (arguments.length === 1 && Array.isArray(arguments[0]))
        return exports.normal.apply(exports, arguments[0]);
    return exports.normal.apply(exports, arguments);
}
```
- example usage
```shell
...
    return Q.fcall(function () {
        chunks.splice(0, chunks.length).forEach(write, thisp);
    });
};

BufferStream.prototype.read = function () {
    var result;
    result = Reader.join(this._chunks);
    if (this._charset) {
        result = result.toString(this._charset);
    }
    return Q.resolve(result);
};

BufferStream.prototype.write = function (chunk) {
...
```

#### <a name="apidoc.element.q-io.fs.lastAccessed"></a>[function <span class="apidocSignatureSpan">q-io.fs.</span>lastAccessed (path)](#apidoc.element.q-io.fs.lastAccessed)
- description and source-code
```javascript
lastAccessed = function (path) {
    var self = this;
    return self.stat(path).invoke('lastAccessed');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.q-io.fs.lastModified"></a>[function <span class="apidocSignatureSpan">q-io.fs.</span>lastModified (path)](#apidoc.element.q-io.fs.lastModified)
- description and source-code
```javascript
lastModified = function (path) {
    var self = this;
    return self.stat(path).invoke('lastModified');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.q-io.fs.link"></a>[function <span class="apidocSignatureSpan">q-io.fs.</span>link (source, target)](#apidoc.element.q-io.fs.link)
- description and source-code
```javascript
link = function (source, target) {
    source = String(source);
    target = String(target);
    var done = Q.defer();
    try {
        FS.link(source, target, function (error) {
            if (error) {
                error.message = "Can't link " + JSON.stringify(source) + " to " + JSON.stringify(target) + ": " + error.message;
                done.reject(error);
            } else {
                done.resolve();
            }
        });
    } catch (error) {
        done.reject(error);
    }
    return done.promise;
}
```
- example usage
```shell
...
};

exports.link = function (source, target) {
source = String(source);
target = String(target);
var done = Q.defer();
try {
    FS.link(source, target, function (error) {
        if (error) {
            error.message = "Can't link " + JSON.stringify(source) + " to " + JSON.stringify(target) + ": " + error.message;
            done.reject(error);
        } else {
            done.resolve();
        }
    });
...
```

#### <a name="apidoc.element.q-io.fs.list"></a>[function <span class="apidocSignatureSpan">q-io.fs.</span>list ()](#apidoc.element.q-io.fs.list)
- description and source-code
```javascript
list = function () {
    var args = arguments;
    var ready = backOffDelay ? Q.delay(backOffDelay) : Q.resolve();
    return ready.then(function () {
        return Q.when(wrapped.apply(thisp, args), function (stream) {
            backOffDelay = Math.max(0, backOffDelay - 1);
            return stream;
        }, function (error) {
            if (error.code === "EMFILE") {
                backOffDelay = (backOffDelay + 1) * backOffFactor;
                return retry.apply(null, args);
            } else {
                throw error;
            }
        });
    });
}
```
- example usage
```shell
...
var self = this;
return Q.when(self.stat(source), function (stat) {
    if (stat.isFile()) {
        return self.copy(source, target);
    } else if (stat.isDirectory()) {
        return self.exists(target).then(function (targetExists) {
            function copySubTree() {
                return Q.when(self.list(source), function (list) {
                    return Q.all(list.map(function (child) {
                        return self.copyTree(
                            self.join(source, child),
                            self.join(target, child)
                        );
                    }));
                });
...
```

#### <a name="apidoc.element.q-io.fs.listDirectoryTree"></a>[function <span class="apidocSignatureSpan">q-io.fs.</span>listDirectoryTree (path)](#apidoc.element.q-io.fs.listDirectoryTree)
- description and source-code
```javascript
listDirectoryTree = function (path) {
    return this.listTree(path, function (path, stat) {
        return stat.isDirectory();
    });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.q-io.fs.listTree"></a>[function <span class="apidocSignatureSpan">q-io.fs.</span>listTree (basePath, guard)](#apidoc.element.q-io.fs.listTree)
- description and source-code
```javascript
listTree = function (basePath, guard) {
    var self = this;
    basePath = String(basePath || '');
    if (!basePath)
        basePath = ".";
    guard = guard || function () {
        return true;
    };
    var stat = self.stat(basePath);
    return Q.when(stat, function (stat) {
        var paths = [];
        var mode; // true:include, false:exclude, null:no-recur
        try {
            var include = guard(basePath, stat);
        } catch (exception) {
            return Q.reject(exception);
        }
        return Q.when(include, function (include) {
            if (include) {
                paths.push([basePath]);
            }
            if (include !== null && stat.isDirectory()) {
                return Q.when(self.list(basePath), function (children) {
                    paths.push.apply(paths, children.map(function (child) {
                        var path = self.join(basePath, child);
                        return self.listTree(path, guard);
                    }));
                    return paths;
                });
            } else {
                return paths;
            }
        });
    }, function noSuchFile(reason) {
        return [];
    }).then(Q.all).then(concat);
}
```
- example usage
```shell
...



require("collections/shim");
var Q = require("q");
var FS = require("./fs");

FS.listTree(".coverage_data", function (name, stat) {
return (/^\.coverage_data\/coveragefile/).test(name);
})
.then(function (list) {
return Q.all(list.map(function (file) {
    return FS.read(file)
    .then(function (content) {
        return JSON.parse(content);
...
```

#### <a name="apidoc.element.q-io.fs.makeDirectory"></a>[function <span class="apidocSignatureSpan">q-io.fs.</span>makeDirectory (path, mode)](#apidoc.element.q-io.fs.makeDirectory)
- description and source-code
```javascript
makeDirectory = function (path, mode) {
    path = String(path);
    var done = Q.defer();
    if (typeof mode === "string") {
        mode = parseInt(mode, 8);
    } else if (mode === void 0) {
        mode = parseInt('755', 8);
    }
    FS.mkdir(path, mode, function (error) {
        if (error) {
            if (error.code === "EISDIR") {
                error.exists = true;
                error.isDirectory = true;
                error.message = "directory already exists: " + error.message;
            }
            if (error.code === "EEXIST") {
                error.exists = true;
                error.message = "file exists at that path: " + error.message;
            }
            error.message = "Can't makeDirectory " + JSON.stringify(path) + " with mode " + mode + ": " + error.message;
            done.reject(error);
        } else {
            done.resolve();
        }
    });
    return done.promise;
}
```
- example usage
```shell
...
                    );
                }));
            });
        }
        if (targetExists) {
            return copySubTree();
        } else {
            return Q.when(self.makeDirectory(target, stat.node.mode), copySubTree);
        }
    });
} else if (stat.isSymbolicLink()) {
    // TODO copy the link and type with readPath (but what about
    // Windows junction type?)
    return self.symbolicCopy(source, target);
}
...
```

#### <a name="apidoc.element.q-io.fs.makeTree"></a>[function <span class="apidocSignatureSpan">q-io.fs.</span>makeTree (path, mode)](#apidoc.element.q-io.fs.makeTree)
- description and source-code
```javascript
makeTree = function (path, mode) {
    path = String(path);
    var self = this;
    var parts = self.split(path);
    var at = [];
    if (self.isAbsolute(path)) {
        // On Windows use the root drive (e.g. "C:"), on *nix the first
        // part is the falsey "", and so use the ROOT ("/")
        at.push(parts.shift() || self.ROOT);
    }
    return parts.reduce(function (parent, part) {
        return Q.when(parent, function () {
            at.push(part);
            var parts = self.join(at) || ".";
            var made = self.makeDirectory(parts, mode);
            return Q.when(made, null, function rejected(error) {
                // throw away errors for already made directories
                if (error.exists) {
                    return;
                } else {
                    throw error;
                }
            });
        });
    }, undefined);
}
```
- example usage
```shell
...
    }).catch(function (error) {
        throw new Error("Can't remove " + JSON.stringify(path));
    });
};

inner.makeTree = function (path) {
    return attenuate(path).then(function (path) {
        return outer.makeTree(path.outer);
    }).catch(function (error) {
        throw new Error("Can't make tree " + JSON.stringify(path));
    });
};

inner.removeTree = function (path) {
    return attenuate(path).then(function (path) {
...
```

#### <a name="apidoc.element.q-io.fs.merge"></a>[function <span class="apidocSignatureSpan">q-io.fs.</span>merge (fss)](#apidoc.element.q-io.fs.merge)
- description and source-code
```javascript
merge = function (fss) {
    var tree = {};
    var done;
    fss.forEach(function (fs) {
        done = Q.when(done, function () {
            return fs.listTree("", function (path, stat) {
                return stat.isFile();
            })
            .then(function (list) {
                return Q.all(list.map(function (path) {
                    return Q.when(fs.read(path, "rb"), function (content) {
                        tree[path] = content;
                    });
                }));
            });
        });
    })
    return Q.when(done, function () {
        return MockFs(tree);
    });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.q-io.fs.mock"></a>[function <span class="apidocSignatureSpan">q-io.fs.</span>mock (path)](#apidoc.element.q-io.fs.mock)
- description and source-code
```javascript
mock = function (path) {
    return Mock.mock(this, path);
}
```
- example usage
```shell
...

You can also instantiate a mock file system with the content of a
subtree of a real file system.  You receive a promise for the mock
filesystem.

'''javascript
var FS = require("q-io/fs");
FS.mock(__dirname)
.then(function (fs) {
    //
})
.done();
'''

## HTTP
...
```

#### <a name="apidoc.element.q-io.fs.move"></a>[function <span class="apidocSignatureSpan">q-io.fs.</span>move (source, target)](#apidoc.element.q-io.fs.move)
- description and source-code
```javascript
move = function (source, target) {
    var self = this;
    return this.rename(source, target)
    .catch(function (error) {
        if (error.crossDevice) {
            return self.copyTree(source, target)
            .then(function () {
                return self.removeTree(source);
            });
        } else {
            throw error;
        }
    });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.q-io.fs.normal"></a>[function <span class="apidocSignatureSpan">q-io.fs.</span>normal ()](#apidoc.element.q-io.fs.normal)
- description and source-code
```javascript
normal = function () {
    var root = "";
    var parents = [];
    var children = [];
    for (var i = 0, ii = arguments.length; i < ii; i++) {
        var path = String(arguments[i]);
        // empty paths have no affect
        if (path === "")
            continue;
        var parts = path.split(exports.SEPARATORS_RE());
        if (exports.isAbsolute(path)) {
            root = parts.shift() + exports.SEPARATOR;
            parents = [];
            children = [];
        }
        for (var j = 0, jj = parts.length; j < jj; j++) {
            var part = parts[j];
            if (part === "." || part === "") {
            } else if (part == "..") {
                if (children.length) {
                    children.pop();
                } else {
                    if (root) {
                    } else {
                        parents.push("..");
                    }
                }
            } else {
                children.push(part);
            }
        }
    }
    path = parents.concat(children).join(exports.SEPARATOR);
    return root + path;
}
```
- example usage
```shell
...
return exports.join(parts[0], "");
};

/**
 * @returns {String} the parent directory of the given path.
 */
exports.directory = function (path) {
path = exports.normal(path);
var absolute = exports.isAbsolute(path);
var parts = exports.split(path);
// XXX needs to be sensitive to the root for
// Windows compatibility
if (parts.length) {
    if (parts[parts.length - 1] == "..") {
        parts.push("..");
...
```

#### <a name="apidoc.element.q-io.fs.open"></a>[function <span class="apidocSignatureSpan">q-io.fs.</span>open ()](#apidoc.element.q-io.fs.open)
- description and source-code
```javascript
open = function () {
    var args = arguments;
    var ready = backOffDelay ? Q.delay(backOffDelay) : Q.resolve();
    return ready.then(function () {
        return Q.when(wrapped.apply(thisp, args), function (stream) {
            backOffDelay = Math.max(0, backOffDelay - 1);
            return stream;
        }, function (error) {
            if (error.code === "EMFILE") {
                backOffDelay = (backOffDelay + 1) * backOffFactor;
                return retry.apply(null, args);
            } else {
                throw error;
            }
        });
    });
}
```
- example usage
```shell
...
    options.flags = flags;
} else {
    options = options || {};
    options.flags = flags;
    options.charset = charset;
}
options.flags = options.flags || "r";
return Q.when(this.open(path, options), function (stream) {
    return stream.read();
}, function (error) {
    error.message = "Can't read " + path + " because " + error.message;
    error.path = path;
    error.flags = flags;
    error.charset = charset;
    throw error;
...
```

#### <a name="apidoc.element.q-io.fs.read"></a>[function <span class="apidocSignatureSpan">q-io.fs.</span>read (path, flags, charset, options)](#apidoc.element.q-io.fs.read)
- description and source-code
```javascript
read = function (path, flags, charset, options) {
    if (typeof flags === "object") {
        options = flags;
    } else if (typeof charset === "object") {
        options = charset;
        options.flags = flags;
    } else {
        options = options || {};
        options.flags = flags;
        options.charset = charset;
    }
    options.flags = options.flags || "r";
    return Q.when(this.open(path, options), function (stream) {
        return stream.read();
    }, function (error) {
        error.message = "Can't read " + path + " because " + error.message;
        error.path = path;
        error.flags = flags;
        error.charset = charset;
        throw error;
    });
}
```
- example usage
```shell
...
into memory.  It returns a promise for the whole file contents.  By
default, 'read' provides a string decoded from UTF-8.  With the bytewise
mode flag, provides a 'Buffer'.

The options argument is identical to that of 'open'.

'''javascript
return FS.read(__filename, "b")
.then(function (content) {
    // ...
})
'''

'''javascript
return FS.read(__filename, {
...
```

#### <a name="apidoc.element.q-io.fs.readLink"></a>[function <span class="apidocSignatureSpan">q-io.fs.</span>readLink (path)](#apidoc.element.q-io.fs.readLink)
- description and source-code
```javascript
readLink = function (path) {
    var result = Q.defer();
    FS.readlink(path, function (error, path) {
        if (error) {
            error.message = "Can't get link from " + JSON.stringify(path) + " by way of C readlink: " + error.message;
            result.reject(error);
        } else {
            result.resolve(path);
        }
    });
    return result.promise;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.q-io.fs.relative"></a>[function <span class="apidocSignatureSpan">q-io.fs.</span>relative (source, target)](#apidoc.element.q-io.fs.relative)
- description and source-code
```javascript
relative = function (source, target) {
    var self = this;
    return Q.when(this.isDirectory(source), function (isDirectory) {
        if (isDirectory) {
            return self.relativeFromDirectory(source, target);
        } else {
            return self.relativeFromFile(source, target);
        }
    });
}
```
- example usage
```shell
...
            return self.remove(path);
        }
    });
};

exports.symbolicCopy = function (source, target, type) {
    var self = this;
    return Q.when(self.relative(target, source), function (relative) {
        return self.symbolicLink(target, relative, type || "file");
    });
};

exports.exists = function (path) {
    return Q.when(this.stat(path), function () {
        return true;
...
```

#### <a name="apidoc.element.q-io.fs.relativeFromDirectory"></a>[function <span class="apidocSignatureSpan">q-io.fs.</span>relativeFromDirectory (source, target)](#apidoc.element.q-io.fs.relativeFromDirectory)
- description and source-code
```javascript
relativeFromDirectory = function (source, target) {
    if (!target) {
        target = source;
        source = workingDirectory();
    }
    source = this.absolute(source);
    target = this.absolute(target);
    source = source.split(this.SEPARATORS_RE());
    target = target.split(this.SEPARATORS_RE());
    if (source.length === 2 && source[1] === "")
        source.pop();
    while (
        source.length &&
        target.length &&
        target[0] == source[0]
    ) {
        source.shift();
        target.shift();
    }
    while (source.length) {
        source.shift();
        target.unshift("..");
    }
    return target.join(this.SEPARATOR);
}
```
- example usage
```shell
...
console.log("            <th>File</th>");
console.log("            <th>Percentage</th>");
console.log("            <th>Missing</th>");
console.log("        </tr>");
console.log("    </thead>");
console.log("    <tbody>");
Object.forEach(coverage.files, function (file, path) {
    path = FS.relativeFromDirectory(__dirname, path);
    if (/^spec/.test(path))
        return;
    console.log("        <tr>");
    console.log("            <td><code>" + path + "</code></td>");
    console.log("            <td>" + (file.stats.percentage * 100).toFixed(0) + "%</td>");
    console.log("            <td>" + file.stats.missing + "</td>");
    console.log("        </tr>");
...
```

#### <a name="apidoc.element.q-io.fs.relativeFromFile"></a>[function <span class="apidocSignatureSpan">q-io.fs.</span>relativeFromFile (source, target)](#apidoc.element.q-io.fs.relativeFromFile)
- description and source-code
```javascript
relativeFromFile = function (source, target) {
    var self = this;
    source = self.absolute(source);
    target = self.absolute(target);
    source = source.split(self.SEPARATORS_RE());
    target = target.split(self.SEPARATORS_RE());
    source.pop();
    while (
        source.length &&
        target.length &&
        target[0] == source[0]
    ) {
        source.shift();
        target.shift();
    }
    while (source.length) {
        source.shift();
        target.unshift("..");
    }
    return target.join(self.SEPARATOR);
}
```
- example usage
```shell
...

exports.relative = function (source, target) {
    var self = this;
    return Q.when(this.isDirectory(source), function (isDirectory) {
        if (isDirectory) {
            return self.relativeFromDirectory(source, target);
        } else {
            return self.relativeFromFile(source, target);
        }
    });
};

exports.relativeFromFile = function (source, target) {
    var self = this;
    source = self.absolute(source);
...
```

#### <a name="apidoc.element.q-io.fs.remove"></a>[function <span class="apidocSignatureSpan">q-io.fs.</span>remove (path)](#apidoc.element.q-io.fs.remove)
- description and source-code
```javascript
remove = function (path) {
    path = String(path);
    var done = Q.defer();
    FS.unlink(path, function (error) {
        if (error) {
            error.message = "Can't remove " + JSON.stringify(path) + ": " + error.message;
            done.reject(error);
        } else {
            done.resolve();
        }
    });
    return done.promise;
}
```
- example usage
```shell
...
    }, undefined);
};

exports.removeTree = function (path) {
    var self = this;
    return Q.when(self.statLink(path), function (stat) {
        if (stat.isSymbolicLink()) {
            return self.remove(path);
        } else if (stat.isDirectory()) {
            return self.list(path)
            .then(function (list) {
                // asynchronously remove every subtree
                return Q.all(list.map(function (name) {
                    return self.removeTree(self.join(path, name));
                }))
...
```

#### <a name="apidoc.element.q-io.fs.removeDirectory"></a>[function <span class="apidocSignatureSpan">q-io.fs.</span>removeDirectory (path)](#apidoc.element.q-io.fs.removeDirectory)
- description and source-code
```javascript
removeDirectory = function (path) {
    path = String(path);
    var done = Q.defer();
    FS.rmdir(path, function (error) {
        if (error) {
            error.message = "Can't removeDirectory " + JSON.stringify(path) + ": " + error.message;
            done.reject(error);
        } else {
            done.resolve();
        }
    });
    return done.promise;
}
```
- example usage
```shell
...
            return self.list(path)
            .then(function (list) {
                // asynchronously remove every subtree
                return Q.all(list.map(function (name) {
                    return self.removeTree(self.join(path, name));
                }))
                .then(function () {
                    return self.removeDirectory(path);
                });
            });
        } else {
            return self.remove(path);
        }
    });
};
...
```

#### <a name="apidoc.element.q-io.fs.removeTree"></a>[function <span class="apidocSignatureSpan">q-io.fs.</span>removeTree (path)](#apidoc.element.q-io.fs.removeTree)
- description and source-code
```javascript
removeTree = function (path) {
    var self = this;
    return Q.when(self.statLink(path), function (stat) {
        if (stat.isSymbolicLink()) {
            return self.remove(path);
        } else if (stat.isDirectory()) {
            return self.list(path)
            .then(function (list) {
                // asynchronously remove every subtree
                return Q.all(list.map(function (name) {
                    return self.removeTree(self.join(path, name));
                }))
                .then(function () {
                    return self.removeDirectory(path);
                });
            });
        } else {
            return self.remove(path);
        }
    });
}
```
- example usage
```shell
...
exports.move = function (source, target) {
    var self = this;
    return this.rename(source, target)
    .catch(function (error) {
        if (error.crossDevice) {
            return self.copyTree(source, target)
            .then(function () {
                return self.removeTree(source);
            });
        } else {
            throw error;
        }
    });
};
...
```

#### <a name="apidoc.element.q-io.fs.rename"></a>[function <span class="apidocSignatureSpan">q-io.fs.</span>rename (source, target)](#apidoc.element.q-io.fs.rename)
- description and source-code
```javascript
rename = function (source, target) {
    source = String(source);
    target = String(target);
    return Q.ninvoke(FS, "rename", source, target)
    .fail(function (error) {
        if (error.code === "EXDEV") {
            error.message = "source and target are on different devices: " + error.message;
            error.crossDevice = true;
        }
        error.message = (
            "Can't move " + JSON.stringify(source) + " to " +
            JSON.stringify(target) + " because " + error.message
        );
        throw error;
    });
}
```
- example usage
```shell
...
            return stream.close();
        });
    });
};

exports.move = function (source, target) {
    var self = this;
    return this.rename(source, target)
    .catch(function (error) {
        if (error.crossDevice) {
            return self.copyTree(source, target)
            .then(function () {
                return self.removeTree(source);
            });
        } else {
...
```

#### <a name="apidoc.element.q-io.fs.reroot"></a>[function <span class="apidocSignatureSpan">q-io.fs.</span>reroot (path)](#apidoc.element.q-io.fs.reroot)
- description and source-code
```javascript
function reroot(path) {
    var self = this;
    path = path || this.ROOT;
    return RootFs(self, path);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.q-io.fs.resolve"></a>[function <span class="apidocSignatureSpan">q-io.fs.</span>resolve ()](#apidoc.element.q-io.fs.resolve)
- description and source-code
```javascript
resolve = function () {
    var root = "";
    var parents = [];
    var children = [];
    var leaf = "";
    for (var i = 0; i < arguments.length; i++) {
        var path = String(arguments[i]);
        if (path == "")
            continue;
        var parts = path.split(exports.SEPARATORS_RE());
        if (exports.isAbsolute(path)) {
            root = parts.shift() + exports.SEPARATOR;
            parents = [];
            children = [];
        }
        leaf = parts.pop();
        if (leaf == "." || leaf == "..") {
            parts.push(leaf);
            leaf = "";
        }
        for (var j = 0; j < parts.length; j++) {
            var part = parts[j];
            if (part == "." || part == "") {
            } else if (part == "..") {
                if (children.length) {
                    children.pop();
                } else {
                    if (root) {
                    } else {
                        parents.push("..");
                    }
                }
            } else {
                children.push(part);
            }
        };
    }
    path = parents.concat(children).join(exports.SEPARATOR);
    if (path) leaf = exports.SEPARATOR + leaf;
    return root + path + leaf;
}
```
- example usage
```shell
...

BufferStream.prototype.read = function () {
var result;
result = Reader.join(this._chunks);
if (this._charset) {
    result = result.toString(this._charset);
}
return Q.resolve(result);
};

BufferStream.prototype.write = function (chunk) {
if (this._charset) {
    chunk = new Buffer(String(chunk), this._charset);
} else {
    if (!(chunk instanceof Buffer)) {
...
```

#### <a name="apidoc.element.q-io.fs.root"></a>[function <span class="apidocSignatureSpan">q-io.fs.</span>root (path)](#apidoc.element.q-io.fs.root)
- description and source-code
```javascript
root = function (path) {
    if (!exports.isAbsolute(path))
        path = require("./fs").absolute(path);
    var parts = exports.split(path);
    return exports.join(parts[0], "");
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.q-io.fs.split"></a>[function <span class="apidocSignatureSpan">q-io.fs.</span>split (path)](#apidoc.element.q-io.fs.split)
- description and source-code
```javascript
split = function (path) {
    var parts;
    try {
        parts = String(path).split(exports.SEPARATORS_RE());
    } catch (exception) {
        throw new Error("Cannot split " + (typeof path) + ", " + JSON.stringify(path));
    }
    // this special case helps isAbsolute
    // distinguish an empty path from an absolute path
    // "" -> [] NOT [""]
    if (parts.length === 1 && parts[0] === "")
        return [];
    // "a" -> ["a"]
    // "/a" -> ["", "a"]
    return parts;
}
```
- example usage
```shell
...
 * file system, indicated by an empty string on Unix, and a
 * drive letter followed by a colon on Windows.
 * @returns {Array * String}
 */
exports.split = function (path) {
var parts;
try {
    parts = String(path).split(exports.SEPARATORS_RE());
} catch (exception) {
    throw new Error("Cannot split " + (typeof path) + ", " + JSON.stringify(path));
}
// this special case helps isAbsolute
// distinguish an empty path from an absolute path
// "" -> [] NOT [""]
if (parts.length === 1 && parts[0] === "")
...
```

#### <a name="apidoc.element.q-io.fs.stat"></a>[function <span class="apidocSignatureSpan">q-io.fs.</span>stat (path)](#apidoc.element.q-io.fs.stat)
- description and source-code
```javascript
stat = function (path) {
    var self = this;
    path = String(path);
    var done = Q.defer();
    try {
        FS.stat(path, function (error, stat) {
            if (error) {
                error.message = "Can't stat " + JSON.stringify(path) + ": " + error;
                done.reject(error);
            } else {
                done.resolve(new self.Stats(stat));
            }
        });
    } catch (error) {
        done.reject(error);
    }
    return done.promise;
}
```
- example usage
```shell
...
            throw error;
        }
    });
};

exports.copy = function (source, target) {
    var self = this;
    return Q.when(self.stat(source), function (stat) {
        var mode = stat.node.mode;
        return Q.all([
            self.open(source, {flags: "rb"}),
            self.open(target, {flags: "wb", mode: mode})
        ]);
    })
    .spread(function (reader, writer) {
...
```

#### <a name="apidoc.element.q-io.fs.statFd"></a>[function <span class="apidocSignatureSpan">q-io.fs.</span>statFd (fd)](#apidoc.element.q-io.fs.statFd)
- description and source-code
```javascript
statFd = function (fd) {
    fd = Number(fd);
    var done = Q.defer();
    try {
        FS.fstat(fd, function (error, stat) {
            if (error) {
                error.message = "Can't statFd file descriptor " + JSON.stringify(fd) + ": " + error.message;
                done.reject(error);
            } else {
                done.resolve(stat);
            }
        });
    } catch (error) {
        done.reject(error);
    }
    return done.promise;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.q-io.fs.statLink"></a>[function <span class="apidocSignatureSpan">q-io.fs.</span>statLink (path)](#apidoc.element.q-io.fs.statLink)
- description and source-code
```javascript
statLink = function (path) {
    path = String(path);
    var done = Q.defer();
    try {
        FS.lstat(path, function (error, stat) {
            if (error) {
                error.message = "Can't statLink " + JSON.stringify(path) + ": " + error.message;
                done.reject(error);
            } else {
                done.resolve(stat);
            }
        });
    } catch (error) {
        done.reject(error);
    }
    return done.promise;
}
```
- example usage
```shell
...
            });
        });
    }, undefined);
};

exports.removeTree = function (path) {
    var self = this;
    return Q.when(self.statLink(path), function (stat) {
        if (stat.isSymbolicLink()) {
            return self.remove(path);
        } else if (stat.isDirectory()) {
            return self.list(path)
            .then(function (list) {
                // asynchronously remove every subtree
                return Q.all(list.map(function (name) {
...
```

#### <a name="apidoc.element.q-io.fs.symbolicCopy"></a>[function <span class="apidocSignatureSpan">q-io.fs.</span>symbolicCopy (source, target, type)](#apidoc.element.q-io.fs.symbolicCopy)
- description and source-code
```javascript
symbolicCopy = function (source, target, type) {
    var self = this;
    return Q.when(self.relative(target, source), function (relative) {
        return self.symbolicLink(target, relative, type || "file");
    });
}
```
- example usage
```shell
...
                } else {
                    return Q.when(self.makeDirectory(target, stat.node.mode), copySubTree);
                }
            });
        } else if (stat.isSymbolicLink()) {
            // TODO copy the link and type with readPath (but what about
            // Windows junction type?)
            return self.symbolicCopy(source, target);
        }
    });
};

exports.listTree = function (basePath, guard) {
    var self = this;
    basePath = String(basePath || '');
...
```

#### <a name="apidoc.element.q-io.fs.symbolicLink"></a>[function <span class="apidocSignatureSpan">q-io.fs.</span>symbolicLink (target, relative, type)](#apidoc.element.q-io.fs.symbolicLink)
- description and source-code
```javascript
symbolicLink = function (target, relative, type) {
    if (!linkTypes.hasOwnProperty(type)) {
        console.warn(new Error("For Windows compatibility, symbolicLink must be called with a type argument \"file\", \"directory\", or \"junction\""));
    }
    type = linkTypes[type];
    target = String(target);
    relative = String(relative);
    var done = Q.defer();
    try {
        FS.symlink(relative, target, type || 'file', function (error) {
            if (error) {
                error.message = "Can't create symbolicLink " + JSON.stringify(target) + " to relative location " + JSON.stringify
(relative) + ": " + error.message;
                done.reject(error);
            } else {
                done.resolve();
            }
        });
    } catch (error) {
        done.reject(error);
    }
    return done.promise;
}
```
- example usage
```shell
...
        }
    });
};

exports.symbolicCopy = function (source, target, type) {
    var self = this;
    return Q.when(self.relative(target, source), function (relative) {
        return self.symbolicLink(target, relative, type || "file");
    });
};

exports.exists = function (path) {
    return Q.when(this.stat(path), function () {
        return true;
    }, function () {
...
```

#### <a name="apidoc.element.q-io.fs.toObject"></a>[function <span class="apidocSignatureSpan">q-io.fs.</span>toObject (path)](#apidoc.element.q-io.fs.toObject)
- description and source-code
```javascript
toObject = function (path) {
    var self = this;
    var list = self.listTree(path || "", function (path, stat) {
        return stat.isFile();
    });
    return Q.when(list, function (list) {
        var tree = {};
        return Q.all(list.map(function (path) {
            return Q.when(self.read(path, "rb"), function (content) {
                tree[path] = content;
            });
        })).then(function () {
            return tree;
        });
    });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.q-io.fs.write"></a>[function <span class="apidocSignatureSpan">q-io.fs.</span>write (path, content, flags, charset, options)](#apidoc.element.q-io.fs.write)
- description and source-code
```javascript
write = function (path, content, flags, charset, options) {
    var self = this;
    if (typeof flags === "object") {
        options = flags;
    } else if (typeof charset === "object") {
        options = charset;
        options.flags = flags;
    } else {
        options = options || {};
        options.flags = flags;
        options.charset = charset;
    }
    flags = options.flags || "w";
    if (flags.indexOf("b") !== -1) {
        if (!(content instanceof Buffer)) {
            content = new Buffer(content);
        }
    } else if (content instanceof Buffer) {
        flags += "b";
    }
    options.flags = flags;
    return Q.when(self.open(path, options), function (stream) {
        return Q.when(stream.write(content), function () {
            return stream.close();
        });
    });
}
```
- example usage
```shell
...
'write' is a shortcut for opening a file and writing its entire content
from a single string or buffer.

The options are identical to that of 'open', but the "w" flag is
implied, and the "b" flag is implied if the content is a buffer.

'''javascript
return FS.write("hello.txt", "Hello, World!\n")
.then(function () {
    return FS.read("hello.txt")
})
.then(function (hello) {
    expect(hello).toBe("Hello, World!\n")
})
'''
...
```



# <a name="apidoc.module.q-io.fs2http"></a>[module q-io.fs2http](#apidoc.module.q-io.fs2http)

#### <a name="apidoc.element.q-io.fs2http.Client"></a>[function <span class="apidocSignatureSpan">q-io.fs2http.</span>Client (fs)](#apidoc.element.q-io.fs2http.Client)
- description and source-code
```javascript
function Client(fs) {
    var self = Object.create(Client.prototype);

    self.request = function (request) {
        return Q.when(request, function (request) {
            request = HTTP.normalizeRequest(request);
            var url = URL.parse(request.url);
            if (url.protocol !== "file:") {
                return {
                    status: 404,
                    headers: {},
                    body: ["Can't access protocol " + url.protocol]
                };
            } else {
                var path = url.pathname;
                return fs.open(path, {
                    charset: request.charset
                }).then(function (body) {
                    return {
                        status: 200,
                        headers: {},
                        body: body
                    };
                });
            }
        });
    };

    self.read = function (request, qualifier) {
        qualifier = qualifier || function (response) {
            return response.status === 200;
        };
        return Q.when(exports.request(request), function (response) {
            if (!qualifier(response)){
                var error = new Error("HTTP request failed with code " + response.status);
                error.response = response;
                throw error;
            }
            return Q.invoke(response.body, "read");
        });
    };

    return self;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.q-io.fs2http.read"></a>[function <span class="apidocSignatureSpan">q-io.fs2http.</span>read (request, qualifier)](#apidoc.element.q-io.fs2http.read)
- description and source-code
```javascript
read = function (request, qualifier) {
    return Q.fcall(require.async || require, "./fs")
    .then(function (fs) {
        return Client(fs).read(request);
    });
}
```
- example usage
```shell
...
into memory.  It returns a promise for the whole file contents.  By
default, 'read' provides a string decoded from UTF-8.  With the bytewise
mode flag, provides a 'Buffer'.

The options argument is identical to that of 'open'.

'''javascript
return FS.read(__filename, "b")
.then(function (content) {
    // ...
})
'''

'''javascript
return FS.read(__filename, {
...
```

#### <a name="apidoc.element.q-io.fs2http.request"></a>[function <span class="apidocSignatureSpan">q-io.fs2http.</span>request (request)](#apidoc.element.q-io.fs2http.request)
- description and source-code
```javascript
request = function (request) {
    return Q.fcall(require.async || require, "./fs")
    .then(function (fs) {
        return Client(fs).request(request);
    });
}
```
- example usage
```shell
...
    });
};

self.read = function (request, qualifier) {
    qualifier = qualifier || function (response) {
        return response.status === 200;
    };
    return Q.when(exports.request(request), function (response) {
        if (!qualifier(response)){
            var error = new Error("HTTP request failed with code " + response.status);
            error.response = response;
            throw error;
        }
        return Q.invoke(response.body, "read");
    });
...
```



# <a name="apidoc.module.q-io.fs_boot"></a>[module q-io.fs_boot](#apidoc.module.q-io.fs_boot)

#### <a name="apidoc.element.q-io.fs_boot.SEPARATORS_RE"></a>[function <span class="apidocSignatureSpan">q-io.fs_boot.</span>SEPARATORS_RE ()](#apidoc.element.q-io.fs_boot.SEPARATORS_RE)
- description and source-code
```javascript
SEPARATORS_RE = function () {
    if (
        separatorCached !== exports.SEPARATOR ||
        altSeparatorCached !== exports.ALT_SEPARATOR
    ) {
        separatorCached = exports.SEPARATOR;
        altSeparatorCached = exports.ALT_SEPARATOR;
        separatorReCached = new RegExp("[" +
            (separatorCached || "").replace(/[-[\]{}()*+?.\\^$|,#\s]/g, "\\$&") +
            (altSeparatorCached || "").replace(/[-[\]{}()*+?.\\^$|,#\s]/g, "\\$&") +
        "]", "g");
    }
    return separatorReCached;
}
```
- example usage
```shell
...
 * file system, indicated by an empty string on Unix, and a
 * drive letter followed by a colon on Windows.
 * @returns {Array * String}
 */
exports.split = function (path) {
var parts;
try {
    parts = String(path).split(exports.SEPARATORS_RE());
} catch (exception) {
    throw new Error("Cannot split " + (typeof path) + ", " + JSON.stringify(path));
}
// this special case helps isAbsolute
// distinguish an empty path from an absolute path
// "" -> [] NOT [""]
if (parts.length === 1 && parts[0] === "")
...
```

#### <a name="apidoc.element.q-io.fs_boot.base"></a>[function <span class="apidocSignatureSpan">q-io.fs_boot.</span>base (path, extension)](#apidoc.element.q-io.fs_boot.base)
- description and source-code
```javascript
base = function (path, extension) {
    var base = path.split(exports.SEPARATORS_RE()).pop();
    if (extension)
        base = base.replace(
            new RegExp(regExpEscape(extension) + "$"),
            ""
        );
    return base;
}
```
- example usage
```shell
...
};

/**
 * @returns {String} the extension (e.g., 'txt') of the file
 * at the given path.
 */
exports.extension = function (path) {
    path = exports.base(path);
    path = path.replace(/^\.*/, "");
    var index = path.lastIndexOf(".");
    return index <= 0 ? "" : path.substring(index);
};

})(typeof exports !== "undefined" ? exports : FS_BOOT = {});
...
```

#### <a name="apidoc.element.q-io.fs_boot.directory"></a>[function <span class="apidocSignatureSpan">q-io.fs_boot.</span>directory (path)](#apidoc.element.q-io.fs_boot.directory)
- description and source-code
```javascript
directory = function (path) {
    path = exports.normal(path);
    var absolute = exports.isAbsolute(path);
    var parts = exports.split(path);
    // XXX needs to be sensitive to the root for
    // Windows compatibility
    if (parts.length) {
        if (parts[parts.length - 1] == "..") {
            parts.push("..");
        } else {
            parts.pop();
        }
    } else {
        parts.unshift("..");
    }
    return parts.join(exports.SEPARATOR) || (
        exports.isRelative(path) ?
        "" : exports.ROOT
    );
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.q-io.fs_boot.extension"></a>[function <span class="apidocSignatureSpan">q-io.fs_boot.</span>extension (path)](#apidoc.element.q-io.fs_boot.extension)
- description and source-code
```javascript
extension = function (path) {
    path = exports.base(path);
    path = path.replace(/^\.*/, "");
    var index = path.lastIndexOf(".");
    return index <= 0 ? "" : path.substring(index);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.q-io.fs_boot.isAbsolute"></a>[function <span class="apidocSignatureSpan">q-io.fs_boot.</span>isAbsolute (path)](#apidoc.element.q-io.fs_boot.isAbsolute)
- description and source-code
```javascript
isAbsolute = function (path) {
    // for absolute paths on any operating system,
    // the first path component always determines
    // whether it is relative or absolute.  On Unix,
    // it is empty, so ["", "foo"].join("/") == "/foo",
    // "/foo".split("/") == ["", "foo"].
    var parts = exports.split(path);
    // split("") == [].  "" is not absolute.
    // split("/") == ["", ""] is absolute.
    // split(?) == [""] does not occur.
    if (parts.length == 0)
        return false;
    return exports.isRoot(parts[0]);
}
```
- example usage
```shell
...
var children = [];
var leaf = "";
for (var i = 0; i < arguments.length; i++) {
    var path = String(arguments[i]);
    if (path == "")
        continue;
    var parts = path.split(exports.SEPARATORS_RE());
    if (exports.isAbsolute(path)) {
        root = parts.shift() + exports.SEPARATOR;
        parents = [];
        children = [];
    }
    leaf = parts.pop();
    if (leaf == "." || leaf == "..") {
        parts.push(leaf);
...
```

#### <a name="apidoc.element.q-io.fs_boot.isRelative"></a>[function <span class="apidocSignatureSpan">q-io.fs_boot.</span>isRelative (path)](#apidoc.element.q-io.fs_boot.isRelative)
- description and source-code
```javascript
isRelative = function (path) {
    return !exports.isAbsolute(path);
}
```
- example usage
```shell
...
       } else {
           parts.pop();
       }
   } else {
       parts.unshift("..");
   }
   return parts.join(exports.SEPARATOR) || (
       exports.isRelative(path) ?
       "" : exports.ROOT
   );
};

/**
* @returns {String} the last component of a path, without
* the given extension if the extension is provided and
...
```

#### <a name="apidoc.element.q-io.fs_boot.isRoot"></a>[function <span class="apidocSignatureSpan">q-io.fs_boot.</span>isRoot (first)](#apidoc.element.q-io.fs_boot.isRoot)
- description and source-code
```javascript
isRoot = function (first) {
    if (exports.SEPARATOR === "\\") {
        return /[a-zA-Z]:$/.test(first);
    } else {
        return first == "";
    }
}
```
- example usage
```shell
...
    // "/foo".split("/") == ["", "foo"].
    var parts = exports.split(path);
    // split("") == [].  "" is not absolute.
    // split("/") == ["", ""] is absolute.
    // split(?) == [""] does not occur.
    if (parts.length == 0)
        return false;
    return exports.isRoot(parts[0]);
};

/**
 * @returns {Boolean} whether the given path does not begin
 * at the root of the file system or a drive letter.
 */
exports.isRelative = function (path) {
...
```

#### <a name="apidoc.element.q-io.fs_boot.join"></a>[function <span class="apidocSignatureSpan">q-io.fs_boot.</span>join ()](#apidoc.element.q-io.fs_boot.join)
- description and source-code
```javascript
join = function () {
    if (arguments.length === 1 && Array.isArray(arguments[0]))
        return exports.normal.apply(exports, arguments[0]);
    return exports.normal.apply(exports, arguments);
}
```
- example usage
```shell
...
    return Q.fcall(function () {
        chunks.splice(0, chunks.length).forEach(write, thisp);
    });
};

BufferStream.prototype.read = function () {
    var result;
    result = Reader.join(this._chunks);
    if (this._charset) {
        result = result.toString(this._charset);
    }
    return Q.resolve(result);
};

BufferStream.prototype.write = function (chunk) {
...
```

#### <a name="apidoc.element.q-io.fs_boot.normal"></a>[function <span class="apidocSignatureSpan">q-io.fs_boot.</span>normal ()](#apidoc.element.q-io.fs_boot.normal)
- description and source-code
```javascript
normal = function () {
    var root = "";
    var parents = [];
    var children = [];
    for (var i = 0, ii = arguments.length; i < ii; i++) {
        var path = String(arguments[i]);
        // empty paths have no affect
        if (path === "")
            continue;
        var parts = path.split(exports.SEPARATORS_RE());
        if (exports.isAbsolute(path)) {
            root = parts.shift() + exports.SEPARATOR;
            parents = [];
            children = [];
        }
        for (var j = 0, jj = parts.length; j < jj; j++) {
            var part = parts[j];
            if (part === "." || part === "") {
            } else if (part == "..") {
                if (children.length) {
                    children.pop();
                } else {
                    if (root) {
                    } else {
                        parents.push("..");
                    }
                }
            } else {
                children.push(part);
            }
        }
    }
    path = parents.concat(children).join(exports.SEPARATOR);
    return root + path;
}
```
- example usage
```shell
...
return exports.join(parts[0], "");
};

/**
 * @returns {String} the parent directory of the given path.
 */
exports.directory = function (path) {
path = exports.normal(path);
var absolute = exports.isAbsolute(path);
var parts = exports.split(path);
// XXX needs to be sensitive to the root for
// Windows compatibility
if (parts.length) {
    if (parts[parts.length - 1] == "..") {
        parts.push("..");
...
```

#### <a name="apidoc.element.q-io.fs_boot.resolve"></a>[function <span class="apidocSignatureSpan">q-io.fs_boot.</span>resolve ()](#apidoc.element.q-io.fs_boot.resolve)
- description and source-code
```javascript
resolve = function () {
    var root = "";
    var parents = [];
    var children = [];
    var leaf = "";
    for (var i = 0; i < arguments.length; i++) {
        var path = String(arguments[i]);
        if (path == "")
            continue;
        var parts = path.split(exports.SEPARATORS_RE());
        if (exports.isAbsolute(path)) {
            root = parts.shift() + exports.SEPARATOR;
            parents = [];
            children = [];
        }
        leaf = parts.pop();
        if (leaf == "." || leaf == "..") {
            parts.push(leaf);
            leaf = "";
        }
        for (var j = 0; j < parts.length; j++) {
            var part = parts[j];
            if (part == "." || part == "") {
            } else if (part == "..") {
                if (children.length) {
                    children.pop();
                } else {
                    if (root) {
                    } else {
                        parents.push("..");
                    }
                }
            } else {
                children.push(part);
            }
        };
    }
    path = parents.concat(children).join(exports.SEPARATOR);
    if (path) leaf = exports.SEPARATOR + leaf;
    return root + path + leaf;
}
```
- example usage
```shell
...

BufferStream.prototype.read = function () {
var result;
result = Reader.join(this._chunks);
if (this._charset) {
    result = result.toString(this._charset);
}
return Q.resolve(result);
};

BufferStream.prototype.write = function (chunk) {
if (this._charset) {
    chunk = new Buffer(String(chunk), this._charset);
} else {
    if (!(chunk instanceof Buffer)) {
...
```

#### <a name="apidoc.element.q-io.fs_boot.root"></a>[function <span class="apidocSignatureSpan">q-io.fs_boot.</span>root (path)](#apidoc.element.q-io.fs_boot.root)
- description and source-code
```javascript
root = function (path) {
    if (!exports.isAbsolute(path))
        path = require("./fs").absolute(path);
    var parts = exports.split(path);
    return exports.join(parts[0], "");
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.q-io.fs_boot.split"></a>[function <span class="apidocSignatureSpan">q-io.fs_boot.</span>split (path)](#apidoc.element.q-io.fs_boot.split)
- description and source-code
```javascript
split = function (path) {
    var parts;
    try {
        parts = String(path).split(exports.SEPARATORS_RE());
    } catch (exception) {
        throw new Error("Cannot split " + (typeof path) + ", " + JSON.stringify(path));
    }
    // this special case helps isAbsolute
    // distinguish an empty path from an absolute path
    // "" -> [] NOT [""]
    if (parts.length === 1 && parts[0] === "")
        return [];
    // "a" -> ["a"]
    // "/a" -> ["", "a"]
    return parts;
}
```
- example usage
```shell
...
 * file system, indicated by an empty string on Unix, and a
 * drive letter followed by a colon on Windows.
 * @returns {Array * String}
 */
exports.split = function (path) {
var parts;
try {
    parts = String(path).split(exports.SEPARATORS_RE());
} catch (exception) {
    throw new Error("Cannot split " + (typeof path) + ", " + JSON.stringify(path));
}
// this special case helps isAbsolute
// distinguish an empty path from an absolute path
// "" -> [] NOT [""]
if (parts.length === 1 && parts[0] === "")
...
```



# <a name="apidoc.module.q-io.fs_common"></a>[module q-io.fs_common](#apidoc.module.q-io.fs_common)

#### <a name="apidoc.element.q-io.fs_common.update"></a>[function <span class="apidocSignatureSpan">q-io.fs_common.</span>update (exports, workingDirectory)](#apidoc.element.q-io.fs_common.update)
- description and source-code
```javascript
update = function (exports, workingDirectory) {

    for (var name in Boot) {
        exports[name] = Boot[name];
    }

<span class="apidocCodeCommentSpan">    /**
     * Read a complete file.
     * @param {String} path    Path to the file.
     * @param {String} [options.flags]  The mode to open the file with.
     * @param {String} [options.charset]  The charset to open the file with.
     * @param {Object} [options]   An object with options.
     * second argument.
     * @returns {Promise * (String || Buffer)}
     */
</span>    exports.read = function (path, flags, charset, options) {
        if (typeof flags === "object") {
            options = flags;
        } else if (typeof charset === "object") {
            options = charset;
            options.flags = flags;
        } else {
            options = options || {};
            options.flags = flags;
            options.charset = charset;
        }
        options.flags = options.flags || "r";
        return Q.when(this.open(path, options), function (stream) {
            return stream.read();
        }, function (error) {
            error.message = "Can't read " + path + " because " + error.message;
            error.path = path;
            error.flags = flags;
            error.charset = charset;
            throw error;
        });
    };

    /**
     * Write content to a file, overwriting the existing content.
     * @param {String} path    Path to the file.
     * @param {String || Buffer} content
     * @param {String} [options.flags]  The mode to open the file with.
     * @param {String} [options.charset]  The charset to open the file with.
     * @param {Object} [options]   An object with options.
     * @returns {Promise * Undefined} a promise that resolves
     * when the writing is complete.
     */
    exports.write = function (path, content, flags, charset, options) {
        var self = this;
        if (typeof flags === "object") {
            options = flags;
        } else if (typeof charset === "object") {
            options = charset;
            options.flags = flags;
        } else {
            options = options || {};
            options.flags = flags;
            options.charset = charset;
        }
        flags = options.flags || "w";
        if (flags.indexOf("b") !== -1) {
            if (!(content instanceof Buffer)) {
                content = new Buffer(content);
            }
        } else if (content instanceof Buffer) {
            flags += "b";
        }
        options.flags = flags;
        return Q.when(self.open(path, options), function (stream) {
            return Q.when(stream.write(content), function () {
                return stream.close();
            });
        });
    };

    /**
     * Append content to the end of a file.
     * @param {String} path    Path to the file.
     * @param {String || Buffer} content
     * @param {String} [options.flags]  The mode to open the file with.
     * @param {String} [options.charset]  The charset to open the file with.
     * @param {Object} [options]   An object with options.
     * @returns {Promise * Undefined} a promise that resolves
     * when the writing is complete.
     */
    exports.append = function (path, content, flags, charset, options) {
        var self = this;
        if (typeof flags === "object") {
            options = flags;
        } else if (typeof charset === "object") {
            options = charset;
            options.flags = flags;
        } else {
            options = options || {};
            options.flags = flags;
            options.charset = charset;
        }
        flags = options.flags || "a";
        if (content instanceof Buffer) {
            flags += "b";
        }
        options.flags = flags;
        return Q.when(self.open(path, options), function (stream) {
            return Q.when(stream.write(content), function () {
                return stream.close();
            });
        });
    };

    exports.move = function (source, target) {
        var self = this;
        return this.rename(source, target)
        .catch(function (error) {
            if (error.crossDevic ...
```
- example usage
```shell
...
    });
}

function workingDirectory() {
    return outer.ROOT;
}

COMMON.update(inner, workingDirectory);

inner.list = function (path) {
    return attenuate(path).then(function (path) {
        return outer.list(path.outer);
    }).then(null, function (reason) {
        return Q.reject("Can't list " + JSON.stringify(path));
    });
...
```



# <a name="apidoc.module.q-io.html"></a>[module q-io.html](#apidoc.module.q-io.html)

#### <a name="apidoc.element.q-io.html.HandleHtmlFragmentResponses"></a>[function <span class="apidocSignatureSpan">q-io.html.</span>HandleHtmlFragmentResponses (app, handleHtmlFragmentResponse)](#apidoc.element.q-io.html.HandleHtmlFragmentResponses)
- description and source-code
```javascript
HandleHtmlFragmentResponses = function (app, handleHtmlFragmentResponse) {
    handleHtmlFragmentResponse = handleHtmlFragmentResponse || exports.handleHtmlFragmentResponse;
    return function (request) {
        request.handleHtmlFragmentResponse = handleHtmlFragmentResponse;
        return Q.fcall(app, request)
        .then(function (response) {
            if (response.htmlFragment) {
                return Q.fcall(handleHtmlFragmentResponse, response);
            } else {
                return response;
            }
        });
    };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.q-io.html.escapeHtml"></a>[function <span class="apidocSignatureSpan">q-io.html.</span>escapeHtml (text)](#apidoc.element.q-io.html.escapeHtml)
- description and source-code
```javascript
function escapeHtml(text) {
    return String(text)
        .replace(/&/g, "&amp;")
        .replace(/</g, "&lt;")
        .replace(/>/g, "&gt;")
        .replace(/"/g, "&quot;")
}
```
- example usage
```shell
...
headers: {
    location: location,
    "content-type": "text/html"
},
htmlTitle: title,
htmlFragment: {
    forEach: function (write) {
        write("<h1>" + HtmlApps.escapeHtml(title) + "</h1>\n");
        write(
            "<p>See: <a href=\"" + HtmlApps.escapeHtml(location) + "\">" +
            HtmlApps.escapeHtml(location) +
            "</a></p>\n"
        );
    }
}
...
```

#### <a name="apidoc.element.q-io.html.handleHtmlFragmentResponse"></a>[function <span class="apidocSignatureSpan">q-io.html.</span>handleHtmlFragmentResponse (response)](#apidoc.element.q-io.html.handleHtmlFragmentResponse)
- description and source-code
```javascript
handleHtmlFragmentResponse = function (response) {
    var htmlFragment = response.htmlFragment;
    delete response.htmlFragment;
    response.headers["content-type"] = "text/html; charset=utf-8";
    response.body = {
        forEach: function (write) {
            write("<!doctype html>\n");
            write("<html>\n");
            write("    <head>\n");
            if (response.htmlTitle !== void 0) {
                write("        <title>" + escapeHtml(response.htmlTitle) + "</title>\n");
            }
            write("    </head>\n");
            write("    <body>\n");
            htmlFragment.forEach(function (line) {
                write("        " + line);
            });
            write("    </body>\n");
            write("</html>\n");
        }
    };
    return response;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.q-io.http"></a>[module q-io.http](#apidoc.module.q-io.http)

#### <a name="apidoc.element.q-io.http.ClientResponse"></a>[function <span class="apidocSignatureSpan">q-io.http.</span>ClientResponse (_response, charset)](#apidoc.element.q-io.http.ClientResponse)
- description and source-code
```javascript
ClientResponse = function (_response, charset) {
    var response = Object.create(exports.ClientResponse.prototype);
<span class="apidocCodeCommentSpan">    /*** {Number} HTTP status code */
</span>    response.status = _response.statusCode;
    /*** HTTP version */
    response.version = _response.httpVersion;
    /*** {Object} HTTP headers */
    response.headers = _response.headers;
    /***
     * A Q IO asynchronous text reader.
     */
    response.node = _response;
    response.nodeResponse = _response; // Deprecated
    response.nodeConnection = _response.connection; // Deprecated
    return Q.when(Reader(_response, charset), function (body) {
        response.body = body;
        return response;
    });
}
```
- example usage
```shell
...
};

if (request.agent !== undefined) {
    requestOptions.agent = request.agent;
}

var _request = http.request(requestOptions, function (_response) {
    deferred.resolve(exports.ClientResponse(_response, request.charset));
    _response.on("error", function (error) {
        // TODO find a better way to channel
        // this into the response
        console.warn(error && error.stack || error);
        deferred.reject(error);
    });
});
...
```

#### <a name="apidoc.element.q-io.http.Server"></a>[function <span class="apidocSignatureSpan">q-io.http.</span>Server (respond)](#apidoc.element.q-io.http.Server)
- description and source-code
```javascript
Server = function (respond) {
    var self = Object.create(exports.Server.prototype);

    var server = HTTP.createServer(function (_request, _response) {
        var request = exports.ServerRequest(_request);
        var response = exports.ServerResponse(_response);

        var closed = Q.defer();
        _request.on("end", function (error, value) {
            if (error) {
                closed.reject(error);
            } else {
                closed.resolve(value);
            }
        });

        Q.when(request, function (request) {
            return Q.when(respond(request, response), function (response) {
                if (!response)
                    return;

                _response.writeHead(response.status, response.headers);

                if (response.onclose || response.onClose)
                    Q.when(closed, response.onclose || response.onClose);

                return Q.when(response.body, function (body) {
                    var length;
                    if (
                        Array.isArray(body) &&
                        (length = body.length) &&
                        body.every(function (chunk) {
                            return typeof chunk === "string"
                        })
                    ) {
                        body.forEach(function (chunk, i) {
                            if (i < length - 1) {
                                _response.write(chunk, response.charset);
                            } else {
                                _response.end(chunk, response.charset);
                            }
                        });
                    } else if (body) {
                        var end;
                        var done = body.forEach(function (chunk) {
                            end = Q.when(end, function () {
                                return Q.when(chunk, function (chunk) {
                                    _response.write(chunk, response.charset);
                                });
                            });
                        });
                        return Q.when(done, function () {
                            return Q.when(end, function () {
                                _response.end();
                            });
                        });
                    } else {
                        _response.end();
                    }
                });

            })
        })
        .done(); // should be .fail(self.emitter("error"))

    });

    var stopped = Q.defer();
    server.on("close", function (err) {
        if (err) {
            stopped.reject(err);
        } else {
            stopped.resolve();
        }
    });

<span class="apidocCodeCommentSpan">    /***
     * Stops the server.
     * @returns {Promise * Undefined} a promise that will
     * resolve when the server is stopped.
     */
</span>    self.stop = function () {
        server.close();
        listening = undefined;
        return stopped.promise;
    };

    var listening = Q.defer();
    server.on("listening", function (err) {
        if (err) {
            listening.reject(err);
        } else {
            listening.resolve(self);
        }
    });

    /***
     * Starts the server, listening on the given port
     * @param {Number} port
     * @returns {Promise * Undefined} a promise that will
     * resolve when the server is ready to receive
     * connections
     */
    self.listen = function (/*...args*/) {
        if (typeof server.port !== "undefined")
            return Q.reject(new Error("A server cannot be restarted or " +
            "started on a new port"));
        server.listen.apply(server, arguments);
        return listening.promise;
    };

    self.stopped = stopped.promise;

    self.node = server;
    self.nodeServer = server; // Deprecated
    self.address = server.address.bind(server);

    return self;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.q-io.http.ServerRequest"></a>[function <span class="apidocSignatureSpan">q-io.http.</span>ServerRequest (_request, ssl)](#apidoc.element.q-io.http.ServerRequest)
- description and source-code
```javascript
ServerRequest = function (_request, ssl) {
    var request = Object.create(_request, requestDescriptor);
<span class="apidocCodeCommentSpan">    /*** {Array} HTTP version. (JSGI) */
</span>    request.version = _request.httpVersion.split(".").map(Math.floor);
    /*** {String} HTTP method, e.g., '"GET"' (JSGI) */
    request.method = _request.method;
    /*** {String} path, starting with '"/"' */
    request.path = _request.url;
    /*** {String} pathInfo, starting with '"/"', the
     * portion of the path that has not yet
     * been routed (JSGI) */
    request._pathInfo = null;
    /*** {String} scriptName, the portion of the path that
     * has already been routed (JSGI) */
    request.scriptName = "";
    /*** {String} (JSGI) */
    request.scheme = "http";

    var address = _request.connection.address();
    /*** {String} hostname */
    if (_request.headers.host) {
        request.hostname = _request.headers.host.split(":")[0];
    } else {
        request.hostname = address.address;
    }
    /*** {String} host */
    request.port = address.port;
    var defaultPort = request.port === (ssl ? 443 : 80);
    request.host = request.hostname + (defaultPort ? "" : ":" + request.port);

    var socket = _request.socket;
    /*** {String} */
    request.remoteHost = socket.remoteAddress;
    /*** {Number} */
    request.remotePort = socket.remotePort;

    /*** {String} url */
    request.url = URL.format({
        protocol: request.scheme,
        host: _request.headers.host,
        port: request.port === (ssl ? 443 : 80) ? null : request.port,
        path: request.path
    });
    /*** A Q IO asynchronous text reader */
    request.body = Reader(_request);
    /*** {Object} HTTP headers (JSGI)*/
    request.headers = _request.headers;
    /*** The underlying Node request */
    request.node = _request;
    request.nodeRequest = _request; // Deprecated
    /*** The underlying Node TCP connection */
    request.nodeConnection = _request.connection;

    return Q.when(request.body, function (body) {
        request.body = body;
        return request;
    });
}
```
- example usage
```shell
...
 * written.
 * @returns a Node Server object.
 */
exports.Server = function (respond) {
    var self = Object.create(exports.Server.prototype);

    var server = HTTP.createServer(function (_request, _response) {
var request = exports.ServerRequest(_request);
var response = exports.ServerResponse(_response);

var closed = Q.defer();
_request.on("end", function (error, value) {
    if (error) {
        closed.reject(error);
    } else {
...
```

#### <a name="apidoc.element.q-io.http.ServerResponse"></a>[function <span class="apidocSignatureSpan">q-io.http.</span>ServerResponse (_response, ssl)](#apidoc.element.q-io.http.ServerResponse)
- description and source-code
```javascript
ServerResponse = function (_response, ssl) {
    var response = Object.create(_response);
    response.ssl = ssl;
    response.node = _response;
    response.nodeResponse = _response; // Deprecated
    return response;
}
```
- example usage
```shell
...
 * @returns a Node Server object.
 */
exports.Server = function (respond) {
    var self = Object.create(exports.Server.prototype);

    var server = HTTP.createServer(function (_request, _response) {
var request = exports.ServerRequest(_request);
var response = exports.ServerResponse(_response);

var closed = Q.defer();
_request.on("end", function (error, value) {
    if (error) {
        closed.reject(error);
    } else {
        closed.resolve(value);
...
```

#### <a name="apidoc.element.q-io.http.normalizeRequest"></a>[function <span class="apidocSignatureSpan">q-io.http.</span>normalizeRequest (request)](#apidoc.element.q-io.http.normalizeRequest)
- description and source-code
```javascript
normalizeRequest = function (request) {
    if (typeof request === "string") {
        request = {url: request};
    }
    request.method = request.method || "GET";
    request.headers = request.headers || {};
    if (request.url) {
        var url = URL.parse(request.url);
        request.ssl = url.protocol === "https:";
        request.hostname = url.hostname;
        request.host = url.host;
        request.port = +url.port;
        request.path = (url.pathname || "") + (url.search || "");
        request.auth = url.auth || void 0;
    }
    request.host = request.host || request.headers.host;
    request.port = request.port || (request.ssl ? 443 : 80);
    if (request.host && !request.hostname) {
        request.hostname = request.host.split(":")[0];
    }
    if (request.hostname && request.port && !request.host) {
        var defaultPort = request.ssl ? 443 : 80;
        request.host = request.hostname + (defaultPort ? "" : ":" + request.port);
    }
    request.headers.host = request.headers.host || request.host;
    request.path = request.path || "/";
    return request;
}
```
- example usage
```shell
...

exports.Client = Client;
function Client(fs) {
var self = Object.create(Client.prototype);

self.request = function (request) {
    return Q.when(request, function (request) {
        request = HTTP.normalizeRequest(request);
        var url = URL.parse(request.url);
        if (url.protocol !== "file:") {
            return {
                status: 404,
                headers: {},
                body: ["Can't access protocol " + url.protocol]
            };
...
```

#### <a name="apidoc.element.q-io.http.normalizeResponse"></a>[function <span class="apidocSignatureSpan">q-io.http.</span>normalizeResponse (response)](#apidoc.element.q-io.http.normalizeResponse)
- description and source-code
```javascript
normalizeResponse = function (response) {
    if (response === void 0) {
        return;
    }
    if (typeof response == "string") {
        response = [response];
    }
    if (response.forEach) {
        response = {
            status: 200,
            headers: {},
            body: response
        }
    }
    return response;
}
```
- example usage
```shell
...
var RouteApps = require("./route");
var StatusApps = require("./status");

exports.Normalize = function (app) {
return function (request, response) {
    var request = HTTP.normalizeRequest(request);
    return Q.when(app(request, response), function (response) {
        return HTTP.normalizeResponse(response);
    });
};
};

exports.Date = function (app, present) {
present = present || function () {
    return new Date();
...
```

#### <a name="apidoc.element.q-io.http.read"></a>[function <span class="apidocSignatureSpan">q-io.http.</span>read (request, qualifier)](#apidoc.element.q-io.http.read)
- description and source-code
```javascript
read = function (request, qualifier) {
    qualifier = qualifier || function (response) {
        return response.status === 200;
    };
    return Q.when(exports.request(request), function (response) {
        if (!qualifier(response)){
            var error = new Error("HTTP request failed with code " + response.status);
            error.response = response;
            throw error;
        }
        return Q.post(response.body, 'read', []);
    });
}
```
- example usage
```shell
...
into memory.  It returns a promise for the whole file contents.  By
default, 'read' provides a string decoded from UTF-8.  With the bytewise
mode flag, provides a 'Buffer'.

The options argument is identical to that of 'open'.

'''javascript
return FS.read(__filename, "b")
.then(function (content) {
    // ...
})
'''

'''javascript
return FS.read(__filename, {
...
```

#### <a name="apidoc.element.q-io.http.request"></a>[function <span class="apidocSignatureSpan">q-io.http.</span>request (request)](#apidoc.element.q-io.http.request)
- description and source-code
```javascript
request = function (request) {
    return Q.when(request, function (request) {

        request = exports.normalizeRequest(request);

        var deferred = Q.defer();
        var http = request.ssl ? HTTPS : HTTP;

        var requestOptions = {
            hostname: request.hostname,
            port: request.port || (request.ssl ? 443 : 80),
            localAddress: request.localAddress,
            socketPath: request.socketPath,
            method: request.method,
            path: request.path,
            headers: request.headers,
            auth: request.auth // Generates the appropriate header
        };

        if (request.agent !== undefined) {
            requestOptions.agent = request.agent;
        }

        var _request = http.request(requestOptions, function (_response) {
            deferred.resolve(exports.ClientResponse(_response, request.charset));
            _response.on("error", function (error) {
                // TODO find a better way to channel
                // this into the response
                console.warn(error && error.stack || error);
                deferred.reject(error);
            });
        });

        _request.on("error", function (error) {
            deferred.reject(error);
        });

        if (request.timeout) {
            _request.setTimeout(request.timeout, function() {
                _request.abort();
            });
        }

        Q.when(request.body, function (body) {
            var end, done;
            if (body) {
                done = body.forEach(function (chunk) {
                    end = Q.when(end, function () {
                        return Q.when(chunk, function (chunk) {
                            _request.write(chunk, request.charset);
                        });
                    });
                });
            }
            return Q.when(end, function () {
                return Q.when(done, function () {
                    _request.end();
                });
            });
        }).done();

        return deferred.promise;
    });
}
```
- example usage
```shell
...
    });
};

self.read = function (request, qualifier) {
    qualifier = qualifier || function (response) {
        return response.status === 200;
    };
    return Q.when(exports.request(request), function (response) {
        if (!qualifier(response)){
            var error = new Error("HTTP request failed with code " + response.status);
            error.response = response;
            throw error;
        }
        return Q.invoke(response.body, "read");
    });
...
```



# <a name="apidoc.module.q-io.http_apps"></a>[module q-io.http_apps](#apidoc.module.q-io.http_apps)

#### <a name="apidoc.element.q-io.http_apps.Branch"></a>[function <span class="apidocSignatureSpan">q-io.http_apps.</span>Branch (paths, notFound)](#apidoc.element.q-io.http_apps.Branch)
- description and source-code
```javascript
Branch = function (paths, notFound) {
    if (!paths)
        paths = {};
    if (!notFound)
        notFound = StatusApps.notFound;
    return function (request, response) {
        if (!/^\//.test(request.pathInfo)) {
            return notFound(request, response);
        }
        var path = request.pathInfo.slice(1);
        var parts = path.split("/");
        var part = decodeURIComponent(parts.shift());
        if (Object.has(paths, part)) {
            request.scriptName = request.scriptName + part + "/";
            request.pathInfo = path.slice(part.length);
            return Object.get(paths, part)(request, response);
        }
        return notFound(request, response);
    };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.q-io.http_apps.Cap"></a>[function <span class="apidocSignatureSpan">q-io.http_apps.</span>Cap (app, notFound)](#apidoc.element.q-io.http_apps.Cap)
- description and source-code
```javascript
Cap = function (app, notFound) {
    notFound = notFound || StatusApps.notFound;
    return function (request, response) {
        // TODO Distinguish these cases
        if (request.pathInfo === "" || request.pathInfo === "/") {
            return app(request, response);
        } else {
            return notFound(request, response);
        }
    };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.q-io.http_apps.Chain"></a>[function <span class="apidocSignatureSpan">q-io.http_apps.</span>Chain (end)](#apidoc.element.q-io.http_apps.Chain)
- description and source-code
```javascript
function Chain(end) {
    var self = Object.create(Chain.prototype);
    self.end = end || function (next) {
        return next;
    };
    return self;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.q-io.http_apps.Charset"></a>[function <span class="apidocSignatureSpan">q-io.http_apps.</span>Charset (types, notAcceptable)](#apidoc.element.q-io.http_apps.Charset)
- description and source-code
```javascript
Charset = function (types, notAcceptable) {
    var keys = Object.keys(types);
    if (!notAcceptable)
        notAcceptable = Status.notAcceptable;
    return function (request) {
        var accept = request.headers[requestHeader] || "*";
        var type = MimeParse.bestMatch(keys, accept);
        request.terms = request.terms || {};
        request.terms[responseHeader] = type;
        if (Object.has(keys, type)) {
            return Q.when(types[type](request), function (response) {
                if (
                    respond !== null &&
                    response &&
                    response.status === 200 &&
                    response.headers
                ) {
                    response.headers[responseHeader] = type;
                }
                return response;
            });
        } else {
            return notAcceptable(request);
        }
    };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.q-io.http_apps.Content"></a>[function <span class="apidocSignatureSpan">q-io.http_apps.</span>Content (body, contentType, status)](#apidoc.element.q-io.http_apps.Content)
- description and source-code
```javascript
Content = function (body, contentType, status) {
    return function () {
        return exports.content(body, contentType, status);
    };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.q-io.http_apps.ContentRequest"></a>[function <span class="apidocSignatureSpan">q-io.http_apps.</span>ContentRequest (app)](#apidoc.element.q-io.http_apps.ContentRequest)
- description and source-code
```javascript
ContentRequest = function (app) {
    return function (request, response) {
        return Q.when(request.body.read(), function (body) {
            return app(body, request, response);
        });
    };
}
```
- example usage
```shell
...
 * @param {Function(Request, Object):Response} app
 * @param {App} badRequest
 * @returns {App}
 */
exports.JsonRequest = function (app, badRequest) {
if (!badRequest)
    badRequest = Status.badRequest;
return Content.ContentRequest(function (content, request, response) {
    try {
        var object = JSON.parse(content);
    } catch (error) {
        return badRequest(request, error);
    }
    return app(object, request, response);
});
...
```

#### <a name="apidoc.element.q-io.http_apps.ContentType"></a>[function <span class="apidocSignatureSpan">q-io.http_apps.</span>ContentType (types, notAcceptable)](#apidoc.element.q-io.http_apps.ContentType)
- description and source-code
```javascript
ContentType = function (types, notAcceptable) {
    var keys = Object.keys(types);
    if (!notAcceptable)
        notAcceptable = Status.notAcceptable;
    return function (request) {
        var accept = request.headers[requestHeader] || "*";
        var type = MimeParse.bestMatch(keys, accept);
        request.terms = request.terms || {};
        request.terms[responseHeader] = type;
        if (Object.has(keys, type)) {
            return Q.when(types[type](request), function (response) {
                if (
                    respond !== null &&
                    response &&
                    response.status === 200 &&
                    response.headers
                ) {
                    response.headers[responseHeader] = type;
                }
                return response;
            });
        } else {
            return notAcceptable(request);
        }
    };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.q-io.http_apps.CookieJar"></a>[function <span class="apidocSignatureSpan">q-io.http_apps.</span>CookieJar (app)](#apidoc.element.q-io.http_apps.CookieJar)
- description and source-code
```javascript
CookieJar = function (app) {
    var hostCookies = {}; // to {} of pathCookies to [] of cookies
    return function (request) {

        if (!request.headers.host) {
            throw new Error("Requests must have a host header");
        }
        var hosts = allHostsContaining(request.headers.host);

        var now = new Date();

        // delete expired cookies
        for (var host in hostCookies) {
            var pathCookies = hostCookies[host];
            for (var path in pathCookies) {
                var cookies = pathCookies[path];
                for (var name in cookies) {
                    var cookie = cookies[name];
                    if (cookie.expires && cookie.expires > now) {
                        delete cookie[name];
                    }
                }
            }
        }

        // collect applicable cookies
        var requestCookies = concat(
            Object.keys(hostCookies)
            .map(function (host) {
                if (!hostContains(host, request.headers.host)) {
                    return [];
                }
                var pathCookies = hostCookies[host];
                return concat(
                    Object.keys(pathCookies)
                    .map(function (path) {
                        if (!pathContains(path, request.path))
                            return [];
                        var cookies = pathCookies[path];
                        return (
                            Object.keys(cookies)
                            .map(function (name) {
                                return cookies[name];
                            })
                            .filter(function (cookie) {
                                return cookie.secure ?
                                    request.ssl :
                                    true;
                            })
                        );
                    })
                )
            })
        );

        if (requestCookies.length) {
            request.headers["cookie"] = (
                requestCookies
                .map(function (cookie) {
                    return Cookie.stringify(
                        cookie.key,
                        cookie.value
                    );
                })
                .join("; ")
            );
        }

        return Q.when(app.apply(this, arguments), function (response) {
            response.headers = response.headers || {};
            if (response.headers["set-cookie"]) {
                var host = request.headers.host;
                var hostParts = splitHost(host);
                var hostname = hostParts[0];
                var requestHost = ipRe.test(hostname) ? host : "." + host;
                // normalize to array
                if (!Array.isArray(response.headers["set-cookie"])) {
                    response.headers["set-cookie"] = [response.headers["set-cookie"]];
                }
                response.headers["set-cookie"].forEach(function (cookie) {
                    var date = response.headers["date"] ?
                        new Date(response.headers["date"]) :
                        new Date();
                    cookie = Cookie.parse(cookie, date);
                    // ignore illegal host
                    if (cookie.host && !hostContains(requestHost, cookie.host))
                        delete cookie.host;
                    var host = requestHost || cookie.host;
                    var path = cookie.path || "/";
                    var pathCookies = hostCookies[host] = hostCookies[host] || {};
                    var cookies = pathCookies[path] = pathCookies[path] || {};
                    cookies[cookie.key] = cookie;
                })
                delete response.headers["set-cookie"];
            }

            return response;
        });

    };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.q-io.http_apps.Date"></a>[function <span class="apidocSignatureSpan">q-io.http_apps.</span>Date (app, present)](#apidoc.element.q-io.http_apps.Date)
- description and source-code
```javascript
Date = function (app, present) {
    present = present || function () {
        return new Date();
    };
    return RouteApps.Trap(app, function (response, request) {
        response.headers["date"] = "" + present();
    });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.q-io.http_apps.Debug"></a>[function <span class="apidocSignatureSpan">q-io.http_apps.</span>Debug (app)](#apidoc.element.q-io.http_apps.Debug)
- description and source-code
```javascript
Debug = function (app) {
    return exports.Error(app, true);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.q-io.http_apps.Decorators"></a>[function <span class="apidocSignatureSpan">q-io.http_apps.</span>Decorators (decorators, app)](#apidoc.element.q-io.http_apps.Decorators)
- description and source-code
```javascript
Decorators = function (decorators, app) {
    decorators.reversed().forEach(function (Middleware) {
        app = Middleware(app);
    });
    return app;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.q-io.http_apps.DirectoryIndex"></a>[function <span class="apidocSignatureSpan">q-io.http_apps.</span>DirectoryIndex (app, indexFile)](#apidoc.element.q-io.http_apps.DirectoryIndex)
- description and source-code
```javascript
DirectoryIndex = function (app, indexFile) {
    indexFile = indexFile || "index.html";
    return function (request) {
        request.directoryIndex = true;
        request.location = URL.parse(request.path);
        // redirect index.html to containing directory
        // TODO worry about whether this file actually exists
        if (request.location.file === indexFile) {
            return RedirectApps.redirect(request, ".");
        } else {
            return Q.fcall(app, request)
            .then(function (response) {
                if (response.directory !== void 0) {
                    if (request.location.file) {
                        return RedirectApps.redirect(request, request.location.file + "/");
                    } else {
                        var index = request.fs.join(response.directory, indexFile);
                        return Q.invoke(request.fs, "isFile", index)
                        .then(function (isFile) {
                            if (isFile) {
                                request.url = URL.resolve(request.url, indexFile);
                                request.pathInfo += indexFile;
                                return app(request);
                            } else {
                                return response;
                            }
                        });
                    }
                } else {
                    return response;
                }
            });
        }
    };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.q-io.http_apps.Encoding"></a>[function <span class="apidocSignatureSpan">q-io.http_apps.</span>Encoding (types, notAcceptable)](#apidoc.element.q-io.http_apps.Encoding)
- description and source-code
```javascript
Encoding = function (types, notAcceptable) {
    var keys = Object.keys(types);
    if (!notAcceptable)
        notAcceptable = Status.notAcceptable;
    return function (request) {
        var accept = request.headers[requestHeader] || "*";
        var type = MimeParse.bestMatch(keys, accept);
        request.terms = request.terms || {};
        request.terms[responseHeader] = type;
        if (Object.has(keys, type)) {
            return Q.when(types[type](request), function (response) {
                if (
                    respond !== null &&
                    response &&
                    response.status === 200 &&
                    response.headers
                ) {
                    response.headers[responseHeader] = type;
                }
                return response;
            });
        } else {
            return notAcceptable(request);
        }
    };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.q-io.http_apps.Error"></a>[function <span class="apidocSignatureSpan">q-io.http_apps.</span>Error (app, debug)](#apidoc.element.q-io.http_apps.Error)
- description and source-code
```javascript
Error = function (app, debug) {
    return function (request, response) {
        return Q.when(app(request, response), null, function (error) {
            if (!debug)
                error = undefined;
            return StatusApps.responseForStatus(request, 500, error && error.stack || error);
        });
    };
}
```
- example usage
```shell
...
               error = undefined;
           return StatusApps.responseForStatus(request, 500, error && error.stack || error);
       });
   };
};

exports.Debug = function (app) {
   return exports.Error(app, true);
};

/**
* Decorates a Q-JSGI application such that all requests and responses
* are logged.
*
* @param {App} app
...
```

#### <a name="apidoc.element.q-io.http_apps.File"></a>[function <span class="apidocSignatureSpan">q-io.http_apps.</span>File (path, contentType)](#apidoc.element.q-io.http_apps.File)
- description and source-code
```javascript
File = function (path, contentType) {
    return function (request, response) {
        return exports.file(request, String(path), contentType);
    };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.q-io.http_apps.FileTree"></a>[function <span class="apidocSignatureSpan">q-io.http_apps.</span>FileTree (root, options)](#apidoc.element.q-io.http_apps.FileTree)
- description and source-code
```javascript
FileTree = function (root, options) {
    if (!options)
        options = {};
    options.notFound = options.notFound || StatusApps.notFound;
    options.file = options.file || exports.file;
    options.directory = options.directory || exports.directory;
    options.fs = options.fs || FS;
    var fs = options.fs;
    root = fs.canonical(root);
    return function (request, response) {
        var location = URL.parse(request.url);
        request.fs = fs;
        var redirect = options.redirect || (
            request.permanent || options.permanent ?
            RedirectApps.permanentRedirect :
            RedirectApps.temporaryRedirect
        );
        return Q.when(root, function (root) {
            var path = fs.join(root, request.pathInfo.slice(1));
            return Q.when(fs.canonical(path), function (canonical) {
                //TODO remove for 2.0.0
                if (options.followInsecureSymlinks) {
                    Deprecate.deprecationWarning("followInsecureSymlinks", "followInsecureSymbolicLinks");
                    options.followInsecureSymbolicLinks = true;
                }
                if (!fs.contains(root, canonical) && !options.followInsecureSymbolicLinks)
                    return options.notFound(request, response);
                if (path !== canonical && options.redirectSymbolicLinks)
                    return redirect(request, fs.relativeFromFile(path, canonical));
                // TODO: relativeFromFile should be designed for URL’s, not generalized paths.
                // HTTP.relative(pathToDirectoryLocation(path), pathToFile/DirectoryLocation(canonical))
                return Q.when(fs.stat(canonical), function (stat) {
                    if (stat.isFile()) {
                        return options.file(request, canonical, options.contentType, fs);
                    } else if (stat.isDirectory()) {
                        return options.directory(request, canonical, options.contentType, fs);
                    } else {
                        return options.notFound(request, response);
                    }
                });
            }, function (reason) {
                return options.notFound(request, response);
            });
        });
    };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.q-io.http_apps.HandleHtmlFragmentResponses"></a>[function <span class="apidocSignatureSpan">q-io.http_apps.</span>HandleHtmlFragmentResponses (app, handleHtmlFragmentResponse)](#apidoc.element.q-io.http_apps.HandleHtmlFragmentResponses)
- description and source-code
```javascript
HandleHtmlFragmentResponses = function (app, handleHtmlFragmentResponse) {
    handleHtmlFragmentResponse = handleHtmlFragmentResponse || exports.handleHtmlFragmentResponse;
    return function (request) {
        request.handleHtmlFragmentResponse = handleHtmlFragmentResponse;
        return Q.fcall(app, request)
        .then(function (response) {
            if (response.htmlFragment) {
                return Q.fcall(handleHtmlFragmentResponse, response);
            } else {
                return response;
            }
        });
    };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.q-io.http_apps.HandleJsonResponses"></a>[function <span class="apidocSignatureSpan">q-io.http_apps.</span>HandleJsonResponses (app, reviver, tab)](#apidoc.element.q-io.http_apps.HandleJsonResponses)
- description and source-code
```javascript
HandleJsonResponses = function (app, reviver, tab) {
    return function (request) {
        request.handleJsonResponse = exports.handleJsonResponse;
        return Q.fcall(app, request)
        .then(function (response) {
            if (response.data !== void 0) {
                return Q.fcall(exports.handleJsonResponse, response, reviver, tab);
            } else {
                return response;
            }
        });
    };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.q-io.http_apps.Headers"></a>[function <span class="apidocSignatureSpan">q-io.http_apps.</span>Headers (app, headers)](#apidoc.element.q-io.http_apps.Headers)
- description and source-code
```javascript
Headers = function (app, headers) {
    return function (request, response) {
        return Q.when(app(request, response), function (response) {
            if (response && response.headers) {
                Object.keys(headers).forEach(function (key) {
                    if (!(key in response.headers)) {
                        response.headers[key] = headers[key];
                    }
                });
            }
            return response;
        });
    };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.q-io.http_apps.Host"></a>[function <span class="apidocSignatureSpan">q-io.http_apps.</span>Host (appForHost, notAcceptable)](#apidoc.element.q-io.http_apps.Host)
- description and source-code
```javascript
Host = function (appForHost, notAcceptable) {
    var table = Object.keys(appForHost).map(function (pattern) {
        var parts = pattern.split(":");
        return [
            pattern,
            parts[0] || "*",
            parts[1] || "*",
            appForHost[pattern]
        ];
    });
    if (!notAcceptable) {
        notAcceptable = Status.notAcceptable;
    }
    return function (request) {
        // find first matching host for app
        for (var index = 0; index < table.length; index++) {
            var row = table[index]; // [hostname, port, app]
            var pattern = row[0];
            var hostname = row[1];
            var port = row[2];
            var app = row[3];
            if (
                (hostname === "*" || hostname === request.hostname) &&
                (port === "*" || port === "" + request.port)
            ) {
                request.terms = request.terms || {};
                request.terms.host = pattern;
                return app(request);
            }
        }
        return notAcceptable(request);
    };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.q-io.http_apps.Inspect"></a>[function <span class="apidocSignatureSpan">q-io.http_apps.</span>Inspect (app)](#apidoc.element.q-io.http_apps.Inspect)
- description and source-code
```javascript
Inspect = function (app) {
    return Negotiate.Method({"GET": function (request, response) {
        return Q.when(app(request, response), function (object) {
            return {
                status: 200,
                headers: {
                    "content-type": "text/plain"
                },
                body: [inspect(object)]
            }
        });
    }});
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.q-io.http_apps.Json"></a>[function <span class="apidocSignatureSpan">q-io.http_apps.</span>Json (app, reviver, tabs)](#apidoc.element.q-io.http_apps.Json)
- description and source-code
```javascript
Json = function (app, reviver, tabs) {
    return function (request, response) {
        return Q.when(app(request, response), function (object) {
            return exports.json(object, reviver, tabs);
        });
    };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.q-io.http_apps.JsonRequest"></a>[function <span class="apidocSignatureSpan">q-io.http_apps.</span>JsonRequest (app, badRequest)](#apidoc.element.q-io.http_apps.JsonRequest)
- description and source-code
```javascript
JsonRequest = function (app, badRequest) {
    if (!badRequest)
        badRequest = Status.badRequest;
    return Content.ContentRequest(function (content, request, response) {
        try {
            var object = JSON.parse(content);
        } catch (error) {
            return badRequest(request, error);
        }
        return app(object, request, response);
    });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.q-io.http_apps.Language"></a>[function <span class="apidocSignatureSpan">q-io.http_apps.</span>Language (types, notAcceptable)](#apidoc.element.q-io.http_apps.Language)
- description and source-code
```javascript
Language = function (types, notAcceptable) {
    var keys = Object.keys(types);
    if (!notAcceptable)
        notAcceptable = Status.notAcceptable;
    return function (request) {
        var accept = request.headers[requestHeader] || "*";
        var type = MimeParse.bestMatch(keys, accept);
        request.terms = request.terms || {};
        request.terms[responseHeader] = type;
        if (Object.has(keys, type)) {
            return Q.when(types[type](request), function (response) {
                if (
                    respond !== null &&
                    response &&
                    response.status === 200 &&
                    response.headers
                ) {
                    response.headers[responseHeader] = type;
                }
                return response;
            });
        } else {
            return notAcceptable(request);
        }
    };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.q-io.http_apps.ListDirectories"></a>[function <span class="apidocSignatureSpan">q-io.http_apps.</span>ListDirectories (app, listDirectory)](#apidoc.element.q-io.http_apps.ListDirectories)
- description and source-code
```javascript
ListDirectories = function (app, listDirectory) {
    listDirectory = listDirectory || exports.listDirectory;
    return function (request) {
        if (request.directoryIndex) {
            throw new Error("DirectoryIndex must be used after ListDirectories");
        }
        request.listDirectories = true;
        return Q.fcall(app, request)
        .then(function (response) {
            if (response.directory !== void 0) {
                return listDirectory(request, response);
            } else {
                return response;
            }
        });
    };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.q-io.http_apps.Log"></a>[function <span class="apidocSignatureSpan">q-io.http_apps.</span>Log (app, log, stamp)](#apidoc.element.q-io.http_apps.Log)
- description and source-code
```javascript
Log = function (app, log, stamp) {
    log = log || console.log;
    stamp = stamp || function (message) {
        return new Date().toISOString() + " " + message;
    };
    return function (request, response) {
        var remoteHost =
            request.remoteHost + ":" +
            request.remotePort;
        var requestLine =
            request.method + " " +
            request.path + " " +
            "HTTP/" + request.version.join(".");
        log(stamp(
            remoteHost + " " +
            "-->     " +
            requestLine
        ));
        return Q.when(app(request, response), function (response) {
            if (response) {
                log(stamp(
                    remoteHost + " " +
                    "<== " +
                    response.status + " " +
                    requestLine + " " +
                    (response.headers["content-length"] || "-")
                ));
            } else {
                log(stamp(
                    remoteHost + " " +
                    "... " +
                    "... " +
                    requestLine + " (response undefined / presumed streaming)"
                ));
            }
            return response;
        }, function (reason) {
            log(stamp(
                remoteHost + " " +
                "!!!     " +
                requestLine + " " +
                (reason && reason.message || reason)
            ));
            return Q.reject(reason);
        });
    };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.q-io.http_apps.Method"></a>[function <span class="apidocSignatureSpan">q-io.http_apps.</span>Method (methods, methodNotAllowed)](#apidoc.element.q-io.http_apps.Method)
- description and source-code
```javascript
Method = function (methods, methodNotAllowed) {
    var keys = Object.keys(methods);
    if (!methodNotAllowed)
        methodNotAllowed = Status.methodNotAllowed;
    return function (request) {
        var method = request.method;
        if (Object.has(keys, method)) {
            return Object.get(methods, method)(request);
        } else {
            return methodNotAllowed(request);
        }
    };
}
```
- example usage
```shell
...
};

/**
 * @param {Function(Request):Object}
 * @returns {App}
 */
exports.Inspect = function (app) {
return Negotiate.Method({"GET": function (request, response) {
    return Q.when(app(request, response), function (object) {
        return {
            status: 200,
            headers: {
                "content-type": "text/plain"
            },
            body: [inspect(object)]
...
```

#### <a name="apidoc.element.q-io.http_apps.Normalize"></a>[function <span class="apidocSignatureSpan">q-io.http_apps.</span>Normalize (app)](#apidoc.element.q-io.http_apps.Normalize)
- description and source-code
```javascript
Normalize = function (app) {
    return function (request, response) {
        var request = HTTP.normalizeRequest(request);
        return Q.when(app(request, response), function (response) {
            return HTTP.normalizeResponse(response);
        });
    };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.q-io.http_apps.ParseQuery"></a>[function <span class="apidocSignatureSpan">q-io.http_apps.</span>ParseQuery (app)](#apidoc.element.q-io.http_apps.ParseQuery)
- description and source-code
```javascript
ParseQuery = function (app) {
    return function (request, response) {
        request.query = QS.parse(URL.parse(request.url).query || "");
        return app(request, response);
    };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.q-io.http_apps.Permanent"></a>[function <span class="apidocSignatureSpan">q-io.http_apps.</span>Permanent (app, future)](#apidoc.element.q-io.http_apps.Permanent)
- description and source-code
```javascript
Permanent = function (app, future) {
    future = future || function () {
        return new Date(new Date().getTime() + farFuture);
    };
    app = RouteApps.Tap(app, function (request, response) {
        request.permanent = future;
    });
    app = RouteApps.Trap(app, function (response, request) {
        response.headers["expires"] = "" + future();
    });
    return app;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.q-io.http_apps.PermanentRedirect"></a>[function <span class="apidocSignatureSpan">q-io.http_apps.</span>PermanentRedirect (location, status, tree)](#apidoc.element.q-io.http_apps.PermanentRedirect)
- description and source-code
```javascript
PermanentRedirect = function (location, status, tree) {
    return function (request, response) {
        return exports.permanentRedirect(request, location, status, tree);
    };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.q-io.http_apps.PermanentRedirectTree"></a>[function <span class="apidocSignatureSpan">q-io.http_apps.</span>PermanentRedirectTree (location, status)](#apidoc.element.q-io.http_apps.PermanentRedirectTree)
- description and source-code
```javascript
PermanentRedirectTree = function (location, status) {
    return function (request, response) {
        return exports.permanentRedirect(request, location, status, true);
    };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.q-io.http_apps.Proxy"></a>[function <span class="apidocSignatureSpan">q-io.http_apps.</span>Proxy (app)](#apidoc.element.q-io.http_apps.Proxy)
- description and source-code
```javascript
Proxy = function (app) {
    if (typeof app === "string") {
        var location = app;
        app = function (request) {
            request.url = location;
            return request;
        };
    }
    return function (request, response) {
        return Q.when(app.apply(this, arguments), function (request) {
            return HTTP.request(request);
        });
    };
}
```
- example usage
```shell
...
        return Q.when(app.apply(this, arguments), function (request) {
            return HTTP.request(request);
        });
    };
};

exports.ProxyTree = function (url) {
    return exports.Proxy(function (request) {
        request.url = URL.resolve(url, request.pathInfo.replace(/^\//, ""));
        return request;
    });
};
...
```

#### <a name="apidoc.element.q-io.http_apps.ProxyTree"></a>[function <span class="apidocSignatureSpan">q-io.http_apps.</span>ProxyTree (url)](#apidoc.element.q-io.http_apps.ProxyTree)
- description and source-code
```javascript
ProxyTree = function (url) {
    return exports.Proxy(function (request) {
        request.url = URL.resolve(url, request.pathInfo.replace(/^\//, ""));
        return request;
    });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.q-io.http_apps.Redirect"></a>[function <span class="apidocSignatureSpan">q-io.http_apps.</span>Redirect (location, status, tree)](#apidoc.element.q-io.http_apps.Redirect)
- description and source-code
```javascript
Redirect = function (location, status, tree) {
    return function (request, response) {
        return exports.redirect(request, location, status, tree);
    };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.q-io.http_apps.RedirectTrap"></a>[function <span class="apidocSignatureSpan">q-io.http_apps.</span>RedirectTrap (app, maxRedirects)](#apidoc.element.q-io.http_apps.RedirectTrap)
- description and source-code
```javascript
RedirectTrap = function (app, maxRedirects) {
    maxRedirects = maxRedirects || 20;
    return function (request, response) {
        var remaining = maxRedirects;
        var deferred = Q.defer();
        var self = this;
        var args = arguments;

        request = Http.normalizeRequest(request);

        // try redirect loop
        function next() {
            Q.fcall(function () {
                return app(request, response);
            })
            .then(function (response) {
                if (exports.isRedirect(response)) {
                    if (remaining--) {
                        request.url = response.headers.location;
                        next();
                    } else {
                        throw new Error("Maximum redirects.");
                    }
                } else {
                    deferred.resolve(response);
                }
            })
            .fail(deferred.reject)
        }
        next();

        return deferred.promise;
    };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.q-io.http_apps.RedirectTree"></a>[function <span class="apidocSignatureSpan">q-io.http_apps.</span>RedirectTree (location, status)](#apidoc.element.q-io.http_apps.RedirectTree)
- description and source-code
```javascript
RedirectTree = function (location, status) {
    return function (request, response) {
        return exports.redirect(request, location, status, true);
    };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.q-io.http_apps.Select"></a>[function <span class="apidocSignatureSpan">q-io.http_apps.</span>Select (select)](#apidoc.element.q-io.http_apps.Select)
- description and source-code
```javascript
Select = function (select) {
    return function (request) {
        return Q.when(select(request), function (app) {
            return app(request);
        });
    };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.q-io.http_apps.Tap"></a>[function <span class="apidocSignatureSpan">q-io.http_apps.</span>Tap (app, tap)](#apidoc.element.q-io.http_apps.Tap)
- description and source-code
```javascript
Tap = function (app, tap) {
    return function (request, response) {
        var self = this, args = arguments;
        return Q.when(tap.apply(this, arguments), function (response) {
            if (response) {
                return response;
            } else {
                return app.apply(self, args);
            }
        });
    };
}
```
- example usage
```shell
...
    24 * // h
    365 * // d
    10; // years
exports.Permanent = function (app, future) {
    future = future || function () {
        return new Date(new Date().getTime() + farFuture);
    };
    app = RouteApps.Tap(app, function (request, response) {
        request.permanent = future;
    });
    app = RouteApps.Trap(app, function (response, request) {
        response.headers["expires"] = "" + future();
    });
    return app;
};
...
```

#### <a name="apidoc.element.q-io.http_apps.TemporaryRedirect"></a>[function <span class="apidocSignatureSpan">q-io.http_apps.</span>TemporaryRedirect (location, status, tree)](#apidoc.element.q-io.http_apps.TemporaryRedirect)
- description and source-code
```javascript
TemporaryRedirect = function (location, status, tree) {
    return function (request, response) {
        return exports.temporaryRedirect(request, location, status, tree);
    };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.q-io.http_apps.TemporaryRedirectTree"></a>[function <span class="apidocSignatureSpan">q-io.http_apps.</span>TemporaryRedirectTree (location, status)](#apidoc.element.q-io.http_apps.TemporaryRedirectTree)
- description and source-code
```javascript
TemporaryRedirectTree = function (location, status) {
    return function (request, response) {
        return exports.temporaryRedirect(request, location, status, true);
    };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.q-io.http_apps.Time"></a>[function <span class="apidocSignatureSpan">q-io.http_apps.</span>Time (app)](#apidoc.element.q-io.http_apps.Time)
- description and source-code
```javascript
Time = function (app) {
    return function (request, response) {
        var start = new Date();
        return Q.when(app(request, response), function (response) {
            var stop = new Date();
            if (response && response.headers) {
                response.headers["x-response-time"] = "" + (stop - start);
            }
            return response;
        });
    };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.q-io.http_apps.Trap"></a>[function <span class="apidocSignatureSpan">q-io.http_apps.</span>Trap (app, trap)](#apidoc.element.q-io.http_apps.Trap)
- description and source-code
```javascript
Trap = function (app, trap) {
    return function (request, response) {
        return Q.when(app.apply(this, arguments), function (response) {
            if (response) {
                response.headers = response.headers || {};
                return trap(response, request) || response;
            }
        });
    };
}
```
- example usage
```shell
...
   };
};

exports.Date = function (app, present) {
   present = present || function () {
       return new Date();
   };
   return RouteApps.Trap(app, function (response, request) {
       response.headers["date"] = "" + present();
   });
};

/**
* Decorates a JSGI application such that rejected response promises
* get translated into '500' server error responses with no content.
...
```

#### <a name="apidoc.element.q-io.http_apps.appForStatus"></a>[function <span class="apidocSignatureSpan">q-io.http_apps.</span>appForStatus (status)](#apidoc.element.q-io.http_apps.appForStatus)
- description and source-code
```javascript
appForStatus = function (status) {
    return function (request) {
        return exports.responseForStatus(request, status, request.method + " " + request.path);
    };
}
```
- example usage
```shell
...
       }
   }
};

/**
* {App} an application that returns a 400 response.
*/
exports.badRequest = exports.appForStatus(400);
/**
* {App} an application that returns a 404 response.
*/
exports.notFound = exports.appForStatus(404);
/**
* {App} an application that returns a 405 response.
*/
...
```

#### <a name="apidoc.element.q-io.http_apps.badRequest"></a>[function <span class="apidocSignatureSpan">q-io.http_apps.</span>badRequest (request)](#apidoc.element.q-io.http_apps.badRequest)
- description and source-code
```javascript
badRequest = function (request) {
    return exports.responseForStatus(request, status, request.method + " " + request.path);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.q-io.http_apps.content"></a>[function <span class="apidocSignatureSpan">q-io.http_apps.</span>content (content, contentType, status)](#apidoc.element.q-io.http_apps.content)
- description and source-code
```javascript
content = function (content, contentType, status) {
    status = status || 200;
    content = content || "";
    if (typeof content === "string") {
        content = [content];
    }
    contentType = contentType || "text/plain";
    return {
        "status": status,
        "headers": {
            "content-type": contentType
        },
        "body": content
    };
}
```
- example usage
```shell
...
* response body
* @param {String} contentType
* @param {Number} status
* @returns {App} a Q-JSGI app
*/
exports.Content = function (body, contentType, status) {
   return function () {
       return exports.content(body, contentType, status);
   };
};

/**
* Returns a Q-JSGI response with the given content.
* @param {Body} content (optional) defaults to '[""]'
* @param {String} contentType (optional) defaults to '"text/plain"'
...
```

#### <a name="apidoc.element.q-io.http_apps.directory"></a>[function <span class="apidocSignatureSpan">q-io.http_apps.</span>directory (request, path)](#apidoc.element.q-io.http_apps.directory)
- description and source-code
```javascript
directory = function (request, path) {
    var response = StatusApps.notFound(request);
    response.directory = path;
    return response;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.q-io.http_apps.escapeHtml"></a>[function <span class="apidocSignatureSpan">q-io.http_apps.</span>escapeHtml (text)](#apidoc.element.q-io.http_apps.escapeHtml)
- description and source-code
```javascript
function escapeHtml(text) {
    return String(text)
        .replace(/&/g, "&amp;")
        .replace(/</g, "&lt;")
        .replace(/>/g, "&gt;")
        .replace(/"/g, "&quot;")
}
```
- example usage
```shell
...
headers: {
    location: location,
    "content-type": "text/html"
},
htmlTitle: title,
htmlFragment: {
    forEach: function (write) {
        write("<h1>" + HtmlApps.escapeHtml(title) + "</h1>\n");
        write(
            "<p>See: <a href=\"" + HtmlApps.escapeHtml(location) + "\">" +
            HtmlApps.escapeHtml(location) +
            "</a></p>\n"
        );
    }
}
...
```

#### <a name="apidoc.element.q-io.http_apps.etag"></a>[function <span class="apidocSignatureSpan">q-io.http_apps.</span>etag (stat)](#apidoc.element.q-io.http_apps.etag)
- description and source-code
```javascript
etag = function (stat) {
    return [
        stat.node.ino,
        stat.size,
        stat.lastModified().getTime()
    ].join("-");
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.q-io.http_apps.file"></a>[function <span class="apidocSignatureSpan">q-io.http_apps.</span>file (request, path, contentType, fs)](#apidoc.element.q-io.http_apps.file)
- description and source-code
```javascript
file = function (request, path, contentType, fs) {
    fs = fs || FS;
    // TODO last-modified header
    contentType = contentType || MimeTypes.lookup(path);
    return Q.when(fs.stat(path), function (stat) {
        var etag = exports.etag(stat);
        var options = {
            flags: "rb"
        };
        var range;
        var status = 200;
        var headers = {
            "content-type": contentType,
            etag: etag
        };

        // Partial range requests
        if ("range" in request.headers) {
            // Invalid cache
            if (
                "if-range" in request.headers &&
                etag != request.headers["if-range"]
            ) {
                // Normal 200 for entire, altered content
            } else {
                // Truncate to the first requested continuous range
                range = interpretFirstRange(request.headers["range"], stat.size);
                // Like Apache, ignore the range header if it is invalid
                if (range) {
                    if (range.end > stat.size) {
                        range.end = stat.size;
                    }
                    if (range.end <= range.begin) {
                        return StatusApps.responseForStatus(request, 416); // not satisfiable
                    }
                    status = 206; // partial content
                    headers["content-range"] = (
                        "bytes " +
                        range.begin + "-" + (range.end - 1) +
                        "/" + stat.size
                    );
                    headers["content-length"] = "" + (range.end - range.begin);
                    options.begin = range.begin;
                    options.end = range.end;
                } else {
                    return StatusApps.responseForStatus(request, 416); // not satisfiable
                }
            }
        // Full requests
        } else {
            // Cached
            // We do not use date-based caching
            // TODO consider if-match?
            if (etag == request.headers["if-none-match"])
                return StatusApps.responseForStatus(request, 304);
            headers["content-length"] = "" + stat.size;
        }

        // TODO sendfile
        return {
            status: status,
            headers: headers,
            body: fs.open(path, options),
            file: path,
            range: range
        };
    });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.q-io.http_apps.handleHtmlFragmentResponse"></a>[function <span class="apidocSignatureSpan">q-io.http_apps.</span>handleHtmlFragmentResponse (response)](#apidoc.element.q-io.http_apps.handleHtmlFragmentResponse)
- description and source-code
```javascript
handleHtmlFragmentResponse = function (response) {
    var htmlFragment = response.htmlFragment;
    delete response.htmlFragment;
    response.headers["content-type"] = "text/html; charset=utf-8";
    response.body = {
        forEach: function (write) {
            write("<!doctype html>\n");
            write("<html>\n");
            write("    <head>\n");
            if (response.htmlTitle !== void 0) {
                write("        <title>" + escapeHtml(response.htmlTitle) + "</title>\n");
            }
            write("    </head>\n");
            write("    <body>\n");
            htmlFragment.forEach(function (line) {
                write("        " + line);
            });
            write("    </body>\n");
            write("</html>\n");
        }
    };
    return response;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.q-io.http_apps.handleJsonResponse"></a>[function <span class="apidocSignatureSpan">q-io.http_apps.</span>handleJsonResponse (response, revivier, tab)](#apidoc.element.q-io.http_apps.handleJsonResponse)
- description and source-code
```javascript
handleJsonResponse = function (response, revivier, tab) {
    response.headers["content-type"] = "application/json";
    response.body = {
        forEach: function (write) {
            write(JSON.stringify(response.data, revivier, tab));
        }
    };
    return response;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.q-io.http_apps.htmlResponseForStatus"></a>[function <span class="apidocSignatureSpan">q-io.http_apps.</span>htmlResponseForStatus (request, status, message, addendum)](#apidoc.element.q-io.http_apps.htmlResponseForStatus)
- description and source-code
```javascript
htmlResponseForStatus = function (request, status, message, addendum) {
    return {
        status: status,
        statusMessage: message,
        headers: {},
        htmlTitle: message,
        htmlFragment: {
            forEach: function (write) {
                write("<h1>" + HtmlApps.escapeHtml(message) + "</h1>\n");
                write("<p>Status: " + status + "</p>\n");
                if (addendum) {
                    write("<pre>" + HtmlApps.escapeHtml(addendum) + "</pre>\n");
                }
            }
        }
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.q-io.http_apps.isRedirect"></a>[function <span class="apidocSignatureSpan">q-io.http_apps.</span>isRedirect (response)](#apidoc.element.q-io.http_apps.isRedirect)
- description and source-code
```javascript
isRedirect = function (response) {
    return isRedirect[response.status] || false;
}
```
- example usage
```shell
...

// try redirect loop
function next() {
    Q.fcall(function () {
        return app(request, response);
    })
    .then(function (response) {
        if (exports.isRedirect(response)) {
            if (remaining--) {
                request.url = response.headers.location;
                next();
            } else {
                throw new Error("Maximum redirects.");
            }
        } else {
...
```

#### <a name="apidoc.element.q-io.http_apps.json"></a>[function <span class="apidocSignatureSpan">q-io.http_apps.</span>json (content, reviver, tabs)](#apidoc.element.q-io.http_apps.json)
- description and source-code
```javascript
json = function (content, reviver, tabs) {
    try {
        var json = JSON.stringify(content, reviver, tabs);
    } catch (exception) {
        return Q.reject(exception);
    }
    return Content.ok([json], "application/json");
}
```
- example usage
```shell
...
* @param {Function(Request):Object} app an application that accepts a
* request and returns a JSON serializable object.
* @returns {App}
*/
exports.Json = function (app, reviver, tabs) {
   return function (request, response) {
       return Q.when(app(request, response), function (object) {
           return exports.json(object, reviver, tabs);
       });
   };
};

/**
* @param {Object} content data to serialize as JSON
* @param {Function} reviver
...
```

#### <a name="apidoc.element.q-io.http_apps.listDirectory"></a>[function <span class="apidocSignatureSpan">q-io.http_apps.</span>listDirectory (request, response)](#apidoc.element.q-io.http_apps.listDirectory)
- description and source-code
```javascript
listDirectory = function (request, response) {
    // TODO advisory to have JSON or HTML fragment handler.
    request.location = URL.parse(request.path);
    if (request.location.file) {
        return RedirectApps.redirect(request, request.location.file + "/");
    }
    var handlers = {};
    handlers["text/plain"] = exports.listDirectoryText;
    handlers["text/markdown"] = exports.listDirectoryMarkdown;
    if (request.handleHtmlFragmentResponse) {
        handlers["text/html"] = exports.listDirectoryHtmlFragment;
    }
    if (request.handleJsonResponse) {
        handlers["application/json"] = exports.listDirectoryJson;
    }
    var handleResponse = Negotiation.negotiate(request, handlers) || function () {
        return response;
    };
    return handleResponse(request, response);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.q-io.http_apps.listDirectoryData"></a>[function <span class="apidocSignatureSpan">q-io.http_apps.</span>listDirectoryData (request, response)](#apidoc.element.q-io.http_apps.listDirectoryData)
- description and source-code
```javascript
listDirectoryData = function (request, response) {
    if (!request.fs) {
        throw new Error("Can't list a directory without a designated file system");
    }
    var fs = request.fs;
    return Q.invoke(fs, "list", response.directory)
    .then(function (list) {
        list.sort();
        return list.map(function (name) {
            return Q.invoke(fs, "stat", fs.join(response.directory, name))
            .then(function (stat) {
                if (stat.isDirectory()) {
                    return {name: name, stat: {
                        type: "directory"
                    }};
                } else if (stat.isFile()) {
                    return {name: name, stat: {
                        type: "file"
                    }};
                }
            }, function () {
                // ignore unstatable entries
            });
        })
    })
    .all()
    .then(function (stats) {
        var data = {};
        stats.forEach(function (entry) {
            if (entry) {
                data[entry.name] = entry.stat;
            }
        });
        return data;
    });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.q-io.http_apps.listDirectoryHtmlFragment"></a>[function <span class="apidocSignatureSpan">q-io.http_apps.</span>listDirectoryHtmlFragment (request, response)](#apidoc.element.q-io.http_apps.listDirectoryHtmlFragment)
- description and source-code
```javascript
listDirectoryHtmlFragment = function (request, response) {
    return exports.listDirectoryData(request, response)
    .then(function (data) {
        return {
            status: 200,
            headers: {
                "content-type": "text/html"
            },
            htmlTitle: "Directory Index",
            htmlFragment: {
                forEach: function (write) {
                    write("<ul class=\"directory-index\">\n");
                    Object.keys(data).sort().forEach(function (name) {
                        var stat = data[name];
                        var suffix = "";
                        if (stat.type === "directory") {
                            suffix = "/";
                        }
                        write("    <li class=\"entry " + stat.type + "\"><a href=\"" + HtmlApps.escapeHtml(name + suffix) + "\">" +
HtmlApps.escapeHtml(name + suffix) + "</a></li>\n");
                    });
                    write("</ul>\n");
                }
            }
        };
    });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.q-io.http_apps.listDirectoryJson"></a>[function <span class="apidocSignatureSpan">q-io.http_apps.</span>listDirectoryJson (request, response)](#apidoc.element.q-io.http_apps.listDirectoryJson)
- description and source-code
```javascript
listDirectoryJson = function (request, response) {
    return exports.listDirectoryData(request, response)
    .then(function (data) {
        return {
            status: 200,
            headers: {},
            data: data
        };
    });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.q-io.http_apps.listDirectoryMarkdown"></a>[function <span class="apidocSignatureSpan">q-io.http_apps.</span>listDirectoryMarkdown (request, response)](#apidoc.element.q-io.http_apps.listDirectoryMarkdown)
- description and source-code
```javascript
listDirectoryMarkdown = function (request, response) {
    return exports.listDirectoryData(request, response)
    .then(function (data) {
        return {
            status: 200,
            headers: {
                "content-type": "text/plain"
            },
            body: {
                forEach: function (write) {
                    write("\n# Directory Index\n\n");
                    Object.keys(data).forEach(function (name) {
                        var stat = data[name];
                        var suffix = "";
                        if (stat.type === "directory") {
                            suffix = "/";
                        }
                        write("-   " + name + suffix + "\n");
                    });
                    write("\n");
                }
            }
        };
    });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.q-io.http_apps.listDirectoryText"></a>[function <span class="apidocSignatureSpan">q-io.http_apps.</span>listDirectoryText (request, response)](#apidoc.element.q-io.http_apps.listDirectoryText)
- description and source-code
```javascript
listDirectoryText = function (request, response) {
    return exports.listDirectoryData(request, response)
    .then(function (data) {
        return {
            status: 200,
            headers: {
                "content-type": "text/plain"
            },
            body: {
                forEach: function (write) {
                    Object.keys(data).sort().forEach(function (name) {
                        var stat = data[name];
                        var suffix = "";
                        if (stat.type === "directory") {
                            suffix = "/";
                        }
                        write(name + suffix + "\n");
                    });
                }
            }
        };
    });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.q-io.http_apps.methodNotAllowed"></a>[function <span class="apidocSignatureSpan">q-io.http_apps.</span>methodNotAllowed (request)](#apidoc.element.q-io.http_apps.methodNotAllowed)
- description and source-code
```javascript
methodNotAllowed = function (request) {
    return exports.responseForStatus(request, status, request.method + " " + request.path);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.q-io.http_apps.negotiate"></a>[function <span class="apidocSignatureSpan">q-io.http_apps.</span>negotiate (request, types, header)](#apidoc.element.q-io.http_apps.negotiate)
- description and source-code
```javascript
function negotiate(request, types, header) {
    var keys = Object.keys(types);
    var accept = request.headers[header || "accept"] || "*";
    var best = MimeParse.bestMatch(keys, accept);
    return types[best];
}
```
- example usage
```shell
...
}

var handlers = {};
handlers["text/plain"] = exports.redirectText;
if (request.handleHtmlFragmentResponse) {
    handlers["text/html"] = exports.redirectHtml;
}
var handler = Negotiation.negotiate(request, handlers) || exports.redirectText;
return handler(request, location, status);

};

exports.redirectText = function (request, location, status) {
var content = (
    (request.permanent ? "Permanent redirect\n" : "Temporary redirect\n") +
...
```

#### <a name="apidoc.element.q-io.http_apps.noLanguage"></a>[function <span class="apidocSignatureSpan">q-io.http_apps.</span>noLanguage (request)](#apidoc.element.q-io.http_apps.noLanguage)
- description and source-code
```javascript
noLanguage = function (request) {
    return exports.responseForStatus(request, status, request.method + " " + request.path);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.q-io.http_apps.notAcceptable"></a>[function <span class="apidocSignatureSpan">q-io.http_apps.</span>notAcceptable (request)](#apidoc.element.q-io.http_apps.notAcceptable)
- description and source-code
```javascript
notAcceptable = function (request) {
    return exports.responseForStatus(request, status, request.method + " " + request.path);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.q-io.http_apps.notFound"></a>[function <span class="apidocSignatureSpan">q-io.http_apps.</span>notFound (request)](#apidoc.element.q-io.http_apps.notFound)
- description and source-code
```javascript
notFound = function (request) {
    return exports.responseForStatus(request, status, request.method + " " + request.path);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.q-io.http_apps.ok"></a>[function <span class="apidocSignatureSpan">q-io.http_apps.</span>ok (content, contentType, status)](#apidoc.element.q-io.http_apps.ok)
- description and source-code
```javascript
ok = function (content, contentType, status) {
    status = status || 200;
    content = content || "";
    if (typeof content === "string") {
        content = [content];
    }
    contentType = contentType || "text/plain";
    return {
        "status": status,
        "headers": {
            "content-type": contentType
        },
        "body": content
    };
}
```
- example usage
```shell
...
*/
exports.json = function (content, reviver, tabs) {
   try {
       var json = JSON.stringify(content, reviver, tabs);
   } catch (exception) {
       return Q.reject(exception);
   }
   return Content.ok([json], "application/json");
};

/**
* @param {Function(Request, Object):Response} app
* @param {App} badRequest
* @returns {App}
*/
...
```

#### <a name="apidoc.element.q-io.http_apps.permanentRedirect"></a>[function <span class="apidocSignatureSpan">q-io.http_apps.</span>permanentRedirect (request, location, status)](#apidoc.element.q-io.http_apps.permanentRedirect)
- description and source-code
```javascript
permanentRedirect = function (request, location, status) {
    return exports.redirect(request, location, status || 301);
}
```
- example usage
```shell
...
/**
* @param {String} path
* @param {Number} status (optional) default is '301'
* @returns {App}
*/
exports.PermanentRedirect = function (location, status, tree) {
   return function (request, response) {
       return exports.permanentRedirect(request, location, status, tree);
   };
};

/**
* @param {String} path
* @param {Number} status (optional) default is '301'
* @returns {App}
...
```

#### <a name="apidoc.element.q-io.http_apps.permanentRedirectTree"></a>[function <span class="apidocSignatureSpan">q-io.http_apps.</span>permanentRedirectTree (request, location, status)](#apidoc.element.q-io.http_apps.permanentRedirectTree)
- description and source-code
```javascript
permanentRedirectTree = function (request, location, status) {
    return exports.redirect(request, location, status || 301, true);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.q-io.http_apps.redirect"></a>[function <span class="apidocSignatureSpan">q-io.http_apps.</span>redirect (request, location, status, tree)](#apidoc.element.q-io.http_apps.redirect)
- description and source-code
```javascript
redirect = function (request, location, status, tree) {

    // request.permanent gets set by Permanent middleware
    status = status || (request.permanent ? 301 : 307);

    // ascertain that the location is absolute, per spec
    location = URL.resolve(request.url, location);

    // redirect into a subtree with the remaining unrouted
    // portion of the path, if so configured
    if (tree) {
        location = URL.resolve(
            location,
            request.pathInfo.replace(/^\//, "")
        );
    }

    var handlers = {};
    handlers["text/plain"] = exports.redirectText;
    if (request.handleHtmlFragmentResponse) {
        handlers["text/html"] = exports.redirectHtml;
    }
    var handler = Negotiation.negotiate(request, handlers) || exports.redirectText;
    return handler(request, location, status);

}
```
- example usage
```shell
...
/**
* @param {String} path
* @param {Number} status (optional) default is '307'
* @returns {App}
*/
exports.Redirect = function (location, status, tree) {
   return function (request, response) {
       return exports.redirect(request, location, status, tree);
   };
};

/**
* @param {String} path
* @param {Number} status (optional) default is '307'
* @returns {App}
...
```

#### <a name="apidoc.element.q-io.http_apps.redirectHtml"></a>[function <span class="apidocSignatureSpan">q-io.http_apps.</span>redirectHtml (request, location, status)](#apidoc.element.q-io.http_apps.redirectHtml)
- description and source-code
```javascript
redirectHtml = function (request, location, status) {
    var title = request.permanent ? "Permanent redirect" : "Temporary redirect";
    return {
        status: status,
        headers: {
            location: location,
            "content-type": "text/html"
        },
        htmlTitle: title,
        htmlFragment: {
            forEach: function (write) {
                write("<h1>" + HtmlApps.escapeHtml(title) + "</h1>\n");
                write(
                    "<p>See: <a href=\"" + HtmlApps.escapeHtml(location) + "\">" +
                    HtmlApps.escapeHtml(location) +
                    "</a></p>\n"
                );
            }
        }
    };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.q-io.http_apps.redirectText"></a>[function <span class="apidocSignatureSpan">q-io.http_apps.</span>redirectText (request, location, status)](#apidoc.element.q-io.http_apps.redirectText)
- description and source-code
```javascript
redirectText = function (request, location, status) {
    var content = (
        (request.permanent ? "Permanent redirect\n" : "Temporary redirect\n") +
        "See: " + location + "\n"
    );
    var contentLength = content.length;
    return {
        status: status,
        headers: {
            location: location,
            "content-type": "text/plain"
        },
        body: [content]
    };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.q-io.http_apps.redirectTree"></a>[function <span class="apidocSignatureSpan">q-io.http_apps.</span>redirectTree (request, location, status)](#apidoc.element.q-io.http_apps.redirectTree)
- description and source-code
```javascript
redirectTree = function (request, location, status) {
    return exports.redirect(request, location, status, true);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.q-io.http_apps.responseForStatus"></a>[function <span class="apidocSignatureSpan">q-io.http_apps.</span>responseForStatus (request, status, addendum)](#apidoc.element.q-io.http_apps.responseForStatus)
- description and source-code
```javascript
responseForStatus = function (request, status, addendum) {
    if (exports.statusCodes[status] === undefined)
        throw "Unknown status code";

    var message = exports.statusCodes[status];

    // RFC 2616, 10.2.5:
    // The 204 response MUST NOT include a message-body, and thus is always
    // terminated by the first empty line after the header fields.
    // RFC 2616, 10.3.5:
    // The 304 response MUST NOT contain a message-body, and thus is always
    // terminated by the first empty line after the header fields.
    if (exports.statusWithNoEntityBody(status)) {
        return {status: status, headers: {}};
    } else {
        var handlers = {};
        handlers["text/plain"] = exports.textResponseForStatus;
        if (request.handleHtmlFragmentResponse) {
            handlers["text/html"] = exports.htmlResponseForStatus;
        }
        var responseForStatus = Negotiation.negotiate(request, handlers) || exports.textResponseForStatus;
        return responseForStatus(request, status, message, addendum);
    }
}
```
- example usage
```shell
...
 * @returns {App}
 */
exports.Error = function (app, debug) {
    return function (request, response) {
        return Q.when(app(request, response), null, function (error) {
            if (!debug)
                error = undefined;
            return StatusApps.responseForStatus(request, 500, error && error.stack || error);
        });
    };
};

exports.Debug = function (app) {
    return exports.Error(app, true);
};
...
```

#### <a name="apidoc.element.q-io.http_apps.statusWithNoEntityBody"></a>[function <span class="apidocSignatureSpan">q-io.http_apps.</span>statusWithNoEntityBody (status)](#apidoc.element.q-io.http_apps.statusWithNoEntityBody)
- description and source-code
```javascript
statusWithNoEntityBody = function (status) {
    return (status >= 100 && status <= 199) ||
        status == 204 || status == 304;
}
```
- example usage
```shell
...

// RFC 2616, 10.2.5:
// The 204 response MUST NOT include a message-body, and thus is always
// terminated by the first empty line after the header fields.
// RFC 2616, 10.3.5:
// The 304 response MUST NOT contain a message-body, and thus is always
// terminated by the first empty line after the header fields.
if (exports.statusWithNoEntityBody(status)) {
    return {status: status, headers: {}};
} else {
    var handlers = {};
    handlers["text/plain"] = exports.textResponseForStatus;
    if (request.handleHtmlFragmentResponse) {
        handlers["text/html"] = exports.htmlResponseForStatus;
    }
...
```

#### <a name="apidoc.element.q-io.http_apps.temporaryRedirect"></a>[function <span class="apidocSignatureSpan">q-io.http_apps.</span>temporaryRedirect (request, location, status)](#apidoc.element.q-io.http_apps.temporaryRedirect)
- description and source-code
```javascript
temporaryRedirect = function (request, location, status) {
    return exports.redirect(request, location, status || 307);
}
```
- example usage
```shell
...
/**
* @param {String} path
* @param {Number} status (optional) default is '307'
* @returns {App}
*/
exports.TemporaryRedirect = function (location, status, tree) {
   return function (request, response) {
       return exports.temporaryRedirect(request, location, status, tree);
   };
};

/**
* @param {String} path
* @param {Number} status (optional) default is '307'
* @returns {App}
...
```

#### <a name="apidoc.element.q-io.http_apps.temporaryRedirectTree"></a>[function <span class="apidocSignatureSpan">q-io.http_apps.</span>temporaryRedirectTree (request, location, status)](#apidoc.element.q-io.http_apps.temporaryRedirectTree)
- description and source-code
```javascript
temporaryRedirectTree = function (request, location, status) {
    return exports.redirect(request, location, status || 307, true);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.q-io.http_apps.textResponseForStatus"></a>[function <span class="apidocSignatureSpan">q-io.http_apps.</span>textResponseForStatus (request, status, message, addendum)](#apidoc.element.q-io.http_apps.textResponseForStatus)
- description and source-code
```javascript
textResponseForStatus = function (request, status, message, addendum) {
    var content = message + "\n";
    if (addendum) {
        content += addendum + "\n";
    }
    var contentLength = content.length;
    return {
        status: status,
        statusMessage: message,
        headers: {
            "content-length": contentLength
        },
        body: [content]
    };
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.q-io.http_cookie"></a>[module q-io.http_cookie](#apidoc.module.q-io.http_cookie)

#### <a name="apidoc.element.q-io.http_cookie.parse"></a>[function <span class="apidocSignatureSpan">q-io.http_cookie.</span>parse (cookie, date)](#apidoc.element.q-io.http_cookie.parse)
- description and source-code
```javascript
parse = function (cookie, date) {
    date = date || new Date();
    var parsed = {};
    var terms = cookie.split(/[;,]/g);
    var keyValue = terms.shift().split("=");
    parsed.key = decodeURIComponent(keyValue[0]);
    parsed.value = decodeURIComponent(keyValue[1]);
    terms.forEach(function (term) {
        var parts = term.split("=").map(function (part) {
            return part.trim();
        });
        var key = parts[0], value = parts[1];
        if (/^domain$/i.test(key)) {
            parsed.domain = value;
        } else if (/^path$/i.test(key)) {
            parsed.path = value;
        } else if (/^expires$/i.test(key)) {
            parsed.expires = new Date(
                +new Date() + // actual now
                (new Date(value) - date) // server offset
            );
        } else if (/^max-age$/i.test(key)) {
            parsed.expires = new Date(
                new Date().getTime() +
                (value * 1000)
            );
        } else if (/^secure$/i.test(key)) {
            parsed.secure = true;
        } else if (/^httponly$/i.test(key)) {
            parsed.httpOnly = true;
        }
    });
    return parsed;
}
```
- example usage
```shell
...
FS.listTree(".coverage_data", function (name, stat) {
return (/^\.coverage_data\/coveragefile/).test(name);
})
.then(function (list) {
return Q.all(list.map(function (file) {
    return FS.read(file)
    .then(function (content) {
        return JSON.parse(content);
    })
    .then(function (coverage) {
        console.log("<table>");
        console.log("    <thead>");
        console.log("        <tr>");
        console.log("            <th>File</th>");
        console.log("            <th>Percentage</th>");
...
```

#### <a name="apidoc.element.q-io.http_cookie.stringify"></a>[function <span class="apidocSignatureSpan">q-io.http_cookie.</span>stringify (key, value, options)](#apidoc.element.q-io.http_cookie.stringify)
- description and source-code
```javascript
stringify = function (key, value, options) {
    var cookie = (
        encodeURIComponent(key) + "=" +
        encodeURIComponent(value)
    );
    if (options) {
        if (options.domain)
            cookie += "; Domain=" + encodeURIComponent(options.domain);
        if (options.path)
            cookie += "; Path=" + encodeURIComponent(options.path);
        if (options.expires)
            cookie += "; Expires=" + options.expires.toGMTString();
        if (options.secure)
            cookie += "; Secure";
        if (options.httpOnly)
            cookie += "; HttpOnly";
    }
    return cookie;
}
```
- example usage
```shell
...
 * @returns {Array * String}
 */
exports.split = function (path) {
var parts;
try {
    parts = String(path).split(exports.SEPARATORS_RE());
} catch (exception) {
    throw new Error("Cannot split " + (typeof path) + ", " + JSON.stringify(path));
}
// this special case helps isAbsolute
// distinguish an empty path from an absolute path
// "" -> [] NOT [""]
if (parts.length === 1 && parts[0] === "")
    return [];
// "a" -> ["a"]
...
```



# <a name="apidoc.module.q-io.json"></a>[module q-io.json](#apidoc.module.q-io.json)

#### <a name="apidoc.element.q-io.json.json"></a>[function <span class="apidocSignatureSpan">q-io.</span>json (content, reviver, tabs)](#apidoc.element.q-io.json.json)
- description and source-code
```javascript
json = function (content, reviver, tabs) {
    try {
        var json = JSON.stringify(content, reviver, tabs);
    } catch (exception) {
        return Q.reject(exception);
    }
    return Content.ok([json], "application/json");
}
```
- example usage
```shell
...
* @param {Function(Request):Object} app an application that accepts a
* request and returns a JSON serializable object.
* @returns {App}
*/
exports.Json = function (app, reviver, tabs) {
   return function (request, response) {
       return Q.when(app(request, response), function (object) {
           return exports.json(object, reviver, tabs);
       });
   };
};

/**
* @param {Object} content data to serialize as JSON
* @param {Function} reviver
...
```

#### <a name="apidoc.element.q-io.json.HandleJsonResponses"></a>[function <span class="apidocSignatureSpan">q-io.json.</span>HandleJsonResponses (app, reviver, tab)](#apidoc.element.q-io.json.HandleJsonResponses)
- description and source-code
```javascript
HandleJsonResponses = function (app, reviver, tab) {
    return function (request) {
        request.handleJsonResponse = exports.handleJsonResponse;
        return Q.fcall(app, request)
        .then(function (response) {
            if (response.data !== void 0) {
                return Q.fcall(exports.handleJsonResponse, response, reviver, tab);
            } else {
                return response;
            }
        });
    };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.q-io.json.Json"></a>[function <span class="apidocSignatureSpan">q-io.json.</span>Json (app, reviver, tabs)](#apidoc.element.q-io.json.Json)
- description and source-code
```javascript
Json = function (app, reviver, tabs) {
    return function (request, response) {
        return Q.when(app(request, response), function (object) {
            return exports.json(object, reviver, tabs);
        });
    };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.q-io.json.JsonRequest"></a>[function <span class="apidocSignatureSpan">q-io.json.</span>JsonRequest (app, badRequest)](#apidoc.element.q-io.json.JsonRequest)
- description and source-code
```javascript
JsonRequest = function (app, badRequest) {
    if (!badRequest)
        badRequest = Status.badRequest;
    return Content.ContentRequest(function (content, request, response) {
        try {
            var object = JSON.parse(content);
        } catch (error) {
            return badRequest(request, error);
        }
        return app(object, request, response);
    });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.q-io.json.handleJsonResponse"></a>[function <span class="apidocSignatureSpan">q-io.json.</span>handleJsonResponse (response, revivier, tab)](#apidoc.element.q-io.json.handleJsonResponse)
- description and source-code
```javascript
handleJsonResponse = function (response, revivier, tab) {
    response.headers["content-type"] = "application/json";
    response.body = {
        forEach: function (write) {
            write(JSON.stringify(response.data, revivier, tab));
        }
    };
    return response;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.q-io.negotiate"></a>[module q-io.negotiate](#apidoc.module.q-io.negotiate)

#### <a name="apidoc.element.q-io.negotiate.negotiate"></a>[function <span class="apidocSignatureSpan">q-io.</span>negotiate (request, types, header)](#apidoc.element.q-io.negotiate.negotiate)
- description and source-code
```javascript
function negotiate(request, types, header) {
    var keys = Object.keys(types);
    var accept = request.headers[header || "accept"] || "*";
    var best = MimeParse.bestMatch(keys, accept);
    return types[best];
}
```
- example usage
```shell
...
}

var handlers = {};
handlers["text/plain"] = exports.redirectText;
if (request.handleHtmlFragmentResponse) {
    handlers["text/html"] = exports.redirectHtml;
}
var handler = Negotiation.negotiate(request, handlers) || exports.redirectText;
return handler(request, location, status);

};

exports.redirectText = function (request, location, status) {
var content = (
    (request.permanent ? "Permanent redirect\n" : "Temporary redirect\n") +
...
```

#### <a name="apidoc.element.q-io.negotiate.Charset"></a>[function <span class="apidocSignatureSpan">q-io.negotiate.</span>Charset (types, notAcceptable)](#apidoc.element.q-io.negotiate.Charset)
- description and source-code
```javascript
Charset = function (types, notAcceptable) {
    var keys = Object.keys(types);
    if (!notAcceptable)
        notAcceptable = Status.notAcceptable;
    return function (request) {
        var accept = request.headers[requestHeader] || "*";
        var type = MimeParse.bestMatch(keys, accept);
        request.terms = request.terms || {};
        request.terms[responseHeader] = type;
        if (Object.has(keys, type)) {
            return Q.when(types[type](request), function (response) {
                if (
                    respond !== null &&
                    response &&
                    response.status === 200 &&
                    response.headers
                ) {
                    response.headers[responseHeader] = type;
                }
                return response;
            });
        } else {
            return notAcceptable(request);
        }
    };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.q-io.negotiate.ContentType"></a>[function <span class="apidocSignatureSpan">q-io.negotiate.</span>ContentType (types, notAcceptable)](#apidoc.element.q-io.negotiate.ContentType)
- description and source-code
```javascript
ContentType = function (types, notAcceptable) {
    var keys = Object.keys(types);
    if (!notAcceptable)
        notAcceptable = Status.notAcceptable;
    return function (request) {
        var accept = request.headers[requestHeader] || "*";
        var type = MimeParse.bestMatch(keys, accept);
        request.terms = request.terms || {};
        request.terms[responseHeader] = type;
        if (Object.has(keys, type)) {
            return Q.when(types[type](request), function (response) {
                if (
                    respond !== null &&
                    response &&
                    response.status === 200 &&
                    response.headers
                ) {
                    response.headers[responseHeader] = type;
                }
                return response;
            });
        } else {
            return notAcceptable(request);
        }
    };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.q-io.negotiate.Encoding"></a>[function <span class="apidocSignatureSpan">q-io.negotiate.</span>Encoding (types, notAcceptable)](#apidoc.element.q-io.negotiate.Encoding)
- description and source-code
```javascript
Encoding = function (types, notAcceptable) {
    var keys = Object.keys(types);
    if (!notAcceptable)
        notAcceptable = Status.notAcceptable;
    return function (request) {
        var accept = request.headers[requestHeader] || "*";
        var type = MimeParse.bestMatch(keys, accept);
        request.terms = request.terms || {};
        request.terms[responseHeader] = type;
        if (Object.has(keys, type)) {
            return Q.when(types[type](request), function (response) {
                if (
                    respond !== null &&
                    response &&
                    response.status === 200 &&
                    response.headers
                ) {
                    response.headers[responseHeader] = type;
                }
                return response;
            });
        } else {
            return notAcceptable(request);
        }
    };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.q-io.negotiate.Host"></a>[function <span class="apidocSignatureSpan">q-io.negotiate.</span>Host (appForHost, notAcceptable)](#apidoc.element.q-io.negotiate.Host)
- description and source-code
```javascript
Host = function (appForHost, notAcceptable) {
    var table = Object.keys(appForHost).map(function (pattern) {
        var parts = pattern.split(":");
        return [
            pattern,
            parts[0] || "*",
            parts[1] || "*",
            appForHost[pattern]
        ];
    });
    if (!notAcceptable) {
        notAcceptable = Status.notAcceptable;
    }
    return function (request) {
        // find first matching host for app
        for (var index = 0; index < table.length; index++) {
            var row = table[index]; // [hostname, port, app]
            var pattern = row[0];
            var hostname = row[1];
            var port = row[2];
            var app = row[3];
            if (
                (hostname === "*" || hostname === request.hostname) &&
                (port === "*" || port === "" + request.port)
            ) {
                request.terms = request.terms || {};
                request.terms.host = pattern;
                return app(request);
            }
        }
        return notAcceptable(request);
    };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.q-io.negotiate.Language"></a>[function <span class="apidocSignatureSpan">q-io.negotiate.</span>Language (types, notAcceptable)](#apidoc.element.q-io.negotiate.Language)
- description and source-code
```javascript
Language = function (types, notAcceptable) {
    var keys = Object.keys(types);
    if (!notAcceptable)
        notAcceptable = Status.notAcceptable;
    return function (request) {
        var accept = request.headers[requestHeader] || "*";
        var type = MimeParse.bestMatch(keys, accept);
        request.terms = request.terms || {};
        request.terms[responseHeader] = type;
        if (Object.has(keys, type)) {
            return Q.when(types[type](request), function (response) {
                if (
                    respond !== null &&
                    response &&
                    response.status === 200 &&
                    response.headers
                ) {
                    response.headers[responseHeader] = type;
                }
                return response;
            });
        } else {
            return notAcceptable(request);
        }
    };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.q-io.negotiate.Method"></a>[function <span class="apidocSignatureSpan">q-io.negotiate.</span>Method (methods, methodNotAllowed)](#apidoc.element.q-io.negotiate.Method)
- description and source-code
```javascript
Method = function (methods, methodNotAllowed) {
    var keys = Object.keys(methods);
    if (!methodNotAllowed)
        methodNotAllowed = Status.methodNotAllowed;
    return function (request) {
        var method = request.method;
        if (Object.has(keys, method)) {
            return Object.get(methods, method)(request);
        } else {
            return methodNotAllowed(request);
        }
    };
}
```
- example usage
```shell
...
};

/**
 * @param {Function(Request):Object}
 * @returns {App}
 */
exports.Inspect = function (app) {
return Negotiate.Method({"GET": function (request, response) {
    return Q.when(app(request, response), function (object) {
        return {
            status: 200,
            headers: {
                "content-type": "text/plain"
            },
            body: [inspect(object)]
...
```

#### <a name="apidoc.element.q-io.negotiate.Select"></a>[function <span class="apidocSignatureSpan">q-io.negotiate.</span>Select (select)](#apidoc.element.q-io.negotiate.Select)
- description and source-code
```javascript
Select = function (select) {
    return function (request) {
        return Q.when(select(request), function (app) {
            return app(request);
        });
    };
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.q-io.proxy"></a>[module q-io.proxy](#apidoc.module.q-io.proxy)

#### <a name="apidoc.element.q-io.proxy.Proxy"></a>[function <span class="apidocSignatureSpan">q-io.proxy.</span>Proxy (app)](#apidoc.element.q-io.proxy.Proxy)
- description and source-code
```javascript
Proxy = function (app) {
    if (typeof app === "string") {
        var location = app;
        app = function (request) {
            request.url = location;
            return request;
        };
    }
    return function (request, response) {
        return Q.when(app.apply(this, arguments), function (request) {
            return HTTP.request(request);
        });
    };
}
```
- example usage
```shell
...
        return Q.when(app.apply(this, arguments), function (request) {
            return HTTP.request(request);
        });
    };
};

exports.ProxyTree = function (url) {
    return exports.Proxy(function (request) {
        request.url = URL.resolve(url, request.pathInfo.replace(/^\//, ""));
        return request;
    });
};
...
```

#### <a name="apidoc.element.q-io.proxy.ProxyTree"></a>[function <span class="apidocSignatureSpan">q-io.proxy.</span>ProxyTree (url)](#apidoc.element.q-io.proxy.ProxyTree)
- description and source-code
```javascript
ProxyTree = function (url) {
    return exports.Proxy(function (request) {
        request.url = URL.resolve(url, request.pathInfo.replace(/^\//, ""));
        return request;
    });
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.q-io.reader"></a>[module q-io.reader](#apidoc.module.q-io.reader)

#### <a name="apidoc.element.q-io.reader.reader"></a>[function <span class="apidocSignatureSpan">q-io.</span>reader (_stream, charset)](#apidoc.element.q-io.reader.reader)
- description and source-code
```javascript
function Reader(_stream, charset) {
    var self = Object.create(Reader.prototype);

    if (charset && _stream.setEncoding) // TODO complain about inconsistency
        _stream.setEncoding(charset);

    var begin = Q.defer();
    var end = Q.defer();

    _stream.on("error", function (reason) {
        begin.reject(reason);
    });

    var chunks = [];
    var receiver;

    _stream.on("end", function () {
        begin.resolve(self);
        end.resolve()
    });

    _stream.on("data", function (chunk) {
        begin.resolve(self);
        if (receiver) {
            receiver(chunk);
        } else {
            chunks.push(chunk);
        }
    });

    function slurp() {
        var result;
        if (charset) {
            result = chunks.join("");
        } else {
            result = self.constructor.join(chunks);
        }
        chunks.splice(0, chunks.length);
        return result;
    }

<span class="apidocCodeCommentSpan">    /***
     * Reads all of the remaining data from the stream.
     * @returns {Promise * String} a promise for a String
     * containing the entirety the remaining stream.
     */
</span>    self.read = function () {
        receiver = undefined;
        var deferred = Q.defer();
        Q.done(end.promise, function () {
            deferred.resolve(slurp());
        });
        return deferred.promise;
    };

    /***
     * Reads and writes all of the remaining data from the
     * stream in chunks.
     * @param {Function(Promise * String)} write a function
     * to be called on each chunk of input from this stream.
     * @returns {Promise * Undefined} a promise that will
     * be resolved when the input is depleted.
     */
    self.forEach = function (write) {
        if (chunks && chunks.length)
            write(slurp());
        receiver = write;
        return Q.when(end.promise, function () {
            receiver = undefined;
        });
    };

    self.close = function () {
        _stream.destroy();
    };

    self.node = _stream;

    return begin.promise;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.q-io.reader.join"></a>[function <span class="apidocSignatureSpan">q-io.reader.</span>join (buffers)](#apidoc.element.q-io.reader.join)
- description and source-code
```javascript
function join(buffers) {
    var length = 0;
    var at;
    var i;
    var ii = buffers.length;
    var buffer;
    var result;
    for (i = 0; i < ii; i++) {
        buffer = buffers[i];
        length += buffer.length;
    }
    result = new Buffer(length);
    at = 0;
    for (i = 0; i < ii; i++) {
        buffer = buffers[i];
        buffer.copy(result, at, 0);
        at += buffer.length;
    }
    buffers.splice(0, ii, result);
    return result;
}
```
- example usage
```shell
...
    return Q.fcall(function () {
        chunks.splice(0, chunks.length).forEach(write, thisp);
    });
};

BufferStream.prototype.read = function () {
    var result;
    result = Reader.join(this._chunks);
    if (this._charset) {
        result = result.toString(this._charset);
    }
    return Q.resolve(result);
};

BufferStream.prototype.write = function (chunk) {
...
```

#### <a name="apidoc.element.q-io.reader.read"></a>[function <span class="apidocSignatureSpan">q-io.reader.</span>read (stream, charset)](#apidoc.element.q-io.reader.read)
- description and source-code
```javascript
function read(stream, charset) {
    var chunks = [];
    stream.forEach(function (chunk) {
        chunks.push(chunk);
    });
    if (charset) {
        return chunks.join("");
    } else {
        return join(chunks);
    }
}
```
- example usage
```shell
...
into memory.  It returns a promise for the whole file contents.  By
default, 'read' provides a string decoded from UTF-8.  With the bytewise
mode flag, provides a 'Buffer'.

The options argument is identical to that of 'open'.

'''javascript
return FS.read(__filename, "b")
.then(function (content) {
    // ...
})
'''

'''javascript
return FS.read(__filename, {
...
```



# <a name="apidoc.module.q-io.redirect"></a>[module q-io.redirect](#apidoc.module.q-io.redirect)

#### <a name="apidoc.element.q-io.redirect.redirect"></a>[function <span class="apidocSignatureSpan">q-io.</span>redirect (request, location, status, tree)](#apidoc.element.q-io.redirect.redirect)
- description and source-code
```javascript
redirect = function (request, location, status, tree) {

    // request.permanent gets set by Permanent middleware
    status = status || (request.permanent ? 301 : 307);

    // ascertain that the location is absolute, per spec
    location = URL.resolve(request.url, location);

    // redirect into a subtree with the remaining unrouted
    // portion of the path, if so configured
    if (tree) {
        location = URL.resolve(
            location,
            request.pathInfo.replace(/^\//, "")
        );
    }

    var handlers = {};
    handlers["text/plain"] = exports.redirectText;
    if (request.handleHtmlFragmentResponse) {
        handlers["text/html"] = exports.redirectHtml;
    }
    var handler = Negotiation.negotiate(request, handlers) || exports.redirectText;
    return handler(request, location, status);

}
```
- example usage
```shell
...
/**
* @param {String} path
* @param {Number} status (optional) default is '307'
* @returns {App}
*/
exports.Redirect = function (location, status, tree) {
   return function (request, response) {
       return exports.redirect(request, location, status, tree);
   };
};

/**
* @param {String} path
* @param {Number} status (optional) default is '307'
* @returns {App}
...
```

#### <a name="apidoc.element.q-io.redirect.PermanentRedirect"></a>[function <span class="apidocSignatureSpan">q-io.redirect.</span>PermanentRedirect (location, status, tree)](#apidoc.element.q-io.redirect.PermanentRedirect)
- description and source-code
```javascript
PermanentRedirect = function (location, status, tree) {
    return function (request, response) {
        return exports.permanentRedirect(request, location, status, tree);
    };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.q-io.redirect.PermanentRedirectTree"></a>[function <span class="apidocSignatureSpan">q-io.redirect.</span>PermanentRedirectTree (location, status)](#apidoc.element.q-io.redirect.PermanentRedirectTree)
- description and source-code
```javascript
PermanentRedirectTree = function (location, status) {
    return function (request, response) {
        return exports.permanentRedirect(request, location, status, true);
    };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.q-io.redirect.Redirect"></a>[function <span class="apidocSignatureSpan">q-io.redirect.</span>Redirect (location, status, tree)](#apidoc.element.q-io.redirect.Redirect)
- description and source-code
```javascript
Redirect = function (location, status, tree) {
    return function (request, response) {
        return exports.redirect(request, location, status, tree);
    };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.q-io.redirect.RedirectTrap"></a>[function <span class="apidocSignatureSpan">q-io.redirect.</span>RedirectTrap (app, maxRedirects)](#apidoc.element.q-io.redirect.RedirectTrap)
- description and source-code
```javascript
RedirectTrap = function (app, maxRedirects) {
    maxRedirects = maxRedirects || 20;
    return function (request, response) {
        var remaining = maxRedirects;
        var deferred = Q.defer();
        var self = this;
        var args = arguments;

        request = Http.normalizeRequest(request);

        // try redirect loop
        function next() {
            Q.fcall(function () {
                return app(request, response);
            })
            .then(function (response) {
                if (exports.isRedirect(response)) {
                    if (remaining--) {
                        request.url = response.headers.location;
                        next();
                    } else {
                        throw new Error("Maximum redirects.");
                    }
                } else {
                    deferred.resolve(response);
                }
            })
            .fail(deferred.reject)
        }
        next();

        return deferred.promise;
    };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.q-io.redirect.RedirectTree"></a>[function <span class="apidocSignatureSpan">q-io.redirect.</span>RedirectTree (location, status)](#apidoc.element.q-io.redirect.RedirectTree)
- description and source-code
```javascript
RedirectTree = function (location, status) {
    return function (request, response) {
        return exports.redirect(request, location, status, true);
    };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.q-io.redirect.TemporaryRedirect"></a>[function <span class="apidocSignatureSpan">q-io.redirect.</span>TemporaryRedirect (location, status, tree)](#apidoc.element.q-io.redirect.TemporaryRedirect)
- description and source-code
```javascript
TemporaryRedirect = function (location, status, tree) {
    return function (request, response) {
        return exports.temporaryRedirect(request, location, status, tree);
    };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.q-io.redirect.TemporaryRedirectTree"></a>[function <span class="apidocSignatureSpan">q-io.redirect.</span>TemporaryRedirectTree (location, status)](#apidoc.element.q-io.redirect.TemporaryRedirectTree)
- description and source-code
```javascript
TemporaryRedirectTree = function (location, status) {
    return function (request, response) {
        return exports.temporaryRedirect(request, location, status, true);
    };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.q-io.redirect.isRedirect"></a>[function <span class="apidocSignatureSpan">q-io.redirect.</span>isRedirect (response)](#apidoc.element.q-io.redirect.isRedirect)
- description and source-code
```javascript
isRedirect = function (response) {
    return isRedirect[response.status] || false;
}
```
- example usage
```shell
...

// try redirect loop
function next() {
    Q.fcall(function () {
        return app(request, response);
    })
    .then(function (response) {
        if (exports.isRedirect(response)) {
            if (remaining--) {
                request.url = response.headers.location;
                next();
            } else {
                throw new Error("Maximum redirects.");
            }
        } else {
...
```

#### <a name="apidoc.element.q-io.redirect.permanentRedirect"></a>[function <span class="apidocSignatureSpan">q-io.redirect.</span>permanentRedirect (request, location, status)](#apidoc.element.q-io.redirect.permanentRedirect)
- description and source-code
```javascript
permanentRedirect = function (request, location, status) {
    return exports.redirect(request, location, status || 301);
}
```
- example usage
```shell
...
/**
* @param {String} path
* @param {Number} status (optional) default is '301'
* @returns {App}
*/
exports.PermanentRedirect = function (location, status, tree) {
   return function (request, response) {
       return exports.permanentRedirect(request, location, status, tree);
   };
};

/**
* @param {String} path
* @param {Number} status (optional) default is '301'
* @returns {App}
...
```

#### <a name="apidoc.element.q-io.redirect.permanentRedirectTree"></a>[function <span class="apidocSignatureSpan">q-io.redirect.</span>permanentRedirectTree (request, location, status)](#apidoc.element.q-io.redirect.permanentRedirectTree)
- description and source-code
```javascript
permanentRedirectTree = function (request, location, status) {
    return exports.redirect(request, location, status || 301, true);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.q-io.redirect.redirectHtml"></a>[function <span class="apidocSignatureSpan">q-io.redirect.</span>redirectHtml (request, location, status)](#apidoc.element.q-io.redirect.redirectHtml)
- description and source-code
```javascript
redirectHtml = function (request, location, status) {
    var title = request.permanent ? "Permanent redirect" : "Temporary redirect";
    return {
        status: status,
        headers: {
            location: location,
            "content-type": "text/html"
        },
        htmlTitle: title,
        htmlFragment: {
            forEach: function (write) {
                write("<h1>" + HtmlApps.escapeHtml(title) + "</h1>\n");
                write(
                    "<p>See: <a href=\"" + HtmlApps.escapeHtml(location) + "\">" +
                    HtmlApps.escapeHtml(location) +
                    "</a></p>\n"
                );
            }
        }
    };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.q-io.redirect.redirectText"></a>[function <span class="apidocSignatureSpan">q-io.redirect.</span>redirectText (request, location, status)](#apidoc.element.q-io.redirect.redirectText)
- description and source-code
```javascript
redirectText = function (request, location, status) {
    var content = (
        (request.permanent ? "Permanent redirect\n" : "Temporary redirect\n") +
        "See: " + location + "\n"
    );
    var contentLength = content.length;
    return {
        status: status,
        headers: {
            location: location,
            "content-type": "text/plain"
        },
        body: [content]
    };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.q-io.redirect.redirectTree"></a>[function <span class="apidocSignatureSpan">q-io.redirect.</span>redirectTree (request, location, status)](#apidoc.element.q-io.redirect.redirectTree)
- description and source-code
```javascript
redirectTree = function (request, location, status) {
    return exports.redirect(request, location, status, true);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.q-io.redirect.temporaryRedirect"></a>[function <span class="apidocSignatureSpan">q-io.redirect.</span>temporaryRedirect (request, location, status)](#apidoc.element.q-io.redirect.temporaryRedirect)
- description and source-code
```javascript
temporaryRedirect = function (request, location, status) {
    return exports.redirect(request, location, status || 307);
}
```
- example usage
```shell
...
/**
* @param {String} path
* @param {Number} status (optional) default is '307'
* @returns {App}
*/
exports.TemporaryRedirect = function (location, status, tree) {
   return function (request, response) {
       return exports.temporaryRedirect(request, location, status, tree);
   };
};

/**
* @param {String} path
* @param {Number} status (optional) default is '307'
* @returns {App}
...
```

#### <a name="apidoc.element.q-io.redirect.temporaryRedirectTree"></a>[function <span class="apidocSignatureSpan">q-io.redirect.</span>temporaryRedirectTree (request, location, status)](#apidoc.element.q-io.redirect.temporaryRedirectTree)
- description and source-code
```javascript
temporaryRedirectTree = function (request, location, status) {
    return exports.redirect(request, location, status || 307, true);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.q-io.route"></a>[module q-io.route](#apidoc.module.q-io.route)

#### <a name="apidoc.element.q-io.route.Branch"></a>[function <span class="apidocSignatureSpan">q-io.route.</span>Branch (paths, notFound)](#apidoc.element.q-io.route.Branch)
- description and source-code
```javascript
Branch = function (paths, notFound) {
    if (!paths)
        paths = {};
    if (!notFound)
        notFound = StatusApps.notFound;
    return function (request, response) {
        if (!/^\//.test(request.pathInfo)) {
            return notFound(request, response);
        }
        var path = request.pathInfo.slice(1);
        var parts = path.split("/");
        var part = decodeURIComponent(parts.shift());
        if (Object.has(paths, part)) {
            request.scriptName = request.scriptName + part + "/";
            request.pathInfo = path.slice(part.length);
            return Object.get(paths, part)(request, response);
        }
        return notFound(request, response);
    };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.q-io.route.Cap"></a>[function <span class="apidocSignatureSpan">q-io.route.</span>Cap (app, notFound)](#apidoc.element.q-io.route.Cap)
- description and source-code
```javascript
Cap = function (app, notFound) {
    notFound = notFound || StatusApps.notFound;
    return function (request, response) {
        // TODO Distinguish these cases
        if (request.pathInfo === "" || request.pathInfo === "/") {
            return app(request, response);
        } else {
            return notFound(request, response);
        }
    };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.q-io.route.FirstFound"></a>[function <span class="apidocSignatureSpan">q-io.route.</span>FirstFound (cascade)](#apidoc.element.q-io.route.FirstFound)
- description and source-code
```javascript
FirstFound = function (cascade) {
    return function (request, response) {
        var i = 0, ii = cascade.length;
        function next() {
            var response = cascade[i++](request, response);
            if (i < ii) {
                return Q.when(response, function (response) {
                    if (response.status === 404) {
                        return next();
                    } else {
                        return response;
                    }
                });
            } else {
                return response;
            }
        }
        return next();
    };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.q-io.route.Tap"></a>[function <span class="apidocSignatureSpan">q-io.route.</span>Tap (app, tap)](#apidoc.element.q-io.route.Tap)
- description and source-code
```javascript
Tap = function (app, tap) {
    return function (request, response) {
        var self = this, args = arguments;
        return Q.when(tap.apply(this, arguments), function (response) {
            if (response) {
                return response;
            } else {
                return app.apply(self, args);
            }
        });
    };
}
```
- example usage
```shell
...
    24 * // h
    365 * // d
    10; // years
exports.Permanent = function (app, future) {
    future = future || function () {
        return new Date(new Date().getTime() + farFuture);
    };
    app = RouteApps.Tap(app, function (request, response) {
        request.permanent = future;
    });
    app = RouteApps.Trap(app, function (response, request) {
        response.headers["expires"] = "" + future();
    });
    return app;
};
...
```

#### <a name="apidoc.element.q-io.route.Trap"></a>[function <span class="apidocSignatureSpan">q-io.route.</span>Trap (app, trap)](#apidoc.element.q-io.route.Trap)
- description and source-code
```javascript
Trap = function (app, trap) {
    return function (request, response) {
        return Q.when(app.apply(this, arguments), function (response) {
            if (response) {
                response.headers = response.headers || {};
                return trap(response, request) || response;
            }
        });
    };
}
```
- example usage
```shell
...
   };
};

exports.Date = function (app, present) {
   present = present || function () {
       return new Date();
   };
   return RouteApps.Trap(app, function (response, request) {
       response.headers["date"] = "" + present();
   });
};

/**
* Decorates a JSGI application such that rejected response promises
* get translated into '500' server error responses with no content.
...
```



# <a name="apidoc.module.q-io.status"></a>[module q-io.status](#apidoc.module.q-io.status)

#### <a name="apidoc.element.q-io.status.appForStatus"></a>[function <span class="apidocSignatureSpan">q-io.status.</span>appForStatus (status)](#apidoc.element.q-io.status.appForStatus)
- description and source-code
```javascript
appForStatus = function (status) {
    return function (request) {
        return exports.responseForStatus(request, status, request.method + " " + request.path);
    };
}
```
- example usage
```shell
...
       }
   }
};

/**
* {App} an application that returns a 400 response.
*/
exports.badRequest = exports.appForStatus(400);
/**
* {App} an application that returns a 404 response.
*/
exports.notFound = exports.appForStatus(404);
/**
* {App} an application that returns a 405 response.
*/
...
```

#### <a name="apidoc.element.q-io.status.badRequest"></a>[function <span class="apidocSignatureSpan">q-io.status.</span>badRequest (request)](#apidoc.element.q-io.status.badRequest)
- description and source-code
```javascript
badRequest = function (request) {
    return exports.responseForStatus(request, status, request.method + " " + request.path);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.q-io.status.htmlResponseForStatus"></a>[function <span class="apidocSignatureSpan">q-io.status.</span>htmlResponseForStatus (request, status, message, addendum)](#apidoc.element.q-io.status.htmlResponseForStatus)
- description and source-code
```javascript
htmlResponseForStatus = function (request, status, message, addendum) {
    return {
        status: status,
        statusMessage: message,
        headers: {},
        htmlTitle: message,
        htmlFragment: {
            forEach: function (write) {
                write("<h1>" + HtmlApps.escapeHtml(message) + "</h1>\n");
                write("<p>Status: " + status + "</p>\n");
                if (addendum) {
                    write("<pre>" + HtmlApps.escapeHtml(addendum) + "</pre>\n");
                }
            }
        }
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.q-io.status.methodNotAllowed"></a>[function <span class="apidocSignatureSpan">q-io.status.</span>methodNotAllowed (request)](#apidoc.element.q-io.status.methodNotAllowed)
- description and source-code
```javascript
methodNotAllowed = function (request) {
    return exports.responseForStatus(request, status, request.method + " " + request.path);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.q-io.status.noLanguage"></a>[function <span class="apidocSignatureSpan">q-io.status.</span>noLanguage (request)](#apidoc.element.q-io.status.noLanguage)
- description and source-code
```javascript
noLanguage = function (request) {
    return exports.responseForStatus(request, status, request.method + " " + request.path);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.q-io.status.notAcceptable"></a>[function <span class="apidocSignatureSpan">q-io.status.</span>notAcceptable (request)](#apidoc.element.q-io.status.notAcceptable)
- description and source-code
```javascript
notAcceptable = function (request) {
    return exports.responseForStatus(request, status, request.method + " " + request.path);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.q-io.status.notFound"></a>[function <span class="apidocSignatureSpan">q-io.status.</span>notFound (request)](#apidoc.element.q-io.status.notFound)
- description and source-code
```javascript
notFound = function (request) {
    return exports.responseForStatus(request, status, request.method + " " + request.path);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.q-io.status.responseForStatus"></a>[function <span class="apidocSignatureSpan">q-io.status.</span>responseForStatus (request, status, addendum)](#apidoc.element.q-io.status.responseForStatus)
- description and source-code
```javascript
responseForStatus = function (request, status, addendum) {
    if (exports.statusCodes[status] === undefined)
        throw "Unknown status code";

    var message = exports.statusCodes[status];

    // RFC 2616, 10.2.5:
    // The 204 response MUST NOT include a message-body, and thus is always
    // terminated by the first empty line after the header fields.
    // RFC 2616, 10.3.5:
    // The 304 response MUST NOT contain a message-body, and thus is always
    // terminated by the first empty line after the header fields.
    if (exports.statusWithNoEntityBody(status)) {
        return {status: status, headers: {}};
    } else {
        var handlers = {};
        handlers["text/plain"] = exports.textResponseForStatus;
        if (request.handleHtmlFragmentResponse) {
            handlers["text/html"] = exports.htmlResponseForStatus;
        }
        var responseForStatus = Negotiation.negotiate(request, handlers) || exports.textResponseForStatus;
        return responseForStatus(request, status, message, addendum);
    }
}
```
- example usage
```shell
...
 * @returns {App}
 */
exports.Error = function (app, debug) {
    return function (request, response) {
        return Q.when(app(request, response), null, function (error) {
            if (!debug)
                error = undefined;
            return StatusApps.responseForStatus(request, 500, error && error.stack || error);
        });
    };
};

exports.Debug = function (app) {
    return exports.Error(app, true);
};
...
```

#### <a name="apidoc.element.q-io.status.statusWithNoEntityBody"></a>[function <span class="apidocSignatureSpan">q-io.status.</span>statusWithNoEntityBody (status)](#apidoc.element.q-io.status.statusWithNoEntityBody)
- description and source-code
```javascript
statusWithNoEntityBody = function (status) {
    return (status >= 100 && status <= 199) ||
        status == 204 || status == 304;
}
```
- example usage
```shell
...

// RFC 2616, 10.2.5:
// The 204 response MUST NOT include a message-body, and thus is always
// terminated by the first empty line after the header fields.
// RFC 2616, 10.3.5:
// The 304 response MUST NOT contain a message-body, and thus is always
// terminated by the first empty line after the header fields.
if (exports.statusWithNoEntityBody(status)) {
    return {status: status, headers: {}};
} else {
    var handlers = {};
    handlers["text/plain"] = exports.textResponseForStatus;
    if (request.handleHtmlFragmentResponse) {
        handlers["text/html"] = exports.htmlResponseForStatus;
    }
...
```

#### <a name="apidoc.element.q-io.status.textResponseForStatus"></a>[function <span class="apidocSignatureSpan">q-io.status.</span>textResponseForStatus (request, status, message, addendum)](#apidoc.element.q-io.status.textResponseForStatus)
- description and source-code
```javascript
textResponseForStatus = function (request, status, message, addendum) {
    var content = message + "\n";
    if (addendum) {
        content += addendum + "\n";
    }
    var contentLength = content.length;
    return {
        status: status,
        statusMessage: message,
        headers: {
            "content-length": contentLength
        },
        body: [content]
    };
}
```
- example usage
```shell
n/a
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
