# api documentation for  [node-resque (v4.0.5)](http://github.com/taskrabbit/node-resque)  [![npm package](https://img.shields.io/npm/v/npmdoc-node-resque.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-node-resque) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-node-resque.svg)](https://travis-ci.org/npmdoc/node-npmdoc-node-resque)
#### an opinionated implementation of resque in node

[![NPM](https://nodei.co/npm/node-resque.png?downloads=true)](https://www.npmjs.com/package/node-resque)

[![apidoc](https://npmdoc.github.io/node-npmdoc-node-resque/build/screenCapture.buildNpmdoc.browser._2Fhome_2Ftravis_2Fbuild_2Fnpmdoc_2Fnode-npmdoc-node-resque_2Ftmp_2Fbuild_2Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-node-resque/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-node-resque/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-node-resque/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Evan Tahler",
        "email": "evantahler@gmail.com"
    },
    "bugs": {
        "url": "https://github.com/taskrabbit/node-resque/issues"
    },
    "dependencies": {
        "async": "^2.0.1",
        "ioredis": "^2.0.0"
    },
    "description": "an opinionated implementation of resque in node",
    "devDependencies": {
        "fakeredis": "latest",
        "mocha": "latest",
        "node-schedule": "latest",
        "should": "latest"
    },
    "directories": {},
    "dist": {
        "shasum": "236ef9bd960d1fd40a07cbf674ba9e56dc3be9df",
        "tarball": "https://registry.npmjs.org/node-resque/-/node-resque-4.0.5.tgz"
    },
    "engines": {
        "node": ">= 4"
    },
    "gitHead": "1e73376fa0acdbcc3b91d368ae7d8ea3e8ac04df",
    "homepage": "http://github.com/taskrabbit/node-resque",
    "keywords": [
        "delayed",
        "queue",
        "resque",
        "redis",
        "work",
        "worker",
        "background",
        "job"
    ],
    "license": "Apache-2.0",
    "main": "index.js",
    "maintainers": [
        {
            "name": "evantahler",
            "email": "evan@evantahler.com"
        },
        {
            "name": "bleonard",
            "email": "brian@bleonard.com"
        },
        {
            "name": "davidjairala",
            "email": "davidjairala@gmail.com"
        }
    ],
    "name": "node-resque",
    "optionalDependencies": {},
    "readme": "ERROR: No README data found!",
    "repository": {
        "type": "git",
        "url": "git://github.com/taskrabbit/node-resque.git"
    },
    "scripts": {
        "test": "mocha"
    },
    "version": "4.0.5"
}
```



# <a name="apidoc.tableOfContents"></a>[table of contents](#apidoc.tableOfContents)

#### [module node-resque](#apidoc.module.node-resque)
1.  [function <span class="apidocSignatureSpan">node-resque.</span>connection (options)](#apidoc.element.node-resque.connection)
1.  [function <span class="apidocSignatureSpan">node-resque.</span>multiWorker (options, jobs)](#apidoc.element.node-resque.multiWorker)
1.  [function <span class="apidocSignatureSpan">node-resque.</span>queue (options, jobs)](#apidoc.element.node-resque.queue)
1.  [function <span class="apidocSignatureSpan">node-resque.</span>scheduler (options, jobs)](#apidoc.element.node-resque.scheduler)
1.  [function <span class="apidocSignatureSpan">node-resque.</span>worker (options, jobs)](#apidoc.element.node-resque.worker)
1.  object <span class="apidocSignatureSpan">node-resque.</span>connection.prototype
1.  object <span class="apidocSignatureSpan">node-resque.</span>multiWorker.prototype
1.  object <span class="apidocSignatureSpan">node-resque.</span>pluginRunner
1.  object <span class="apidocSignatureSpan">node-resque.</span>queue.prototype
1.  object <span class="apidocSignatureSpan">node-resque.</span>scheduler.prototype
1.  object <span class="apidocSignatureSpan">node-resque.</span>worker.prototype

#### [module node-resque.connection](#apidoc.module.node-resque.connection)
1.  [function <span class="apidocSignatureSpan">node-resque.</span>connection (options)](#apidoc.element.node-resque.connection.connection)
1.  [function <span class="apidocSignatureSpan">node-resque.connection.</span>super_ ()](#apidoc.element.node-resque.connection.super_)

#### [module node-resque.connection.prototype](#apidoc.module.node-resque.connection.prototype)
1.  [function <span class="apidocSignatureSpan">node-resque.connection.prototype.</span>connect (callback)](#apidoc.element.node-resque.connection.prototype.connect)
1.  [function <span class="apidocSignatureSpan">node-resque.connection.prototype.</span>defaults ()](#apidoc.element.node-resque.connection.prototype.defaults)
1.  [function <span class="apidocSignatureSpan">node-resque.connection.prototype.</span>end ()](#apidoc.element.node-resque.connection.prototype.end)
1.  [function <span class="apidocSignatureSpan">node-resque.connection.prototype.</span>key ()](#apidoc.element.node-resque.connection.prototype.key)

#### [module node-resque.multiWorker](#apidoc.module.node-resque.multiWorker)
1.  [function <span class="apidocSignatureSpan">node-resque.</span>multiWorker (options, jobs)](#apidoc.element.node-resque.multiWorker.multiWorker)
1.  [function <span class="apidocSignatureSpan">node-resque.multiWorker.</span>super_ ()](#apidoc.element.node-resque.multiWorker.super_)

#### [module node-resque.multiWorker.prototype](#apidoc.module.node-resque.multiWorker.prototype)
1.  [function <span class="apidocSignatureSpan">node-resque.multiWorker.prototype.</span>checkWorkers (callback)](#apidoc.element.node-resque.multiWorker.prototype.checkWorkers)
1.  [function <span class="apidocSignatureSpan">node-resque.multiWorker.prototype.</span>checkWraper (callback)](#apidoc.element.node-resque.multiWorker.prototype.checkWraper)
1.  [function <span class="apidocSignatureSpan">node-resque.multiWorker.prototype.</span>cleanupWorker (worker)](#apidoc.element.node-resque.multiWorker.prototype.cleanupWorker)
1.  [function <span class="apidocSignatureSpan">node-resque.multiWorker.prototype.</span>defaults ()](#apidoc.element.node-resque.multiWorker.prototype.defaults)
1.  [function <span class="apidocSignatureSpan">node-resque.multiWorker.prototype.</span>end (callback)](#apidoc.element.node-resque.multiWorker.prototype.end)
1.  [function <span class="apidocSignatureSpan">node-resque.multiWorker.prototype.</span>start (callback)](#apidoc.element.node-resque.multiWorker.prototype.start)
1.  [function <span class="apidocSignatureSpan">node-resque.multiWorker.prototype.</span>startWorker (callback)](#apidoc.element.node-resque.multiWorker.prototype.startWorker)
1.  [function <span class="apidocSignatureSpan">node-resque.multiWorker.prototype.</span>stop (callback)](#apidoc.element.node-resque.multiWorker.prototype.stop)
1.  [function <span class="apidocSignatureSpan">node-resque.multiWorker.prototype.</span>stopWait (callback)](#apidoc.element.node-resque.multiWorker.prototype.stopWait)

#### [module node-resque.pluginRunner](#apidoc.module.node-resque.pluginRunner)
1.  [function <span class="apidocSignatureSpan">node-resque.pluginRunner.</span>runPlugin (self, pluginRefrence, type, func, queue, job, args, callback)](#apidoc.element.node-resque.pluginRunner.runPlugin)
1.  [function <span class="apidocSignatureSpan">node-resque.pluginRunner.</span>runPlugins (self, type, func, queue, job, args, callback, pluginCounter)](#apidoc.element.node-resque.pluginRunner.runPlugins)

#### [module node-resque.queue](#apidoc.module.node-resque.queue)
1.  [function <span class="apidocSignatureSpan">node-resque.</span>queue (options, jobs)](#apidoc.element.node-resque.queue.queue)
1.  [function <span class="apidocSignatureSpan">node-resque.queue.</span>super_ ()](#apidoc.element.node-resque.queue.super_)

#### [module node-resque.queue.prototype](#apidoc.module.node-resque.queue.prototype)
1.  [function <span class="apidocSignatureSpan">node-resque.queue.prototype.</span>allDelayed (callback)](#apidoc.element.node-resque.queue.prototype.allDelayed)
1.  [function <span class="apidocSignatureSpan">node-resque.queue.prototype.</span>allWorkingOn (callback)](#apidoc.element.node-resque.queue.prototype.allWorkingOn)
1.  [function <span class="apidocSignatureSpan">node-resque.queue.prototype.</span>cleanOldWorkers (age, callback)](#apidoc.element.node-resque.queue.prototype.cleanOldWorkers)
1.  [function <span class="apidocSignatureSpan">node-resque.queue.prototype.</span>connect (callback)](#apidoc.element.node-resque.queue.prototype.connect)
1.  [function <span class="apidocSignatureSpan">node-resque.queue.prototype.</span>del (q, func, args, count, callback)](#apidoc.element.node-resque.queue.prototype.del)
1.  [function <span class="apidocSignatureSpan">node-resque.queue.prototype.</span>delDelayed (q, func, args, callback)](#apidoc.element.node-resque.queue.prototype.delDelayed)
1.  [function <span class="apidocSignatureSpan">node-resque.queue.prototype.</span>delLock (key, callback)](#apidoc.element.node-resque.queue.prototype.delLock)
1.  [function <span class="apidocSignatureSpan">node-resque.queue.prototype.</span>delQueue (q, callback)](#apidoc.element.node-resque.queue.prototype.delQueue)
1.  [function <span class="apidocSignatureSpan">node-resque.queue.prototype.</span>delayedAt (timestamp, callback)](#apidoc.element.node-resque.queue.prototype.delayedAt)
1.  [function <span class="apidocSignatureSpan">node-resque.queue.prototype.</span>encode (q, func, args)](#apidoc.element.node-resque.queue.prototype.encode)
1.  [function <span class="apidocSignatureSpan">node-resque.queue.prototype.</span>end (callback)](#apidoc.element.node-resque.queue.prototype.end)
1.  [function <span class="apidocSignatureSpan">node-resque.queue.prototype.</span>enqueue (q, func, args, callback)](#apidoc.element.node-resque.queue.prototype.enqueue)
1.  [function <span class="apidocSignatureSpan">node-resque.queue.prototype.</span>enqueueAt (timestamp, q, func, args, callback)](#apidoc.element.node-resque.queue.prototype.enqueueAt)
1.  [function <span class="apidocSignatureSpan">node-resque.queue.prototype.</span>enqueueIn (time, q, func, args, callback)](#apidoc.element.node-resque.queue.prototype.enqueueIn)
1.  [function <span class="apidocSignatureSpan">node-resque.queue.prototype.</span>failed (start, stop, callback)](#apidoc.element.node-resque.queue.prototype.failed)
1.  [function <span class="apidocSignatureSpan">node-resque.queue.prototype.</span>failedCount (callback)](#apidoc.element.node-resque.queue.prototype.failedCount)
1.  [function <span class="apidocSignatureSpan">node-resque.queue.prototype.</span>forceCleanWorker (workerName, callback)](#apidoc.element.node-resque.queue.prototype.forceCleanWorker)
1.  [function <span class="apidocSignatureSpan">node-resque.queue.prototype.</span>length (q, callback)](#apidoc.element.node-resque.queue.prototype.length)
1.  [function <span class="apidocSignatureSpan">node-resque.queue.prototype.</span>locks (callback)](#apidoc.element.node-resque.queue.prototype.locks)
1.  [function <span class="apidocSignatureSpan">node-resque.queue.prototype.</span>queued (q, start, stop, callback)](#apidoc.element.node-resque.queue.prototype.queued)
1.  [function <span class="apidocSignatureSpan">node-resque.queue.prototype.</span>queues (callback)](#apidoc.element.node-resque.queue.prototype.queues)
1.  [function <span class="apidocSignatureSpan">node-resque.queue.prototype.</span>removeFailed (failedJob, callback)](#apidoc.element.node-resque.queue.prototype.removeFailed)
1.  [function <span class="apidocSignatureSpan">node-resque.queue.prototype.</span>retryAndRemoveFailed (failedJob, callback)](#apidoc.element.node-resque.queue.prototype.retryAndRemoveFailed)
1.  [function <span class="apidocSignatureSpan">node-resque.queue.prototype.</span>scheduledAt (q, func, args, callback)](#apidoc.element.node-resque.queue.prototype.scheduledAt)
1.  [function <span class="apidocSignatureSpan">node-resque.queue.prototype.</span>stats (callback)](#apidoc.element.node-resque.queue.prototype.stats)
1.  [function <span class="apidocSignatureSpan">node-resque.queue.prototype.</span>timestamps (callback)](#apidoc.element.node-resque.queue.prototype.timestamps)
1.  [function <span class="apidocSignatureSpan">node-resque.queue.prototype.</span>workers (callback)](#apidoc.element.node-resque.queue.prototype.workers)
1.  [function <span class="apidocSignatureSpan">node-resque.queue.prototype.</span>workingOn (workerName, queues, callback)](#apidoc.element.node-resque.queue.prototype.workingOn)

#### [module node-resque.scheduler](#apidoc.module.node-resque.scheduler)
1.  [function <span class="apidocSignatureSpan">node-resque.</span>scheduler (options, jobs)](#apidoc.element.node-resque.scheduler.scheduler)
1.  [function <span class="apidocSignatureSpan">node-resque.scheduler.</span>super_ ()](#apidoc.element.node-resque.scheduler.super_)

#### [module node-resque.scheduler.prototype](#apidoc.module.node-resque.scheduler.prototype)
1.  [function <span class="apidocSignatureSpan">node-resque.scheduler.prototype.</span>cleanupTimestamp (timestamp, callback)](#apidoc.element.node-resque.scheduler.prototype.cleanupTimestamp)
1.  [function <span class="apidocSignatureSpan">node-resque.scheduler.prototype.</span>connect (callback)](#apidoc.element.node-resque.scheduler.prototype.connect)
1.  [function <span class="apidocSignatureSpan">node-resque.scheduler.prototype.</span>defaults ()](#apidoc.element.node-resque.scheduler.prototype.defaults)
1.  [function <span class="apidocSignatureSpan">node-resque.scheduler.prototype.</span>end (callback)](#apidoc.element.node-resque.scheduler.prototype.end)
1.  [function <span class="apidocSignatureSpan">node-resque.scheduler.prototype.</span>enqueueDelayedItemsForTimestamp (timestamp, callback)](#apidoc.element.node-resque.scheduler.prototype.enqueueDelayedItemsForTimestamp)
1.  [function <span class="apidocSignatureSpan">node-resque.scheduler.prototype.</span>masterKey ()](#apidoc.element.node-resque.scheduler.prototype.masterKey)
1.  [function <span class="apidocSignatureSpan">node-resque.scheduler.prototype.</span>nextDelayedTimestamp (callback)](#apidoc.element.node-resque.scheduler.prototype.nextDelayedTimestamp)
1.  [function <span class="apidocSignatureSpan">node-resque.scheduler.prototype.</span>nextItemForTimestamp (timestamp, callback)](#apidoc.element.node-resque.scheduler.prototype.nextItemForTimestamp)
1.  [function <span class="apidocSignatureSpan">node-resque.scheduler.prototype.</span>poll (callback)](#apidoc.element.node-resque.scheduler.prototype.poll)
1.  [function <span class="apidocSignatureSpan">node-resque.scheduler.prototype.</span>pollAgainLater ()](#apidoc.element.node-resque.scheduler.prototype.pollAgainLater)
1.  [function <span class="apidocSignatureSpan">node-resque.scheduler.prototype.</span>releaseMasterLock (callback)](#apidoc.element.node-resque.scheduler.prototype.releaseMasterLock)
1.  [function <span class="apidocSignatureSpan">node-resque.scheduler.prototype.</span>start ()](#apidoc.element.node-resque.scheduler.prototype.start)
1.  [function <span class="apidocSignatureSpan">node-resque.scheduler.prototype.</span>transfer (timestamp, job, callback)](#apidoc.element.node-resque.scheduler.prototype.transfer)
1.  [function <span class="apidocSignatureSpan">node-resque.scheduler.prototype.</span>tryForMaster (callback)](#apidoc.element.node-resque.scheduler.prototype.tryForMaster)

#### [module node-resque.worker](#apidoc.module.node-resque.worker)
1.  [function <span class="apidocSignatureSpan">node-resque.</span>worker (options, jobs)](#apidoc.element.node-resque.worker.worker)
1.  [function <span class="apidocSignatureSpan">node-resque.worker.</span>super_ ()](#apidoc.element.node-resque.worker.super_)

#### [module node-resque.worker.prototype](#apidoc.module.node-resque.worker.prototype)
1.  [function <span class="apidocSignatureSpan">node-resque.worker.prototype.</span>checkQueues (callback)](#apidoc.element.node-resque.worker.prototype.checkQueues)
1.  [function <span class="apidocSignatureSpan">node-resque.worker.prototype.</span>completeJob (toRespond, callback)](#apidoc.element.node-resque.worker.prototype.completeJob)
1.  [function <span class="apidocSignatureSpan">node-resque.worker.prototype.</span>connect (callback)](#apidoc.element.node-resque.worker.prototype.connect)
1.  [function <span class="apidocSignatureSpan">node-resque.worker.prototype.</span>defaults ()](#apidoc.element.node-resque.worker.prototype.defaults)
1.  [function <span class="apidocSignatureSpan">node-resque.worker.prototype.</span>doneWorking (callback)](#apidoc.element.node-resque.worker.prototype.doneWorking)
1.  [function <span class="apidocSignatureSpan">node-resque.worker.prototype.</span>end (callback)](#apidoc.element.node-resque.worker.prototype.end)
1.  [function <span class="apidocSignatureSpan">node-resque.worker.prototype.</span>fail (err, callback)](#apidoc.element.node-resque.worker.prototype.fail)
1.  [function <span class="apidocSignatureSpan">node-resque.worker.prototype.</span>failurePayload (err, job)](#apidoc.element.node-resque.worker.prototype.failurePayload)
1.  [function <span class="apidocSignatureSpan">node-resque.worker.prototype.</span>getPids (callback)](#apidoc.element.node-resque.worker.prototype.getPids)
1.  [function <span class="apidocSignatureSpan">node-resque.worker.prototype.</span>init (callback)](#apidoc.element.node-resque.worker.prototype.init)
1.  [function <span class="apidocSignatureSpan">node-resque.worker.prototype.</span>pause ()](#apidoc.element.node-resque.worker.prototype.pause)
1.  [function <span class="apidocSignatureSpan">node-resque.worker.prototype.</span>perform (job, callback)](#apidoc.element.node-resque.worker.prototype.perform)
1.  [function <span class="apidocSignatureSpan">node-resque.worker.prototype.</span>performInline (func, args, callback)](#apidoc.element.node-resque.worker.prototype.performInline)
1.  [function <span class="apidocSignatureSpan">node-resque.worker.prototype.</span>poll (nQueue, callback)](#apidoc.element.node-resque.worker.prototype.poll)
1.  [function <span class="apidocSignatureSpan">node-resque.worker.prototype.</span>start ()](#apidoc.element.node-resque.worker.prototype.start)
1.  [function <span class="apidocSignatureSpan">node-resque.worker.prototype.</span>stringQueues ()](#apidoc.element.node-resque.worker.prototype.stringQueues)
1.  [function <span class="apidocSignatureSpan">node-resque.worker.prototype.</span>succeed (job, callback)](#apidoc.element.node-resque.worker.prototype.succeed)
1.  [function <span class="apidocSignatureSpan">node-resque.worker.prototype.</span>track (callback)](#apidoc.element.node-resque.worker.prototype.track)
1.  [function <span class="apidocSignatureSpan">node-resque.worker.prototype.</span>untrack (name, queues, callback)](#apidoc.element.node-resque.worker.prototype.untrack)
1.  [function <span class="apidocSignatureSpan">node-resque.worker.prototype.</span>workerCleanup (callback)](#apidoc.element.node-resque.worker.prototype.workerCleanup)
1.  [function <span class="apidocSignatureSpan">node-resque.worker.prototype.</span>workingOn (job)](#apidoc.element.node-resque.worker.prototype.workingOn)



# <a name="apidoc.module.node-resque"></a>[module node-resque](#apidoc.module.node-resque)

#### <a name="apidoc.element.node-resque.connection"></a>[function <span class="apidocSignatureSpan">node-resque.</span>connection (options)](#apidoc.element.node-resque.connection)
- description and source-code
```javascript
connection = function (options){
  var self = this;
  var defaults = self.defaults();

  if(!options){ options = {}; }
  for(var i in defaults){
    if(options[i] === null || options[i] === undefined){
      options[i] = defaults[i];
    }
  }
  self.options = options;
  self.listeners = {};
  self.connected = false;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-resque.multiWorker"></a>[function <span class="apidocSignatureSpan">node-resque.</span>multiWorker (options, jobs)](#apidoc.element.node-resque.multiWorker)
- description and source-code
```javascript
multiWorker = function (options, jobs){
  var self = this;

  var defaults = self.defaults();
  for(var i in defaults){
    if(options[i] === null || options[i] === undefined){
      options[i] = defaults[i];
    }
  }

  if(options.connection.redis && typeof options.connection.redis.setMaxListeners === 'function'){
    options.connection.redis.setMaxListeners(options.connection.redis.getMaxListeners() + options.maxTaskProcessors);
  }

  self.workers = [];
  self.options = options;
  self.jobs = jobs;
  self.running = false;
  self.working = false;
  self.name = self.options.name;
  self.eventLoopBlocked = true;
  self.eventLoopDelay = Infinity;
  self.eventLoopCheckCounter = 0;

  eventLoopDelay(
    self.options.maxEventLoopDelay,
    self.options.checkTimeout,
  function(blocked, ms){
    self.eventLoopBlocked = blocked;
    self.eventLoopDelay = ms;
    self.eventLoopCheckCounter++;
  });
}
```
- example usage
```shell
...

var connectionDetails = {
pkg:       "ioredis",
host:      "127.0.0.1",
password:  ""
}

var multiWorker = new NR.multiWorker({
connection: connectionDetails,
queues: ['slowQueue'],
minTaskProcessors:   1,
maxTaskProcessors:   100,
checkTimeout:        1000,
maxEventLoopDelay:   10,
toDisconnectProcessors: true,
...
```

#### <a name="apidoc.element.node-resque.queue"></a>[function <span class="apidocSignatureSpan">node-resque.</span>queue (options, jobs)](#apidoc.element.node-resque.queue)
- description and source-code
```javascript
queue = function (options, jobs){
  var self = this;
  if(!jobs){ jobs = {}; }

  self.options = options;
  self.jobs    = jobs;

  self.connection = new connection(options.connection);

  self.connection.on('error', function(error){
    self.emit('error', error);
  });
}
```
- example usage
```shell
...
scheduler.on('working_timestamp', function(timestamp){ console.log("scheduler working timestamp " + timestamp); });
scheduler.on('transferred_job',   function(timestamp, job){ console.log("scheduler enquing job " + timestamp + " >> " + JSON.stringify
(job)); });

////////////////////////
// CONNECT TO A QUEUE //
////////////////////////

var queue = new NR.queue({connection: connectionDetails}, jobs);
queue.on('error', function(error){ console.log(error); });
queue.connect(function(){
  queue.enqueue('math', "add", [1,2]);
  queue.enqueue('math', "add", [1,2]);
  queue.enqueue('math', "add", [2,3]);
  queue.enqueueIn(3000, 'math', "subtract", [2,1]);
});
...
```

#### <a name="apidoc.element.node-resque.scheduler"></a>[function <span class="apidocSignatureSpan">node-resque.</span>scheduler (options, jobs)](#apidoc.element.node-resque.scheduler)
- description and source-code
```javascript
scheduler = function (options, jobs){
  var self = this;
  if(!jobs){ jobs = {}; }
  var defaults = self.defaults();

  for(var i in defaults){
    if(options[i] === null || options[i] === undefined){
      options[i] = defaults[i];
    }
  }

  self.options    = options;
  self.name       = self.options.name;
  self.master     = false;
  self.running    = false;
  self.processing = false;

  self.queue = new queue({connection: options.connection}, jobs);

  self.queue.on('error', function(error){
    self.emit('error', error);
  });
}
```
- example usage
```shell
...
  worker.start();
});

///////////////////////
// START A SCHEDULER //
///////////////////////

var scheduler = new NR.scheduler({connection: connectionDetails});
scheduler.connect(function(){
  scheduler.start();
});

/////////////////////////
// REGESTER FOR EVENTS //
/////////////////////////
...
```

#### <a name="apidoc.element.node-resque.worker"></a>[function <span class="apidocSignatureSpan">node-resque.</span>worker (options, jobs)](#apidoc.element.node-resque.worker)
- description and source-code
```javascript
worker = function (options, jobs){
  var self = this;
  if(!jobs){ jobs = {}; }

  var defaults = self.defaults();
  for(var i in defaults){
    if(options[i] === undefined || options[i] === null){
      options[i] = defaults[i];
    }
  }

  self.options = options;
  self.jobs = prepareJobs(jobs);
  self.name = self.options.name;
  self.queues = self.options.queues;
  self.error = null;
  self.result = null;
  self.ready = false;
  self.running = false;
  self.working = false;
  self.job = null;

  self.queueObject = new queue({connection: options.connection}, self.jobs);

  self.queueObject.on('error', function(error){
    self.emit('error', null, null, error);
  });
}
```
- example usage
```shell
...
  },
};

////////////////////
// START A WORKER //
////////////////////

var worker = new NR.worker({connection: connectionDetails, queues: ['math', 'otherQueue']}, jobs);
worker.connect(function(){
  worker.workerCleanup(); // optional: cleanup any previous improperly shutdown workers on this host
  worker.start();
});

///////////////////////
// START A SCHEDULER //
...
```



# <a name="apidoc.module.node-resque.connection"></a>[module node-resque.connection](#apidoc.module.node-resque.connection)

#### <a name="apidoc.element.node-resque.connection.connection"></a>[function <span class="apidocSignatureSpan">node-resque.</span>connection (options)](#apidoc.element.node-resque.connection.connection)
- description and source-code
```javascript
connection = function (options){
  var self = this;
  var defaults = self.defaults();

  if(!options){ options = {}; }
  for(var i in defaults){
    if(options[i] === null || options[i] === undefined){
      options[i] = defaults[i];
    }
  }
  self.options = options;
  self.listeners = {};
  self.connected = false;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-resque.connection.super_"></a>[function <span class="apidocSignatureSpan">node-resque.connection.</span>super_ ()](#apidoc.element.node-resque.connection.super_)
- description and source-code
```javascript
function EventEmitter() {
  EventEmitter.init.call(this);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.node-resque.connection.prototype"></a>[module node-resque.connection.prototype](#apidoc.module.node-resque.connection.prototype)

#### <a name="apidoc.element.node-resque.connection.prototype.connect"></a>[function <span class="apidocSignatureSpan">node-resque.connection.prototype.</span>connect (callback)](#apidoc.element.node-resque.connection.prototype.connect)
- description and source-code
```javascript
connect = function (callback){
  var self = this;

  if(self.options.redis){
    var jobs = [];
    self.redis = self.options.redis;

    jobs.push(function(done){
      self.redis.set(self.key('connection_test_key'), 'true', done);
    });

    jobs.push(function(done){
      self.redis.get(self.key('connection_test_key'), function(error, data){
        if(!error && data !== 'true'){ error = new Error('cannot read connection test key'); }
        if(error){
          self.connected = false;
          self.emit('error', error);
          return done(error);
        }
        self.connected = true;
        done();
      });
    });

    async.series(jobs, callback);
  }else{

    if(self.options['package'] && !self.options.pkg){
      self.emit('Depreciation warning: You need to use \'pkg\' instead of \'package\'! Please update your configuration.');
      self.options.pkg = self.options['package'];
    }
    var pkg = require(self.options.pkg);
    self.redis = pkg.createClient(self.options.port, self.options.host, self.options.options);

    self.listeners.connect = function(){
      if(self.connected === true){
        // nothing to do here; this is a reconnect
      }else{
        self.redis.select(self.options.database, function(error){
          if(error){
            self.connected = false;
            self.emit('error', error);
            return callback(error);
          }else{
            self.connected = true;
            return callback();
          }
        });
      }
    };

    self.redis.on('connect', self.listeners.connect);
    if(self.options.pkg === 'fakeredis'){ process.nextTick(self.listeners.connect); }
  }

  self.listeners.error = function(error){ self.emit('error', error); };
  self.redis.on('error', self.listeners.error);

  self.listeners.end = function(){ self.connected = false; };
  self.redis.on('end', self.listeners.end);
}
```
- example usage
```shell
...
};

////////////////////
// START A WORKER //
////////////////////

var worker = new NR.worker({connection: connectionDetails, queues: ['math', 'otherQueue']}, jobs);
worker.connect(function(){
  worker.workerCleanup(); // optional: cleanup any previous improperly shutdown workers on this host
  worker.start();
});

///////////////////////
// START A SCHEDULER //
///////////////////////
...
```

#### <a name="apidoc.element.node-resque.connection.prototype.defaults"></a>[function <span class="apidocSignatureSpan">node-resque.connection.prototype.</span>defaults ()](#apidoc.element.node-resque.connection.prototype.defaults)
- description and source-code
```javascript
defaults = function (){
  return {
    pkg:       'ioredis',
    host:      '127.0.0.1',
    port:      6379,
    database:  0,
    namespace: 'resque',
  };
}
```
- example usage
```shell
...

var util  = require('util');
var async = require('async');
var EventEmitter = require('events').EventEmitter;

var connection = function(options){
var self = this;
var defaults = self.defaults();

if(!options){ options = {}; }
for(var i in defaults){
  if(options[i] === null || options[i] === undefined){
    options[i] = defaults[i];
  }
}
...
```

#### <a name="apidoc.element.node-resque.connection.prototype.end"></a>[function <span class="apidocSignatureSpan">node-resque.connection.prototype.</span>end ()](#apidoc.element.node-resque.connection.prototype.end)
- description and source-code
```javascript
end = function (){
  var self = this;
  self.connected = false;

  Object.keys(self.listeners).forEach(function(eventName){
    self.redis.removeListener(eventName, self.listeners[eventName]);
  });

  // Only disconnect if we established the redis connection on our own.
  if(!self.options.redis && self.options.pkg !== 'fakeredis'){
    if(typeof self.redis.disconnect === 'function'){ self.redis.disconnect(); }
    else{ self.redis.quit(); }
  }
}
```
- example usage
```shell
...

worker.connect(function(){
  worker.start();
});
'''

## Notes
- Be sure to call 'worker.end(callback)', 'queue.end(callback)' and 'scheduler.end(callback)' before shutting down your application
 if you want to properly clear your worker status from resque
- When ending your application, be sure to allow your workers time to finish what they are working on
- This project implements the "scheduler" part of rescue-scheduler (the daemon which can promote enqueued delayed jobs into the
work queues when it is time), but not the CRON scheduler proxy.  To learn more about how to use a CRON-like scheduler, read the [
Job Schedules](#job-schedules) section of this document.
- If you are using any plugins which effect 'beforeEnqueue' or 'afterEnqueue', be sure to pass the 'jobs' argument to the 'new Queue
' constructor
- If a job fails, it will be added to a special 'failed' queue.  You can then inspect these jobs, write a plugin to manage them,
move them back to the normal queues, etc.  Failure behavior by default is just to enter the 'failed' queue, but there are many options
.  Check out these examples from the ruby ecosystem for inspiration:
  - https://github.com/lantins/resque-retry
  - https://github.com/resque/resque/wiki/Failure-Backends
- If you plan to run more than one worker per nodejs process, be sure to name them something distinct.  Names **must** follow the
 pattern 'hostname:pid+unique_id'.  For example:
...
```

#### <a name="apidoc.element.node-resque.connection.prototype.key"></a>[function <span class="apidocSignatureSpan">node-resque.connection.prototype.</span>key ()](#apidoc.element.node-resque.connection.prototype.key)
- description and source-code
```javascript
key = function (){
  var args;
  args = (arguments.length >= 1 ? [].slice.call(arguments, 0) : []);
  args.unshift(this.options.namespace);
  return args.join(':');
}
```
- example usage
```shell
...
  var self = this;

  if(self.options.redis){
var jobs = [];
self.redis = self.options.redis;

jobs.push(function(done){
  self.redis.set(self.key('connection_test_key'), 'true', done);
});

jobs.push(function(done){
  self.redis.get(self.key('connection_test_key'), function(error, data){
    if(!error && data !== 'true'){ error = new Error('cannot read connection test key'); }
    if(error){
      self.connected = false;
...
```



# <a name="apidoc.module.node-resque.multiWorker"></a>[module node-resque.multiWorker](#apidoc.module.node-resque.multiWorker)

#### <a name="apidoc.element.node-resque.multiWorker.multiWorker"></a>[function <span class="apidocSignatureSpan">node-resque.</span>multiWorker (options, jobs)](#apidoc.element.node-resque.multiWorker.multiWorker)
- description and source-code
```javascript
multiWorker = function (options, jobs){
  var self = this;

  var defaults = self.defaults();
  for(var i in defaults){
    if(options[i] === null || options[i] === undefined){
      options[i] = defaults[i];
    }
  }

  if(options.connection.redis && typeof options.connection.redis.setMaxListeners === 'function'){
    options.connection.redis.setMaxListeners(options.connection.redis.getMaxListeners() + options.maxTaskProcessors);
  }

  self.workers = [];
  self.options = options;
  self.jobs = jobs;
  self.running = false;
  self.working = false;
  self.name = self.options.name;
  self.eventLoopBlocked = true;
  self.eventLoopDelay = Infinity;
  self.eventLoopCheckCounter = 0;

  eventLoopDelay(
    self.options.maxEventLoopDelay,
    self.options.checkTimeout,
  function(blocked, ms){
    self.eventLoopBlocked = blocked;
    self.eventLoopDelay = ms;
    self.eventLoopCheckCounter++;
  });
}
```
- example usage
```shell
...

var connectionDetails = {
pkg:       "ioredis",
host:      "127.0.0.1",
password:  ""
}

var multiWorker = new NR.multiWorker({
connection: connectionDetails,
queues: ['slowQueue'],
minTaskProcessors:   1,
maxTaskProcessors:   100,
checkTimeout:        1000,
maxEventLoopDelay:   10,
toDisconnectProcessors: true,
...
```

#### <a name="apidoc.element.node-resque.multiWorker.super_"></a>[function <span class="apidocSignatureSpan">node-resque.multiWorker.</span>super_ ()](#apidoc.element.node-resque.multiWorker.super_)
- description and source-code
```javascript
function EventEmitter() {
  EventEmitter.init.call(this);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.node-resque.multiWorker.prototype"></a>[module node-resque.multiWorker.prototype](#apidoc.module.node-resque.multiWorker.prototype)

#### <a name="apidoc.element.node-resque.multiWorker.prototype.checkWorkers"></a>[function <span class="apidocSignatureSpan">node-resque.multiWorker.prototype.</span>checkWorkers (callback)](#apidoc.element.node-resque.multiWorker.prototype.checkWorkers)
- description and source-code
```javascript
checkWorkers = function (callback){
  var self = this;
  var verb;
  var workingCount = 0;

  setImmediate(function(){

    self.workers.forEach(function(worker){
      if(worker.working === true){ workingCount++; }
    });

    if(workingCount > 0){
      self.working = true;
    }else{
      self.working = false;
    }

    if(self.running === false && self.workers.length > 0){                                     verb = '--'; }
    else if(self.running === false && self.workers.length === 0){                              verb = 'x';  }
    else if(self.eventLoopBlocked  && self.workers.length > self.options.minTaskProcessors){   verb = '-';  }
    else if(self.eventLoopBlocked  && self.workers.length === self.options.minTaskProcessors){ verb = 'x';  }
    else if(!self.eventLoopBlocked && self.workers.length < self.options.minTaskProcessors){   verb = '+';  }
    else if(
      !self.eventLoopBlocked &&
      self.workers.length < self.options.maxTaskProcessors &&
      (
        self.workers.length === 0 ||
        workingCount / self.workers.length > 0.5
      )
    ){ verb = '+'; }
    else if(
      !self.eventLoopBlocked &&
      self.workers.length > self.options.minTaskProcessors &&
      workingCount / self.workers.length < 0.5
    ){
      verb = '-';
    }
    else{ verb = 'x'; }

    if(verb === 'x'){ return callback(null, verb, self.eventLoopDelay); }

    if(verb === '-'){
      var worker = self.workers.pop();
      worker.end(function(error){
        self.cleanupWorker(worker);
        return callback(error, verb, self.eventLoopDelay);
      });
    }

    if(verb === '--'){
      var jobs = [];

      var stopWorker = function(worker){
        jobs.push(function(done){
          worker.end(function(error){
            if(error){ return done(error); }
            self.cleanupWorker(worker);
            done();
          });
        });
      };

      while(self.workers.length > 0){
        var worker = self.workers.pop();
        stopWorker(worker);
      }

      async.parallel(jobs, function(error){
        self.workers = [];
        callback(error, verb, self.eventLoopDelay);
      });
    }

    if(verb === '+'){
      self.startWorker(function(error){
        callback(error, verb, self.eventLoopDelay);
      });
    }
  });
}
```
- example usage
```shell
...
  worker.connection.end();
}
};

multiWorker.prototype.checkWraper = function(callback){
var self = this;
clearTimeout(self.checkTimer);
self.checkWorkers(function(error, verb, delay){
  if(error){ self.emit('internalError', error); }
  self.emit('multiWorkerAction', verb, delay);
  self.checkTimer = setTimeout(function(){
    self.checkWraper();
  }, self.options.checkTimeout);
  if(typeof callback === 'function'){ callback(); }
});
...
```

#### <a name="apidoc.element.node-resque.multiWorker.prototype.checkWraper"></a>[function <span class="apidocSignatureSpan">node-resque.multiWorker.prototype.</span>checkWraper (callback)](#apidoc.element.node-resque.multiWorker.prototype.checkWraper)
- description and source-code
```javascript
checkWraper = function (callback){
  var self = this;
  clearTimeout(self.checkTimer);
  self.checkWorkers(function(error, verb, delay){
    if(error){ self.emit('internalError', error); }
    self.emit('multiWorkerAction', verb, delay);
    self.checkTimer = setTimeout(function(){
      self.checkWraper();
    }, self.options.checkTimeout);
    if(typeof callback === 'function'){ callback(); }
  });
}
```
- example usage
```shell
...
multiWorker.prototype.checkWraper = function(callback){
var self = this;
clearTimeout(self.checkTimer);
self.checkWorkers(function(error, verb, delay){
  if(error){ self.emit('internalError', error); }
  self.emit('multiWorkerAction', verb, delay);
  self.checkTimer = setTimeout(function(){
    self.checkWraper();
  }, self.options.checkTimeout);
  if(typeof callback === 'function'){ callback(); }
});
};

multiWorker.prototype.start = function(callback){
var self = this;
...
```

#### <a name="apidoc.element.node-resque.multiWorker.prototype.cleanupWorker"></a>[function <span class="apidocSignatureSpan">node-resque.multiWorker.prototype.</span>cleanupWorker (worker)](#apidoc.element.node-resque.multiWorker.prototype.cleanupWorker)
- description and source-code
```javascript
cleanupWorker = function (worker){
  var self = this;

  [
    'start',
    'end',
    'cleaning_worker',
    'poll',
    'job',
    'reEnqueue',
    'success',
    'failure',
    'error',
    'pause',
    'internalError',
    'multiWorkerAction',
  ].forEach(function(e){
    worker.removeAllListeners(e);
  });

  if(self.options.toDisconnectProcessors === true){
    worker.connection.end();
  }
}
```
- example usage
```shell
...
else{ verb = 'x'; }

if(verb === 'x'){ return callback(null, verb, self.eventLoopDelay); }

if(verb === '-'){
  var worker = self.workers.pop();
  worker.end(function(error){
    self.cleanupWorker(worker);
    return callback(error, verb, self.eventLoopDelay);
  });
}

if(verb === '--'){
  var jobs = [];
...
```

#### <a name="apidoc.element.node-resque.multiWorker.prototype.defaults"></a>[function <span class="apidocSignatureSpan">node-resque.multiWorker.prototype.</span>defaults ()](#apidoc.element.node-resque.multiWorker.prototype.defaults)
- description and source-code
```javascript
defaults = function (){
  var self = this;
  // all times in ms
  return {
    minTaskProcessors:   1,
    maxTaskProcessors:   10,
    timeout:             5000,
    checkTimeout:        500,
    maxEventLoopDelay:   10,
    toDisconnectProcessors: true,
    name: os.hostname()
  };
}
```
- example usage
```shell
...

var util  = require('util');
var async = require('async');
var EventEmitter = require('events').EventEmitter;

var connection = function(options){
var self = this;
var defaults = self.defaults();

if(!options){ options = {}; }
for(var i in defaults){
  if(options[i] === null || options[i] === undefined){
    options[i] = defaults[i];
  }
}
...
```

#### <a name="apidoc.element.node-resque.multiWorker.prototype.end"></a>[function <span class="apidocSignatureSpan">node-resque.multiWorker.prototype.</span>end (callback)](#apidoc.element.node-resque.multiWorker.prototype.end)
- description and source-code
```javascript
end = function (callback){
  var self = this;
  self.stop(callback);
}
```
- example usage
```shell
...

worker.connect(function(){
  worker.start();
});
'''

## Notes
- Be sure to call 'worker.end(callback)', 'queue.end(callback)' and 'scheduler.end(callback)' before shutting down your application
 if you want to properly clear your worker status from resque
- When ending your application, be sure to allow your workers time to finish what they are working on
- This project implements the "scheduler" part of rescue-scheduler (the daemon which can promote enqueued delayed jobs into the
work queues when it is time), but not the CRON scheduler proxy.  To learn more about how to use a CRON-like scheduler, read the [
Job Schedules](#job-schedules) section of this document.
- If you are using any plugins which effect 'beforeEnqueue' or 'afterEnqueue', be sure to pass the 'jobs' argument to the 'new Queue
' constructor
- If a job fails, it will be added to a special 'failed' queue.  You can then inspect these jobs, write a plugin to manage them,
move them back to the normal queues, etc.  Failure behavior by default is just to enter the 'failed' queue, but there are many options
.  Check out these examples from the ruby ecosystem for inspiration:
  - https://github.com/lantins/resque-retry
  - https://github.com/resque/resque/wiki/Failure-Backends
- If you plan to run more than one worker per nodejs process, be sure to name them something distinct.  Names **must** follow the
 pattern 'hostname:pid+unique_id'.  For example:
...
```

#### <a name="apidoc.element.node-resque.multiWorker.prototype.start"></a>[function <span class="apidocSignatureSpan">node-resque.multiWorker.prototype.</span>start (callback)](#apidoc.element.node-resque.multiWorker.prototype.start)
- description and source-code
```javascript
start = function (callback){
  var self = this;
  self.running = true;
  self.checkWraper(function(){
    if(typeof callback === 'function'){ callback(); }
  });
}
```
- example usage
```shell
...
////////////////////
// START A WORKER //
////////////////////

var worker = new NR.worker({connection: connectionDetails, queues: ['math', 'otherQueue']}, jobs);
worker.connect(function(){
  worker.workerCleanup(); // optional: cleanup any previous improperly shutdown workers on this host
  worker.start();
});

///////////////////////
// START A SCHEDULER //
///////////////////////

var scheduler = new NR.scheduler({connection: connectionDetails});
...
```

#### <a name="apidoc.element.node-resque.multiWorker.prototype.startWorker"></a>[function <span class="apidocSignatureSpan">node-resque.multiWorker.prototype.</span>startWorker (callback)](#apidoc.element.node-resque.multiWorker.prototype.startWorker)
- description and source-code
```javascript
startWorker = function (callback){
  var self = this;
  var id = (self.workers.length + 1);
  var worker = new Worker({
    connection: self.options.connection,
    queues:     self.options.queues,
    timeout:    self.options.timeout,
    name:       self.options.name + ':' + process.pid + '+' + id
  }, self.jobs);
  worker.connect(function(error){
    if(error){ self.emit('error', error); }
    worker.workerCleanup(function(error){
      worker.start();
      if(error){ self.emit('error', error); }
      process.nextTick(callback);
    });
  });

  worker.id = id;

  worker.on('start',           function(){                    self.emit('start', worker.id);                         });
  worker.on('end',             function(){                    self.emit('end', worker.id);                           });
  worker.on('cleaning_worker', function(worker, pid){         self.emit('cleaning_worker', worker.id, worker, pid);  });
  worker.on('poll',            function(queue){               self.emit('poll', worker.id, queue);                   });
  worker.on('job',             function(queue, job){          self.emit('job', worker.id, queue, job);               });
  worker.on('reEnqueue',       function(queue, job, plugin){  self.emit('reEnqueue', worker.id, queue, job, plugin); });
  worker.on('success',         function(queue, job, result){  self.emit('success', worker.id, queue, job, result);   });
  worker.on('failure',         function(queue, job, failure){ self.emit('failure', worker.id, queue, job, failure);  });
  worker.on('error',           function(queue, job, error){   self.emit('error', worker.id, queue, job, error);      });
  worker.on('pause',           function(){                    self.emit('pause', worker.id);                         });

  self.workers.push(worker);
}
```
- example usage
```shell
...
      async.parallel(jobs, function(error){
        self.workers = [];
        callback(error, verb, self.eventLoopDelay);
      });
    }

    if(verb === '+'){
      self.startWorker(function(error){
        callback(error, verb, self.eventLoopDelay);
      });
    }
  });
};

multiWorker.prototype.cleanupWorker = function(worker){
...
```

#### <a name="apidoc.element.node-resque.multiWorker.prototype.stop"></a>[function <span class="apidocSignatureSpan">node-resque.multiWorker.prototype.</span>stop (callback)](#apidoc.element.node-resque.multiWorker.prototype.stop)
- description and source-code
```javascript
stop = function (callback){
  var self = this;
  self.running = false;
  self.stopWait(callback);
}
```
- example usage
```shell
...
var self = this;
self.running = false;
self.stopWait(callback);
};

multiWorker.prototype.end = function(callback){
var self = this;
self.stop(callback);
};

multiWorker.prototype.stopWait = function(callback){
var self = this;
if(self.workers.length === 0 && self.working === false){
  clearTimeout(self.checkTimer);
  process.nextTick(function(){
...
```

#### <a name="apidoc.element.node-resque.multiWorker.prototype.stopWait"></a>[function <span class="apidocSignatureSpan">node-resque.multiWorker.prototype.</span>stopWait (callback)](#apidoc.element.node-resque.multiWorker.prototype.stopWait)
- description and source-code
```javascript
stopWait = function (callback){
  var self = this;
  if(self.workers.length === 0 && self.working === false){
    clearTimeout(self.checkTimer);
    process.nextTick(function(){
      if(typeof callback === 'function'){ callback(); }
    });
  }else{
    setTimeout(function(){
      self.stopWait(callback);
    }, self.options.checkTimeout);
  }
}
```
- example usage
```shell
...
    if(typeof callback === 'function'){ callback(); }
  });
};

multiWorker.prototype.stop = function(callback){
  var self = this;
  self.running = false;
  self.stopWait(callback);
};

multiWorker.prototype.end = function(callback){
  var self = this;
  self.stop(callback);
};
...
```



# <a name="apidoc.module.node-resque.pluginRunner"></a>[module node-resque.pluginRunner](#apidoc.module.node-resque.pluginRunner)

#### <a name="apidoc.element.node-resque.pluginRunner.runPlugin"></a>[function <span class="apidocSignatureSpan">node-resque.pluginRunner.</span>runPlugin (self, pluginRefrence, type, func, queue, job, args, callback)](#apidoc.element.node-resque.pluginRunner.runPlugin)
- description and source-code
```javascript
runPlugin = function (self, pluginRefrence, type, func, queue, job, args, callback){
  process.nextTick(function(){
    if(!job){
      callback(null, true);
    }else{

      var pluginName = pluginRefrence;
      if(typeof pluginRefrence === 'function'){
        pluginName = new pluginRefrence(self, func, queue, job, args, {}).name;
      }

      var pluginOptions = null;
      if(self.jobs[func].pluginOptions && self.jobs[func].pluginOptions[pluginName]){
        pluginOptions = self.jobs[func].pluginOptions[pluginName];
      }else{
        pluginOptions = {};
      }

      var plugin = null;
      if(typeof pluginRefrence === 'string'){
        var pluginConstructor = require(__dirname + '/plugins/' + pluginRefrence + '.js')[pluginRefrence];
        plugin = new pluginConstructor(self, func, queue, job, args, pluginOptions);
      }else if(typeof pluginRefrence === 'function'){
        plugin = new pluginRefrence(self, func, queue, job, args, pluginOptions);
      }else{
        throw new Error('Plugin must be the constructor name or an object');
      }

      if(plugin[type] === null || plugin[type] === undefined  || typeof plugin[type] !== 'function'){
        callback(null, true);
      }else{
        plugin[type](function(err, toRun){
          callback(err, toRun);
        });
      }
    }
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-resque.pluginRunner.runPlugins"></a>[function <span class="apidocSignatureSpan">node-resque.pluginRunner.</span>runPlugins (self, type, func, queue, job, args, callback, pluginCounter)](#apidoc.element.node-resque.pluginRunner.runPlugins)
- description and source-code
```javascript
runPlugins = function (self, type, func, queue, job, args, callback, pluginCounter){
  if(!pluginCounter){ pluginCounter = 0; }
  if(!job){
    callback(null, true);
  }else if(job.plugins === null || job.plugins === undefined || job.plugins.length === 0){
    callback(null, true);
  }else if(pluginCounter >= job.plugins.length){
    callback(null, true);
  }else{
    var pluginRefrence = job.plugins[pluginCounter];
    runPlugin(self, pluginRefrence, type, func, queue, job, args, function(err, toRun){
      pluginCounter++;
      if(err){
        callback(err, toRun);
      }else if(toRun === false){
        callback(err, false);
      }else{
        runPlugins(self, type, func, queue, job, args, callback, pluginCounter);
      }
    });
  }
}
```
- example usage
```shell
...
  }else if(arguments.length < 3){
args = [];
  }

  args = arrayify(args);
  var job = self.jobs[func];

  pluginRunner.runPlugins(self, 'before_enqueue', func, q, job, args, function(error, toRun){
if(error){ return callback(error); }
if(toRun === false){ return callback(error, toRun); }

jobs.push(function(done){
  self.connection.redis.sadd(self.connection.key('queues'), q, done);
});
...
```



# <a name="apidoc.module.node-resque.queue"></a>[module node-resque.queue](#apidoc.module.node-resque.queue)

#### <a name="apidoc.element.node-resque.queue.queue"></a>[function <span class="apidocSignatureSpan">node-resque.</span>queue (options, jobs)](#apidoc.element.node-resque.queue.queue)
- description and source-code
```javascript
queue = function (options, jobs){
  var self = this;
  if(!jobs){ jobs = {}; }

  self.options = options;
  self.jobs    = jobs;

  self.connection = new connection(options.connection);

  self.connection.on('error', function(error){
    self.emit('error', error);
  });
}
```
- example usage
```shell
...
scheduler.on('working_timestamp', function(timestamp){ console.log("scheduler working timestamp " + timestamp); });
scheduler.on('transferred_job',   function(timestamp, job){ console.log("scheduler enquing job " + timestamp + " >> " + JSON.stringify
(job)); });

////////////////////////
// CONNECT TO A QUEUE //
////////////////////////

var queue = new NR.queue({connection: connectionDetails}, jobs);
queue.on('error', function(error){ console.log(error); });
queue.connect(function(){
  queue.enqueue('math', "add", [1,2]);
  queue.enqueue('math', "add", [1,2]);
  queue.enqueue('math', "add", [2,3]);
  queue.enqueueIn(3000, 'math', "subtract", [2,1]);
});
...
```

#### <a name="apidoc.element.node-resque.queue.super_"></a>[function <span class="apidocSignatureSpan">node-resque.queue.</span>super_ ()](#apidoc.element.node-resque.queue.super_)
- description and source-code
```javascript
function EventEmitter() {
  EventEmitter.init.call(this);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.node-resque.queue.prototype"></a>[module node-resque.queue.prototype](#apidoc.module.node-resque.queue.prototype)

#### <a name="apidoc.element.node-resque.queue.prototype.allDelayed"></a>[function <span class="apidocSignatureSpan">node-resque.queue.prototype.</span>allDelayed (callback)](#apidoc.element.node-resque.queue.prototype.allDelayed)
- description and source-code
```javascript
allDelayed = function (callback){
  var self = this;
  var results = {};
  var jobs = [];

  self.timestamps(function(error, timestamps){
    if(error){ return callback(error); }

    timestamps.forEach(function(timestamp){
      jobs.push(function(done){
        self.delayedAt(timestamp, function(error, tasks, rTimestamp){
          if(error){ return done(error); }
          results[(rTimestamp * 1000)] = tasks;
          done();
        });
      });
    });

    async.series(jobs, function(error){
      return callback(error, results);
    });
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-resque.queue.prototype.allWorkingOn"></a>[function <span class="apidocSignatureSpan">node-resque.queue.prototype.</span>allWorkingOn (callback)](#apidoc.element.node-resque.queue.prototype.allWorkingOn)
- description and source-code
```javascript
allWorkingOn = function (callback){
  var self = this;
  var results = {};
  var jobs = [];

  self.workers(function(error, workers){
    if(error){ return callback(error); }

    Object.keys(workers).forEach(function(w){
      jobs.push(function(done){
        results[w] = 'started';
        self.workingOn(w, workers[w], function(error, data){
          if(error){ return done(error); }
          if(data){
            data = JSON.parse(data);
            results[data.worker] = data;
          }
          done();
        });
      });
    });

    async.series(jobs, function(error){
      return callback(error, results);
    });
  });
}
```
- example usage
```shell
...
  // note: this method will remove the data created by a 'stuck' worker and move the payload to the error queue
  // however, it will not actually remove any processes which may be running.  A job *may* be running that you have removed

  var self = this;
  var results = {};
  var jobs = [];

  self.allWorkingOn(function(error, data){
if(error){ return callback(error); }

Object.keys(data).forEach(function(workerName){
  jobs.push(function(done){
    if(Date.now() - Date.parse(data[workerName].run_at) > age){
      self.forceCleanWorker(workerName, function(error, errorPayload){
        if(errorPayload && errorPayload.worker){ results[errorPayload.worker] = errorPayload; }
...
```

#### <a name="apidoc.element.node-resque.queue.prototype.cleanOldWorkers"></a>[function <span class="apidocSignatureSpan">node-resque.queue.prototype.</span>cleanOldWorkers (age, callback)](#apidoc.element.node-resque.queue.prototype.cleanOldWorkers)
- description and source-code
```javascript
cleanOldWorkers = function (age, callback){
  // note: this method will remove the data created by a 'stuck' worker and move the payload to the error queue
  // however, it will not actually remove any processes which may be running.  A job *may* be running that you have removed

  var self = this;
  var results = {};
  var jobs = [];

  self.allWorkingOn(function(error, data){
    if(error){ return callback(error); }

    Object.keys(data).forEach(function(workerName){
      jobs.push(function(done){
        if(Date.now() - Date.parse(data[workerName].run_at) > age){
          self.forceCleanWorker(workerName, function(error, errorPayload){
            if(errorPayload && errorPayload.worker){ results[errorPayload.worker] = errorPayload; }
            done(error);
          });
        }else{
          done();
        }
      });
    });

    async.series(jobs, function(error){
      return callback(error, results);
    });
  });
}
```
- example usage
```shell
...
- **queue.retryAndRemoveFailed** = function(failedJob, callback)
  - callback(error)
  - the input 'failedJob' is an expanded node object representing the failed job, retrieved via 'queue.failed'
  - this method will instantly re-enqueue a failed job back to its original queue, and delete the failed entry for that job

## Failed Worker Management

Sometimes a worker crashes is a *severe* way, and it doesn't get the time/chance to notify redis that it is leaving the pool (this
 happens all the time on PAAS providers like Heroku).  When this happens, you will not only need to extract the job from the now
-zombie worker's "working on" status, but also remove the stuck worker.  To aid you in these edge cases, ''queue.cleanOldWorkers
(age, callback)' is available.

Because there are no 'heartbeats' in resque, it is imposable for the application to know if a worker has been working on a long
job or it is dead.  You are required to provide an "age" for how long a worker has been "working", and all those older than that
 age will be removed, and the job they are working on moved to the error queue (where you can then use 'queue.retryAndRemoveFailed
') to re-enqueue the job.

If you know the name of a worker that should be removed, you can also call 'queue.forceCleanWorker(workerName, callback)' directly
, and that will also remove the worker and move any job it was working on into the error queue.

## Job Schedules
...
```

#### <a name="apidoc.element.node-resque.queue.prototype.connect"></a>[function <span class="apidocSignatureSpan">node-resque.queue.prototype.</span>connect (callback)](#apidoc.element.node-resque.queue.prototype.connect)
- description and source-code
```javascript
connect = function (callback){
  var self = this;
  self.connection.connect(callback);
}
```
- example usage
```shell
...
};

////////////////////
// START A WORKER //
////////////////////

var worker = new NR.worker({connection: connectionDetails, queues: ['math', 'otherQueue']}, jobs);
worker.connect(function(){
  worker.workerCleanup(); // optional: cleanup any previous improperly shutdown workers on this host
  worker.start();
});

///////////////////////
// START A SCHEDULER //
///////////////////////
...
```

#### <a name="apidoc.element.node-resque.queue.prototype.del"></a>[function <span class="apidocSignatureSpan">node-resque.queue.prototype.</span>del (q, func, args, count, callback)](#apidoc.element.node-resque.queue.prototype.del)
- description and source-code
```javascript
del = function (q, func, args, count, callback){
  var self = this;

  if(typeof count === 'function' && callback === undefined){
    callback = count;
    count = 0;
  }else if(arguments.length === 3){
    if(typeof args === 'function'){
      callback = args;
      args = [];
    }
    count = 0;
  }else if(arguments.length < 3){
    args = [];
    count = 0;
  }

  args = arrayify(args);
  self.connection.redis.lrem(self.connection.key('queue', q), count, self.encode(q, func, args), callback);
}
```
- example usage
```shell
...
queue.prototype.queues = function(callback){
var self = this;
self.connection.redis.smembers(self.connection.key('queues'), callback);
};

queue.prototype.delQueue = function(q, callback){
var self = this;
self.connection.redis.del(self.connection.key('queue', q), function(error){
  if(error){ return callback(error); }
  self.connection.redis.srem(self.connection.key('queues'), q, callback);
});
};

queue.prototype.length = function(q, callback){
var self = this;
...
```

#### <a name="apidoc.element.node-resque.queue.prototype.delDelayed"></a>[function <span class="apidocSignatureSpan">node-resque.queue.prototype.</span>delDelayed (q, func, args, callback)](#apidoc.element.node-resque.queue.prototype.delDelayed)
- description and source-code
```javascript
delDelayed = function (q, func, args, callback){
  var self = this;
  var jobs = [];
  var timestamps = [];

  if(arguments.length === 3 && typeof args === 'function'){
    callback = args;
    args = [];
  }else if(arguments.length < 3){
    args = [];
  }

  args = arrayify(args);
  var search = self.encode(q, func, args);
  var timestamps = [];
  self.connection.redis.smembers(self.connection.key('timestamps:' + search), function(error, members){
    if(error){ return callback(error); }

    members.forEach(function(key){
      jobs.push(function(done){
        self.connection.redis.lrem(self.connection.key(key), 0, search, function(error, count){
          if(error){ return done(error); }
          if(count > 0){
            timestamps.push(key.split(':')[key.split(':').length - 1]);
            self.connection.redis.srem(self.connection.key('timestamps:' + search), key, done);
          }else{
            done();
          }
        });
      });
    });

    async.series(jobs, function(error){
      return callback(error, timestamps);
    });
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-resque.queue.prototype.delLock"></a>[function <span class="apidocSignatureSpan">node-resque.queue.prototype.</span>delLock (key, callback)](#apidoc.element.node-resque.queue.prototype.delLock)
- description and source-code
```javascript
delLock = function (key, callback){
  var self = this;
  self.connection.redis.del(self.connection.key(key), callback);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-resque.queue.prototype.delQueue"></a>[function <span class="apidocSignatureSpan">node-resque.queue.prototype.</span>delQueue (q, callback)](#apidoc.element.node-resque.queue.prototype.delQueue)
- description and source-code
```javascript
delQueue = function (q, callback){
  var self = this;
  self.connection.redis.del(self.connection.key('queue', q), function(error){
    if(error){ return callback(error); }
    self.connection.redis.srem(self.connection.key('queues'), q, callback);
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-resque.queue.prototype.delayedAt"></a>[function <span class="apidocSignatureSpan">node-resque.queue.prototype.</span>delayedAt (timestamp, callback)](#apidoc.element.node-resque.queue.prototype.delayedAt)
- description and source-code
```javascript
delayedAt = function (timestamp, callback){
  var self = this;
  var rTimestamp = Math.round(timestamp / 1000); // assume timestamp is in ms
  self.connection.redis.lrange(self.connection.key('delayed:' + rTimestamp), 0, -1, function(error, items){
    var tasks = items.map(function(i){ return JSON.parse(i); });
    callback(error, tasks, rTimestamp);
  });
}
```
- example usage
```shell
...
  var jobs = [];

  self.timestamps(function(error, timestamps){
if(error){ return callback(error); }

timestamps.forEach(function(timestamp){
  jobs.push(function(done){
    self.delayedAt(timestamp, function(error, tasks, rTimestamp){
      if(error){ return done(error); }
      results[(rTimestamp * 1000)] = tasks;
      done();
    });
  });
});
...
```

#### <a name="apidoc.element.node-resque.queue.prototype.encode"></a>[function <span class="apidocSignatureSpan">node-resque.queue.prototype.</span>encode (q, func, args)](#apidoc.element.node-resque.queue.prototype.encode)
- description and source-code
```javascript
encode = function (q, func, args){
  return JSON.stringify({
    'class': func,
    queue: q,
    args: args || []
  });
}
```
- example usage
```shell
...
if(toRun === false){ return callback(error, toRun); }

jobs.push(function(done){
  self.connection.redis.sadd(self.connection.key('queues'), q, done);
});

jobs.push(function(done){
  self.connection.redis.rpush(self.connection.key('queue', q), self.encode(q, func, args), done);
});

jobs.push(function(done){
  pluginRunner.runPlugins(self, 'after_enqueue', func, q, job, args, done);
});

async.series(jobs, callback);
...
```

#### <a name="apidoc.element.node-resque.queue.prototype.end"></a>[function <span class="apidocSignatureSpan">node-resque.queue.prototype.</span>end (callback)](#apidoc.element.node-resque.queue.prototype.end)
- description and source-code
```javascript
end = function (callback){
  var self = this;
  self.connection.end();
  return callback();
}
```
- example usage
```shell
...

worker.connect(function(){
  worker.start();
});
'''

## Notes
- Be sure to call 'worker.end(callback)', 'queue.end(callback)' and 'scheduler.end(callback)' before shutting down your application
 if you want to properly clear your worker status from resque
- When ending your application, be sure to allow your workers time to finish what they are working on
- This project implements the "scheduler" part of rescue-scheduler (the daemon which can promote enqueued delayed jobs into the
work queues when it is time), but not the CRON scheduler proxy.  To learn more about how to use a CRON-like scheduler, read the [
Job Schedules](#job-schedules) section of this document.
- If you are using any plugins which effect 'beforeEnqueue' or 'afterEnqueue', be sure to pass the 'jobs' argument to the 'new Queue
' constructor
- If a job fails, it will be added to a special 'failed' queue.  You can then inspect these jobs, write a plugin to manage them,
move them back to the normal queues, etc.  Failure behavior by default is just to enter the 'failed' queue, but there are many options
.  Check out these examples from the ruby ecosystem for inspiration:
  - https://github.com/lantins/resque-retry
  - https://github.com/resque/resque/wiki/Failure-Backends
- If you plan to run more than one worker per nodejs process, be sure to name them something distinct.  Names **must** follow the
 pattern 'hostname:pid+unique_id'.  For example:
...
```

#### <a name="apidoc.element.node-resque.queue.prototype.enqueue"></a>[function <span class="apidocSignatureSpan">node-resque.queue.prototype.</span>enqueue (q, func, args, callback)](#apidoc.element.node-resque.queue.prototype.enqueue)
- description and source-code
```javascript
enqueue = function (q, func, args, callback){
  var self = this;
  var jobs = [];
  if(arguments.length === 3 && typeof args === 'function'){
    callback = args;
    args = [];
  }else if(arguments.length < 3){
    args = [];
  }

  args = arrayify(args);
  var job = self.jobs[func];

  pluginRunner.runPlugins(self, 'before_enqueue', func, q, job, args, function(error, toRun){
    if(error){ return callback(error); }
    if(toRun === false){ return callback(error, toRun); }

    jobs.push(function(done){
      self.connection.redis.sadd(self.connection.key('queues'), q, done);
    });

    jobs.push(function(done){
      self.connection.redis.rpush(self.connection.key('queue', q), self.encode(q, func, args), done);
    });

    jobs.push(function(done){
      pluginRunner.runPlugins(self, 'after_enqueue', func, q, job, args, done);
    });

    async.series(jobs, callback);
  });
}
```
- example usage
```shell
...
////////////////////////
// CONNECT TO A QUEUE //
////////////////////////

var queue = new NR.queue({connection: connectionDetails}, jobs);
queue.on('error', function(error){ console.log(error); });
queue.connect(function(){
  queue.enqueue('math', "add", [1,2]);
  queue.enqueue('math', "add", [1,2]);
  queue.enqueue('math', "add", [2,3]);
  queue.enqueueIn(3000, 'math', "subtract", [2,1]);
});

'''
...
```

#### <a name="apidoc.element.node-resque.queue.prototype.enqueueAt"></a>[function <span class="apidocSignatureSpan">node-resque.queue.prototype.</span>enqueueAt (timestamp, q, func, args, callback)](#apidoc.element.node-resque.queue.prototype.enqueueAt)
- description and source-code
```javascript
enqueueAt = function (timestamp, q, func, args, callback){
  // Don't run plugins here, they should be run by scheduler at the enqueue step
  var self = this;
  var jobs = [];

  if(arguments.length === 4 && typeof args === 'function'){
    callback = args;
    args = [];
  }else if(arguments.length < 4){
    args = [];
  }

  args = arrayify(args);
  var item = self.encode(q, func, args);
  var rTimestamp = Math.round(timestamp / 1000); // assume timestamp is in ms

  jobs.push(function(done){
    // check if this jobs is already enqueued at this time
    var match = ('delayed:' + rTimestamp);
    self.connection.redis.smembers(self.connection.key('timestamps:' + item), function(error, members){
      for(var i in members){
        if(members[i] === match){
          return done(new Error('Job already enqueued at this time with same arguments'));
        }
      }

      done(error);
    });
  });

  jobs.push(function(done){
    // enqueue the encoded job into a list per timestmp to be popped and workered later
    self.connection.redis.rpush(self.connection.key('delayed:' + rTimestamp), item, done);
  });

  jobs.push(function(done){
    // save the job + args into a set so that it can be checked by plugins
    self.connection.redis.sadd(self.connection.key('timestamps:' + item), ('delayed:' + rTimestamp), done);
  });

  jobs.push(function(done){
    self.connection.redis.zadd(self.connection.key('delayed_queue_schedule'), rTimestamp, rTimestamp, done);
  });

  async.series(jobs, callback);
}
```
- example usage
```shell
...
    args = [];
  }else if(arguments.length < 4){
    args = [];
  }

  args = arrayify(args);
  var timestamp = (new Date().getTime()) + parseInt(time, 10);
  self.enqueueAt(timestamp, q, func, args, callback);
};

queue.prototype.queues = function(callback){
  var self = this;
  self.connection.redis.smembers(self.connection.key('queues'), callback);
};
...
```

#### <a name="apidoc.element.node-resque.queue.prototype.enqueueIn"></a>[function <span class="apidocSignatureSpan">node-resque.queue.prototype.</span>enqueueIn (time, q, func, args, callback)](#apidoc.element.node-resque.queue.prototype.enqueueIn)
- description and source-code
```javascript
enqueueIn = function (time, q, func, args, callback){
  var self = this;

  if(arguments.length === 4 && typeof args === 'function'){
    callback = args;
    args = [];
  }else if(arguments.length < 4){
    args = [];
  }

  args = arrayify(args);
  var timestamp = (new Date().getTime()) + parseInt(time, 10);
  self.enqueueAt(timestamp, q, func, args, callback);
}
```
- example usage
```shell
...

var queue = new NR.queue({connection: connectionDetails}, jobs);
queue.on('error', function(error){ console.log(error); });
queue.connect(function(){
  queue.enqueue('math', "add", [1,2]);
  queue.enqueue('math', "add", [1,2]);
  queue.enqueue('math', "add", [2,3]);
  queue.enqueueIn(3000, 'math', "subtract", [2,1]);
});

'''

## Configuration Options:

'new queue' requires only the "queue" variable to be set.  You can also pass the 'jobs' hash to it.
...
```

#### <a name="apidoc.element.node-resque.queue.prototype.failed"></a>[function <span class="apidocSignatureSpan">node-resque.queue.prototype.</span>failed (start, stop, callback)](#apidoc.element.node-resque.queue.prototype.failed)
- description and source-code
```javascript
failed = function (start, stop, callback){
  var self = this;
  self.connection.redis.lrange(self.connection.key('failed'), start, stop, function(error, data){
    var results = data.map(function(i){ return JSON.parse(i); });
    callback(error, results);
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-resque.queue.prototype.failedCount"></a>[function <span class="apidocSignatureSpan">node-resque.queue.prototype.</span>failedCount (callback)](#apidoc.element.node-resque.queue.prototype.failedCount)
- description and source-code
```javascript
failedCount = function (callback){
  var self = this;
  self.connection.redis.llen(self.connection.key('failed'), callback);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-resque.queue.prototype.forceCleanWorker"></a>[function <span class="apidocSignatureSpan">node-resque.queue.prototype.</span>forceCleanWorker (workerName, callback)](#apidoc.element.node-resque.queue.prototype.forceCleanWorker)
- description and source-code
```javascript
forceCleanWorker = function (workerName, callback){
  var self = this;
  var errorPayload;
  var jobs = [];

  self.workers(function(error, workers){
    if(error){ return callback(error); }
    var queues = workers[workerName];
    if(!queues){ return callback(new Error('worker not round')); }

    self.workingOn(workerName, queues, function(error, workingOn){
      if(error){ return callback(error); }
      if(workingOn){
        workingOn = JSON.parse(workingOn);
        errorPayload = {
          worker: workerName,
          queue: workingOn.queue,
          payload: workingOn.payload,
          exception: 'Worker Timeout (killed manually)',
          error: 'Worker Timeout (killed manually)',
          backtrace: null,
          failed_at: (new Date()).toString()
        };

        jobs.push(function(done){
          self.connection.redis.incr(self.connection.key('stat', 'failed'), done);
        });

        jobs.push(function(done){
          self.connection.redis.incr(self.connection.key('stat', 'failed', workerName), done);
        });

        jobs.push(function(done){
          self.connection.redis.rpush(self.connection.key('failed'), JSON.stringify(errorPayload), done);
        });
      }

      jobs.push(function(done){
        self.connection.redis.del(self.connection.key('stat', 'failed', workerName), done);
      });

      jobs.push(function(done){
        self.connection.redis.del(self.connection.key('stat', 'processed', workerName), done);
      });

      jobs.push(function(done){
        self.connection.redis.del(self.connection.key('worker', workerName), done);
      });

      jobs.push(function(done){
        self.connection.redis.srem(self.connection.key('workers'), workerName + ':' + queues, done);
      });

      async.series(jobs, function(error){
        return callback(error, errorPayload);
      });
    });
  });
}
```
- example usage
```shell
...

## Failed Worker Management

Sometimes a worker crashes is a *severe* way, and it doesn't get the time/chance to notify redis that it is leaving the pool (this
 happens all the time on PAAS providers like Heroku).  When this happens, you will not only need to extract the job from the now
-zombie worker's "working on" status, but also remove the stuck worker.  To aid you in these edge cases, ''queue.cleanOldWorkers
(age, callback)' is available.

Because there are no 'heartbeats' in resque, it is imposable for the application to know if a worker has been working on a long
job or it is dead.  You are required to provide an "age" for how long a worker has been "working", and all those older than that
 age will be removed, and the job they are working on moved to the error queue (where you can then use 'queue.retryAndRemoveFailed
') to re-enqueue the job.

If you know the name of a worker that should be removed, you can also call 'queue.forceCleanWorker(workerName, callback)' directly
, and that will also remove the worker and move any job it was working on into the error queue.

## Job Schedules

You may want to use node-resque to schedule jobs every minute/hour/day, like a distributed CRON system.  There are a number of excellent
 node packages to help you with this, like [node-schedule](https://github.com/tejasmanohar/node-schedule) and [node-cron](https://
github.com/ncb000gt/node-cron).  Node-resque makes it possible for you to use the package of your choice to schedule jobs with.

Assuming you are running node-resque across multiple machines, you will need to ensure that only one of your processes is actually
 scheduling the jobs.  To help you with this, you can inspect which of the scheduler processes is currently acting as master, and
 flag only the master scheduler process to run the schedule.  A full example can be found at [/examples/scheduledJobs.js](https://
github.com/taskrabbit/node-resque/blob/master/examples/scheduledJobs.js), but the relevant section is:
...
```

#### <a name="apidoc.element.node-resque.queue.prototype.length"></a>[function <span class="apidocSignatureSpan">node-resque.queue.prototype.</span>length (q, callback)](#apidoc.element.node-resque.queue.prototype.length)
- description and source-code
```javascript
length = function (q, callback){
  var self = this;
  self.connection.redis.llen(self.connection.key('queue', q), callback);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-resque.queue.prototype.locks"></a>[function <span class="apidocSignatureSpan">node-resque.queue.prototype.</span>locks (callback)](#apidoc.element.node-resque.queue.prototype.locks)
- description and source-code
```javascript
locks = function (callback){
  var self = this;
  var keys = [];
  var data = {};
  var jobs = [];

  jobs.push(function(done){
    self.connection.redis.keys(self.connection.key('lock:*'), function(error, _keys){
      if(error){ return done(error); }
      keys = keys.concat(_keys);
      done();
    });
  });

  jobs.push(function(done){
    self.connection.redis.keys(self.connection.key('workerslock:*'), function(error, _keys){
      if(error){ return done(error); }
      keys = keys.concat(_keys);
      done();
    });
  });

  async.parallel(jobs, function(error){
    if(error){ return callback(error); }
    if(keys.length === 0){ return callback(null, data); }

    self.connection.redis.mget(keys, function(error, values){
      if(error){ return callback(error); }

      for(var i = 0; i < keys.length; i++){
        var k = keys[i];
        k = k.replace(self.connection.key(''), '');
        data[k] = values[i];
      }

      callback(null, data);
    });
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-resque.queue.prototype.queued"></a>[function <span class="apidocSignatureSpan">node-resque.queue.prototype.</span>queued (q, start, stop, callback)](#apidoc.element.node-resque.queue.prototype.queued)
- description and source-code
```javascript
queued = function (q, start, stop, callback){
  var self = this;
  self.connection.redis.lrange(self.connection.key('queue', q), start, stop, function(error, items){
    var tasks = items.map(function(i){ return JSON.parse(i); });
    callback(error, tasks);
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-resque.queue.prototype.queues"></a>[function <span class="apidocSignatureSpan">node-resque.queue.prototype.</span>queues (callback)](#apidoc.element.node-resque.queue.prototype.queues)
- description and source-code
```javascript
queues = function (callback){
  var self = this;
  self.connection.redis.smembers(self.connection.key('queues'), callback);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-resque.queue.prototype.removeFailed"></a>[function <span class="apidocSignatureSpan">node-resque.queue.prototype.</span>removeFailed (failedJob, callback)](#apidoc.element.node-resque.queue.prototype.removeFailed)
- description and source-code
```javascript
removeFailed = function (failedJob, callback){
  var self = this;
  self.connection.redis.lrem(self.connection.key('failed'), 1, JSON.stringify(failedJob), callback);
}
```
- example usage
```shell
...
queue.prototype.removeFailed = function(failedJob, callback){
  var self = this;
  self.connection.redis.lrem(self.connection.key('failed'), 1, JSON.stringify(failedJob), callback);
};

queue.prototype.retryAndRemoveFailed = function(failedJob, callback){
  var self = this;
  self.removeFailed(failedJob, function(error, countFailed){
    if(error){ return callback(error, failedJob); }
    if(countFailed < 1){ return callback(new Error('This job is not in failed queue'), failedJob); }
    self.enqueue(failedJob.queue, failedJob.payload['class'], failedJob.payload.args, callback);
  });
};

queue.prototype.stats = function(callback){
...
```

#### <a name="apidoc.element.node-resque.queue.prototype.retryAndRemoveFailed"></a>[function <span class="apidocSignatureSpan">node-resque.queue.prototype.</span>retryAndRemoveFailed (failedJob, callback)](#apidoc.element.node-resque.queue.prototype.retryAndRemoveFailed)
- description and source-code
```javascript
retryAndRemoveFailed = function (failedJob, callback){
  var self = this;
  self.removeFailed(failedJob, function(error, countFailed){
    if(error){ return callback(error, failedJob); }
    if(countFailed < 1){ return callback(new Error('This job is not in failed queue'), failedJob); }
    self.enqueue(failedJob.queue, failedJob.payload['class'], failedJob.payload.args, callback);
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-resque.queue.prototype.scheduledAt"></a>[function <span class="apidocSignatureSpan">node-resque.queue.prototype.</span>scheduledAt (q, func, args, callback)](#apidoc.element.node-resque.queue.prototype.scheduledAt)
- description and source-code
```javascript
scheduledAt = function (q, func, args, callback){
  var self = this;
  var timestamps = [];

  if(arguments.length === 3 && typeof args === 'function'){
    callback = args;
    args = [];
  }else if(arguments.length < 3){
    args = [];
  }
  args = arrayify(args);
  var search = self.encode(q, func, args);

  self.connection.redis.smembers(self.connection.key('timestamps:' + search), function(error, members){
    if(members !== null){
      members.forEach(function(key){
        timestamps.push(key.split(':')[key.split(':').length - 1]);
      });
    }

    callback(error, timestamps);
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-resque.queue.prototype.stats"></a>[function <span class="apidocSignatureSpan">node-resque.queue.prototype.</span>stats (callback)](#apidoc.element.node-resque.queue.prototype.stats)
- description and source-code
```javascript
stats = function (callback){
  var self = this;
  self.connection.redis.keys(self.connection.key('stat:*'), function(error, keys){
    if(error){ return callback(error); }
    if(keys.length === 0){ return callback(); }

    self.connection.redis.mget(keys, function(error, values){
      if(error){ return callback(error); }

      var data = {};
      for(var i = 0; i < keys.length; i++){
        var k = keys[i];
        k = k.replace(self.connection.key('stat:'), '');
        data[k] = values[i];
      }

      callback(null, data);
    });
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-resque.queue.prototype.timestamps"></a>[function <span class="apidocSignatureSpan">node-resque.queue.prototype.</span>timestamps (callback)](#apidoc.element.node-resque.queue.prototype.timestamps)
- description and source-code
```javascript
timestamps = function (callback){
  var self = this;
  var results = [];
  self.connection.redis.keys(self.connection.key('delayed:*'), function(error, timestamps){
    timestamps.forEach(function(timestamp){
      var parts = timestamp.split(':');
      results.push(parseInt(parts[(parts.length - 1)]) * 1000);
    });
    results.sort();
    callback(error, results);
  });
}
```
- example usage
```shell
...
};

queue.prototype.allDelayed = function(callback){
  var self = this;
  var results = {};
  var jobs = [];

  self.timestamps(function(error, timestamps){
if(error){ return callback(error); }

timestamps.forEach(function(timestamp){
  jobs.push(function(done){
    self.delayedAt(timestamp, function(error, tasks, rTimestamp){
      if(error){ return done(error); }
      results[(rTimestamp * 1000)] = tasks;
...
```

#### <a name="apidoc.element.node-resque.queue.prototype.workers"></a>[function <span class="apidocSignatureSpan">node-resque.queue.prototype.</span>workers (callback)](#apidoc.element.node-resque.queue.prototype.workers)
- description and source-code
```javascript
workers = function (callback){
  var self = this;
  var workers = {};
  self.connection.redis.smembers(self.connection.key('workers'), function(error, results){
    if(!error && results){
      results.forEach(function(r){
        var parts = r.split(':');
        var name;
        var queues;
        if(parts.length === 1){
          name = parts[0];
          workers[name] = null;
        }
        else if(parts.length === 2){
          name = parts[0];
          queues = parts[1];
          workers[name] = queues;
        }else{
          name = parts.shift() + ':' + parts.shift();
          queues = parts.join(':');
          workers[name] = queues;
        }
      });
    }

    return callback(error, workers);
  });
}
```
- example usage
```shell
...
};

queue.prototype.allWorkingOn = function(callback){
  var self = this;
  var results = {};
  var jobs = [];

  self.workers(function(error, workers){
if(error){ return callback(error); }

Object.keys(workers).forEach(function(w){
  jobs.push(function(done){
    results[w] = 'started';
    self.workingOn(w, workers[w], function(error, data){
      if(error){ return done(error); }
...
```

#### <a name="apidoc.element.node-resque.queue.prototype.workingOn"></a>[function <span class="apidocSignatureSpan">node-resque.queue.prototype.</span>workingOn (workerName, queues, callback)](#apidoc.element.node-resque.queue.prototype.workingOn)
- description and source-code
```javascript
workingOn = function (workerName, queues, callback){
  var self = this;
  var fullWorkerName = workerName + ':' + queues;
  self.connection.redis.get(self.connection.key('worker', fullWorkerName), callback);
}
```
- example usage
```shell
...

  self.workers(function(error, workers){
if(error){ return callback(error); }

Object.keys(workers).forEach(function(w){
  jobs.push(function(done){
    results[w] = 'started';
    self.workingOn(w, workers[w], function(error, data){
      if(error){ return done(error); }
      if(data){
        data = JSON.parse(data);
        results[data.worker] = data;
      }
      done();
    });
...
```



# <a name="apidoc.module.node-resque.scheduler"></a>[module node-resque.scheduler](#apidoc.module.node-resque.scheduler)

#### <a name="apidoc.element.node-resque.scheduler.scheduler"></a>[function <span class="apidocSignatureSpan">node-resque.</span>scheduler (options, jobs)](#apidoc.element.node-resque.scheduler.scheduler)
- description and source-code
```javascript
scheduler = function (options, jobs){
  var self = this;
  if(!jobs){ jobs = {}; }
  var defaults = self.defaults();

  for(var i in defaults){
    if(options[i] === null || options[i] === undefined){
      options[i] = defaults[i];
    }
  }

  self.options    = options;
  self.name       = self.options.name;
  self.master     = false;
  self.running    = false;
  self.processing = false;

  self.queue = new queue({connection: options.connection}, jobs);

  self.queue.on('error', function(error){
    self.emit('error', error);
  });
}
```
- example usage
```shell
...
  worker.start();
});

///////////////////////
// START A SCHEDULER //
///////////////////////

var scheduler = new NR.scheduler({connection: connectionDetails});
scheduler.connect(function(){
  scheduler.start();
});

/////////////////////////
// REGESTER FOR EVENTS //
/////////////////////////
...
```

#### <a name="apidoc.element.node-resque.scheduler.super_"></a>[function <span class="apidocSignatureSpan">node-resque.scheduler.</span>super_ ()](#apidoc.element.node-resque.scheduler.super_)
- description and source-code
```javascript
function EventEmitter() {
  EventEmitter.init.call(this);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.node-resque.scheduler.prototype"></a>[module node-resque.scheduler.prototype](#apidoc.module.node-resque.scheduler.prototype)

#### <a name="apidoc.element.node-resque.scheduler.prototype.cleanupTimestamp"></a>[function <span class="apidocSignatureSpan">node-resque.scheduler.prototype.</span>cleanupTimestamp (timestamp, callback)](#apidoc.element.node-resque.scheduler.prototype.cleanupTimestamp)
- description and source-code
```javascript
cleanupTimestamp = function (timestamp, callback){
  var self = this;
  var key = self.connection.key('delayed:' + timestamp);
  self.connection.redis.llen(key, function(error, len){
    if(error){ return callback(error); }
    if(len === 0){
      self.connection.redis.del(key, function(error){
        if(error){ return callback(error); }
        self.connection.redis.zrem(self.connection.key('delayed_queue_schedule'), timestamp, function(error){
          return callback(error);
        });
      });
    }
    else{ return callback(); }
  });
}
```
- example usage
```shell
...
var self = this;
var key = self.connection.key('delayed:' + timestamp);
self.connection.redis.lpop(key, function(error, job){
  if(error){
    return callback(error);
  }else{
    self.connection.redis.srem(self.connection.key('timestamps:' + job), ('delayed:' + timestamp), function(error){
      self.cleanupTimestamp(timestamp, function(){
        if(error){
          return callback(error);
        }else{
          return callback(null, JSON.parse(job));
        }
      });
    });
...
```

#### <a name="apidoc.element.node-resque.scheduler.prototype.connect"></a>[function <span class="apidocSignatureSpan">node-resque.scheduler.prototype.</span>connect (callback)](#apidoc.element.node-resque.scheduler.prototype.connect)
- description and source-code
```javascript
connect = function (callback){
  var self = this;
  self.queue.connect(function(){
    self.connection = self.queue.connection;
    if(typeof callback === 'function'){ callback(); }
  });
}
```
- example usage
```shell
...
};

////////////////////
// START A WORKER //
////////////////////

var worker = new NR.worker({connection: connectionDetails, queues: ['math', 'otherQueue']}, jobs);
worker.connect(function(){
  worker.workerCleanup(); // optional: cleanup any previous improperly shutdown workers on this host
  worker.start();
});

///////////////////////
// START A SCHEDULER //
///////////////////////
...
```

#### <a name="apidoc.element.node-resque.scheduler.prototype.defaults"></a>[function <span class="apidocSignatureSpan">node-resque.scheduler.prototype.</span>defaults ()](#apidoc.element.node-resque.scheduler.prototype.defaults)
- description and source-code
```javascript
defaults = function (){
  var self = this;
  return {
    timeout:           5000,   // in ms
    masterLockTimeout: 60 * 3, // in seconds
    name:              os.hostname() + ':' + process.pid, // assumes only one worker per node process
  };
}
```
- example usage
```shell
...

var util  = require('util');
var async = require('async');
var EventEmitter = require('events').EventEmitter;

var connection = function(options){
var self = this;
var defaults = self.defaults();

if(!options){ options = {}; }
for(var i in defaults){
  if(options[i] === null || options[i] === undefined){
    options[i] = defaults[i];
  }
}
...
```

#### <a name="apidoc.element.node-resque.scheduler.prototype.end"></a>[function <span class="apidocSignatureSpan">node-resque.scheduler.prototype.</span>end (callback)](#apidoc.element.node-resque.scheduler.prototype.end)
- description and source-code
```javascript
end = function (callback){
  var self = this;
  self.running = false;
  clearTimeout(self.timer);

  if(self.processing === false){
    self.releaseMasterLock(function(error, wasMaster){
      if(error){ self.emit('error', error); }
      self.queue.end(function(){
        self.emit('end');
        process.nextTick(function(){
          if(typeof callback === 'function'){ callback(); }
        });
      });
    });
  }

  else{
    setTimeout(function(){
      self.end(callback);
    }, (self.options.timeout / 2));
  }
}
```
- example usage
```shell
...

worker.connect(function(){
  worker.start();
});
'''

## Notes
- Be sure to call 'worker.end(callback)', 'queue.end(callback)' and 'scheduler.end(callback)' before shutting down your application
 if you want to properly clear your worker status from resque
- When ending your application, be sure to allow your workers time to finish what they are working on
- This project implements the "scheduler" part of rescue-scheduler (the daemon which can promote enqueued delayed jobs into the
work queues when it is time), but not the CRON scheduler proxy.  To learn more about how to use a CRON-like scheduler, read the [
Job Schedules](#job-schedules) section of this document.
- If you are using any plugins which effect 'beforeEnqueue' or 'afterEnqueue', be sure to pass the 'jobs' argument to the 'new Queue
' constructor
- If a job fails, it will be added to a special 'failed' queue.  You can then inspect these jobs, write a plugin to manage them,
move them back to the normal queues, etc.  Failure behavior by default is just to enter the 'failed' queue, but there are many options
.  Check out these examples from the ruby ecosystem for inspiration:
  - https://github.com/lantins/resque-retry
  - https://github.com/resque/resque/wiki/Failure-Backends
- If you plan to run more than one worker per nodejs process, be sure to name them something distinct.  Names **must** follow the
 pattern 'hostname:pid+unique_id'.  For example:
...
```

#### <a name="apidoc.element.node-resque.scheduler.prototype.enqueueDelayedItemsForTimestamp"></a>[function <span class="apidocSignatureSpan">node-resque.scheduler.prototype.</span>enqueueDelayedItemsForTimestamp (timestamp, callback)](#apidoc.element.node-resque.scheduler.prototype.enqueueDelayedItemsForTimestamp)
- description and source-code
```javascript
enqueueDelayedItemsForTimestamp = function (timestamp, callback){
  var self = this;
  self.nextItemForTimestamp(timestamp, function(error, job){
    if(!error && job){
      self.transfer(timestamp, job, function(){
        self.enqueueDelayedItemsForTimestamp(timestamp, callback);
      });
    }else{
      return callback(error);
    }
  });
}
```
- example usage
```shell
...
  self.master = true;
  self.emit('master');
}
self.emit('poll');
self.nextDelayedTimestamp(function(error, timestamp){
  if(!error && timestamp){
    self.emit('working_timestamp', timestamp);
    self.enqueueDelayedItemsForTimestamp(timestamp, function(error){
      if(error){ self.emit('error', error); }
      self.poll(callback);
    });
  }else{
    if(error){ self.emit('error', error); }
    self.processing = false;
    self.pollAgainLater();
...
```

#### <a name="apidoc.element.node-resque.scheduler.prototype.masterKey"></a>[function <span class="apidocSignatureSpan">node-resque.scheduler.prototype.</span>masterKey ()](#apidoc.element.node-resque.scheduler.prototype.masterKey)
- description and source-code
```javascript
masterKey = function (){
  var self = this;
  return self.connection.key('resque_scheduler_master_lock');
}
```
- example usage
```shell
...
scheduler.prototype.tryForMaster = function(callback){
var self = this;

if(!self.connection || !self.connection.redis){
  return callback();
}

self.connection.redis.setnx(self.masterKey(), self.options.name, function(error, locked){
  if(error){ return callback(error); }
  else if(locked === true || locked === 1){
    self.connection.redis.expire(self.masterKey(), self.options.masterLockTimeout, function(error){
      return callback(error, true);
    });
  }else{
    self.connection.redis.get(self.masterKey(), function(error, value){
...
```

#### <a name="apidoc.element.node-resque.scheduler.prototype.nextDelayedTimestamp"></a>[function <span class="apidocSignatureSpan">node-resque.scheduler.prototype.</span>nextDelayedTimestamp (callback)](#apidoc.element.node-resque.scheduler.prototype.nextDelayedTimestamp)
- description and source-code
```javascript
nextDelayedTimestamp = function (callback){
  var self = this;
  var time = Math.round(new Date().getTime() / 1000);
  self.connection.redis.zrangebyscore(self.connection.key('delayed_queue_schedule'), '-inf', time, 'limit', 0, 1, function(error
, items){
    if(error || items === null || items.length === 0){
      return callback(error);
    }else{
      return callback(null, items[0]);
    }
  });
}
```
- example usage
```shell
...
if(error){ self.emit('error', error); }
if(isMaster){
  if(!self.master){
    self.master = true;
    self.emit('master');
  }
  self.emit('poll');
  self.nextDelayedTimestamp(function(error, timestamp){
    if(!error && timestamp){
      self.emit('working_timestamp', timestamp);
      self.enqueueDelayedItemsForTimestamp(timestamp, function(error){
        if(error){ self.emit('error', error); }
        self.poll(callback);
      });
    }else{
...
```

#### <a name="apidoc.element.node-resque.scheduler.prototype.nextItemForTimestamp"></a>[function <span class="apidocSignatureSpan">node-resque.scheduler.prototype.</span>nextItemForTimestamp (timestamp, callback)](#apidoc.element.node-resque.scheduler.prototype.nextItemForTimestamp)
- description and source-code
```javascript
nextItemForTimestamp = function (timestamp, callback){
  var self = this;
  var key = self.connection.key('delayed:' + timestamp);
  self.connection.redis.lpop(key, function(error, job){
    if(error){
      return callback(error);
    }else{
      self.connection.redis.srem(self.connection.key('timestamps:' + job), ('delayed:' + timestamp), function(error){
        self.cleanupTimestamp(timestamp, function(){
          if(error){
            return callback(error);
          }else{
            return callback(null, JSON.parse(job));
          }
        });
      });
    }
  });
}
```
- example usage
```shell
...
    return callback(null, items[0]);
  }
});
};

scheduler.prototype.enqueueDelayedItemsForTimestamp = function(timestamp, callback){
var self = this;
self.nextItemForTimestamp(timestamp, function(error, job){
  if(!error && job){
    self.transfer(timestamp, job, function(){
      self.enqueueDelayedItemsForTimestamp(timestamp, callback);
    });
  }else{
    return callback(error);
  }
...
```

#### <a name="apidoc.element.node-resque.scheduler.prototype.poll"></a>[function <span class="apidocSignatureSpan">node-resque.scheduler.prototype.</span>poll (callback)](#apidoc.element.node-resque.scheduler.prototype.poll)
- description and source-code
```javascript
poll = function (callback){
  var self = this;
  self.processing = true;
  clearTimeout(self.timer);
  self.tryForMaster(function(error, isMaster){
    if(error){ self.emit('error', error); }
    if(isMaster){
      if(!self.master){
        self.master = true;
        self.emit('master');
      }
      self.emit('poll');
      self.nextDelayedTimestamp(function(error, timestamp){
        if(!error && timestamp){
          self.emit('working_timestamp', timestamp);
          self.enqueueDelayedItemsForTimestamp(timestamp, function(error){
            if(error){ self.emit('error', error); }
            self.poll(callback);
          });
        }else{
          if(error){ self.emit('error', error); }
          self.processing = false;
          self.pollAgainLater();
          if(typeof callback === 'function'){ callback(); }
        }
      });
    }else{
      self.master = false;
      self.processing = false;
      self.pollAgainLater();
      if(typeof callback === 'function'){ callback(); }
    }
  });
}
```
- example usage
```shell
...
var self = this;
self.processing = false;

if(!self.running){
  self.emit('start');
  self.running = true;
  self.timer = setTimeout((function(){
    self.poll();
  }), self.options.timeout);
}
};

scheduler.prototype.end = function(callback){
var self = this;
self.running = false;
...
```

#### <a name="apidoc.element.node-resque.scheduler.prototype.pollAgainLater"></a>[function <span class="apidocSignatureSpan">node-resque.scheduler.prototype.</span>pollAgainLater ()](#apidoc.element.node-resque.scheduler.prototype.pollAgainLater)
- description and source-code
```javascript
pollAgainLater = function (){
  var self = this;
  if(self.running === true){
    self.timer = setTimeout(function(){
      self.poll();
    }, self.options.timeout);
  }
}
```
- example usage
```shell
...
      self.enqueueDelayedItemsForTimestamp(timestamp, function(error){
        if(error){ self.emit('error', error); }
        self.poll(callback);
      });
    }else{
      if(error){ self.emit('error', error); }
      self.processing = false;
      self.pollAgainLater();
      if(typeof callback === 'function'){ callback(); }
    }
  });
}else{
  self.master = false;
  self.processing = false;
  self.pollAgainLater();
...
```

#### <a name="apidoc.element.node-resque.scheduler.prototype.releaseMasterLock"></a>[function <span class="apidocSignatureSpan">node-resque.scheduler.prototype.</span>releaseMasterLock (callback)](#apidoc.element.node-resque.scheduler.prototype.releaseMasterLock)
- description and source-code
```javascript
releaseMasterLock = function (callback){
  var self = this;
  if(self.connection){
    self.tryForMaster(function(error, isMaster){
      if(error){ return callback(error); }
      else if(!isMaster){ return callback(null, false); }
      else{
        self.connection.redis.del(self.masterKey(), function(error, delted){
          self.master = false;
          return callback(error, (delted === 1));
        });
      }
    });
  }else{
    return callback();
  }
}
```
- example usage
```shell
...

scheduler.prototype.end = function(callback){
var self = this;
self.running = false;
clearTimeout(self.timer);

if(self.processing === false){
  self.releaseMasterLock(function(error, wasMaster){
    if(error){ self.emit('error', error); }
    self.queue.end(function(){
      self.emit('end');
      process.nextTick(function(){
        if(typeof callback === 'function'){ callback(); }
      });
    });
...
```

#### <a name="apidoc.element.node-resque.scheduler.prototype.start"></a>[function <span class="apidocSignatureSpan">node-resque.scheduler.prototype.</span>start ()](#apidoc.element.node-resque.scheduler.prototype.start)
- description and source-code
```javascript
start = function (){
  var self = this;
  self.processing = false;

  if(!self.running){
    self.emit('start');
    self.running = true;
    self.timer = setTimeout((function(){
      self.poll();
    }), self.options.timeout);
  }
}
```
- example usage
```shell
...
////////////////////
// START A WORKER //
////////////////////

var worker = new NR.worker({connection: connectionDetails, queues: ['math', 'otherQueue']}, jobs);
worker.connect(function(){
  worker.workerCleanup(); // optional: cleanup any previous improperly shutdown workers on this host
  worker.start();
});

///////////////////////
// START A SCHEDULER //
///////////////////////

var scheduler = new NR.scheduler({connection: connectionDetails});
...
```

#### <a name="apidoc.element.node-resque.scheduler.prototype.transfer"></a>[function <span class="apidocSignatureSpan">node-resque.scheduler.prototype.</span>transfer (timestamp, job, callback)](#apidoc.element.node-resque.scheduler.prototype.transfer)
- description and source-code
```javascript
transfer = function (timestamp, job, callback){
  var self = this;
  self.queue.enqueue(job.queue, job['class'], job.args, function(error){
    if(error){ self.emit('error', error); }
    self.emit('transferred_job', timestamp, job);
    return callback();
  });
}
```
- example usage
```shell
...
  });
};

scheduler.prototype.enqueueDelayedItemsForTimestamp = function(timestamp, callback){
  var self = this;
  self.nextItemForTimestamp(timestamp, function(error, job){
    if(!error && job){
      self.transfer(timestamp, job, function(){
        self.enqueueDelayedItemsForTimestamp(timestamp, callback);
      });
    }else{
      return callback(error);
    }
  });
};
...
```

#### <a name="apidoc.element.node-resque.scheduler.prototype.tryForMaster"></a>[function <span class="apidocSignatureSpan">node-resque.scheduler.prototype.</span>tryForMaster (callback)](#apidoc.element.node-resque.scheduler.prototype.tryForMaster)
- description and source-code
```javascript
tryForMaster = function (callback){
  var self = this;

  if(!self.connection || !self.connection.redis){
    return callback();
  }

  self.connection.redis.setnx(self.masterKey(), self.options.name, function(error, locked){
    if(error){ return callback(error); }
    else if(locked === true || locked === 1){
      self.connection.redis.expire(self.masterKey(), self.options.masterLockTimeout, function(error){
        return callback(error, true);
      });
    }else{
      self.connection.redis.get(self.masterKey(), function(error, value){
        if(error){ return callback(error); }
        else if(value === self.options.name){
          self.connection.redis.expire(self.masterKey(), self.options.masterLockTimeout, function(error){
            return callback(error, true);
          });
        }else{
          return callback(null, false);
        }
      });
    }
  });
}
```
- example usage
```shell
...
}
};

scheduler.prototype.poll = function(callback){
var self = this;
self.processing = true;
clearTimeout(self.timer);
self.tryForMaster(function(error, isMaster){
  if(error){ self.emit('error', error); }
  if(isMaster){
    if(!self.master){
      self.master = true;
      self.emit('master');
    }
    self.emit('poll');
...
```



# <a name="apidoc.module.node-resque.worker"></a>[module node-resque.worker](#apidoc.module.node-resque.worker)

#### <a name="apidoc.element.node-resque.worker.worker"></a>[function <span class="apidocSignatureSpan">node-resque.</span>worker (options, jobs)](#apidoc.element.node-resque.worker.worker)
- description and source-code
```javascript
worker = function (options, jobs){
  var self = this;
  if(!jobs){ jobs = {}; }

  var defaults = self.defaults();
  for(var i in defaults){
    if(options[i] === undefined || options[i] === null){
      options[i] = defaults[i];
    }
  }

  self.options = options;
  self.jobs = prepareJobs(jobs);
  self.name = self.options.name;
  self.queues = self.options.queues;
  self.error = null;
  self.result = null;
  self.ready = false;
  self.running = false;
  self.working = false;
  self.job = null;

  self.queueObject = new queue({connection: options.connection}, self.jobs);

  self.queueObject.on('error', function(error){
    self.emit('error', null, null, error);
  });
}
```
- example usage
```shell
...
  },
};

////////////////////
// START A WORKER //
////////////////////

var worker = new NR.worker({connection: connectionDetails, queues: ['math', 'otherQueue']}, jobs);
worker.connect(function(){
  worker.workerCleanup(); // optional: cleanup any previous improperly shutdown workers on this host
  worker.start();
});

///////////////////////
// START A SCHEDULER //
...
```

#### <a name="apidoc.element.node-resque.worker.super_"></a>[function <span class="apidocSignatureSpan">node-resque.worker.</span>super_ ()](#apidoc.element.node-resque.worker.super_)
- description and source-code
```javascript
function EventEmitter() {
  EventEmitter.init.call(this);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.node-resque.worker.prototype"></a>[module node-resque.worker.prototype](#apidoc.module.node-resque.worker.prototype)

#### <a name="apidoc.element.node-resque.worker.prototype.checkQueues"></a>[function <span class="apidocSignatureSpan">node-resque.worker.prototype.</span>checkQueues (callback)](#apidoc.element.node-resque.worker.prototype.checkQueues)
- description and source-code
```javascript
checkQueues = function (callback){
  var self = this;
  if(typeof self.queues === 'string'){
    self.queues = [self.queues];
  }
  if(self.ready === true && self.queues.length > 0 && self.queues.shift){
    return;
  }

  if((self.queues[0] === '*' && self.queues.length === 1) || self.queues.length === 0){
    self.originalQueue = '*';
    self.untrack(self.name, self.stringQueues(), function(error){
      if(error){
        self.emit('error', null, null, error);
        if(typeof callback === 'function'){ callback(error); }
        return;
      }

      self.connection.redis.smembers(self.connection.key('queues'), function(error, resp){
        if(error){
          self.emit('error', null, null, error);
          if(typeof callback === 'function'){ callback(error); }
          return;
        }

        self.queues = resp ? resp.sort() : [];
        self.track(function(error){
          if(error){ self.emit('error', null, null, error); }
          self.ready = true;
          if(typeof callback === 'function'){ callback(error); }
        });
      });
    });
  }else{
    if(self.queues instanceof String){ self.queues = self.queues.split(','); }
    self.ready = true;
    if(typeof callback === 'function'){ callback(); }
  }
}
```
- example usage
```shell
...
};
};

worker.prototype.connect = function(callback){
var self = this;
self.queueObject.connect(function(){
  self.connection = self.queueObject.connection;
  self.checkQueues(function(){
    if(typeof callback === 'function'){ callback(); }
  });
});
};

worker.prototype.start = function(){
var self = this;
...
```

#### <a name="apidoc.element.node-resque.worker.prototype.completeJob"></a>[function <span class="apidocSignatureSpan">node-resque.worker.prototype.</span>completeJob (toRespond, callback)](#apidoc.element.node-resque.worker.prototype.completeJob)
- description and source-code
```javascript
completeJob = function (toRespond, callback){
  var self = this;
  var job = self.job;
  var jobs = [];

  if(self.error){
    jobs.push(function(done){
      self.fail(self.error, done);
    });
  }else if(toRespond){
    jobs.push(function(done){
      self.succeed(job, done);
    });
  }

  jobs.push(function(done){
    self.doneWorking(done);
  });

  async.series(jobs, function(error){
    if(error){ self.emit('error', null, null, error); }
    self.job = null;

    if(self.options.looping){
      return self.poll();
    }else if(typeof callback === 'function'){
      return callback(error);
    }
  });
}
```
- example usage
```shell
...
  var self = this;
  var returnCounter = 0; // a state counter to prevent multiple returns from poor jobs or plugins
  var callbackError = new Error('refusing to continue with job, multiple callbacks detected');
  self.job = job;
  self.error = null;
  if(!self.jobs[job['class']]){
self.error = new Error('No job defined for class "' + job['class'] + '"');
self.completeJob(true, callback);
  }else{
var cb = self.jobs[job['class']].perform;
self.emit('job', self.queue, job);

if(cb){
  pluginRunner.runPlugins(self, 'before_perform', job['class'], self.queue, self.jobs[job['class']], job.args, function(err, toRun
){
    returnCounter++;
...
```

#### <a name="apidoc.element.node-resque.worker.prototype.connect"></a>[function <span class="apidocSignatureSpan">node-resque.worker.prototype.</span>connect (callback)](#apidoc.element.node-resque.worker.prototype.connect)
- description and source-code
```javascript
connect = function (callback){
  var self = this;
  self.queueObject.connect(function(){
    self.connection = self.queueObject.connection;
    self.checkQueues(function(){
      if(typeof callback === 'function'){ callback(); }
    });
  });
}
```
- example usage
```shell
...
};

////////////////////
// START A WORKER //
////////////////////

var worker = new NR.worker({connection: connectionDetails, queues: ['math', 'otherQueue']}, jobs);
worker.connect(function(){
  worker.workerCleanup(); // optional: cleanup any previous improperly shutdown workers on this host
  worker.start();
});

///////////////////////
// START A SCHEDULER //
///////////////////////
...
```

#### <a name="apidoc.element.node-resque.worker.prototype.defaults"></a>[function <span class="apidocSignatureSpan">node-resque.worker.prototype.</span>defaults ()](#apidoc.element.node-resque.worker.prototype.defaults)
- description and source-code
```javascript
defaults = function (){
  var self = this;
  return {
    name:      os.hostname() + ':' + process.pid, // assumes only one worker per node process
    queues:    '*',
    timeout:   5000,
    looping:   true,
  };
}
```
- example usage
```shell
...

var util  = require('util');
var async = require('async');
var EventEmitter = require('events').EventEmitter;

var connection = function(options){
var self = this;
var defaults = self.defaults();

if(!options){ options = {}; }
for(var i in defaults){
  if(options[i] === null || options[i] === undefined){
    options[i] = defaults[i];
  }
}
...
```

#### <a name="apidoc.element.node-resque.worker.prototype.doneWorking"></a>[function <span class="apidocSignatureSpan">node-resque.worker.prototype.</span>doneWorking (callback)](#apidoc.element.node-resque.worker.prototype.doneWorking)
- description and source-code
```javascript
doneWorking = function (callback){
  var self = this;
  self.working = false;
  self.connection.redis.del(self.connection.key('worker', self.name, self.stringQueues()), callback);
}
```
- example usage
```shell
...
  }else if(toRespond){
jobs.push(function(done){
  self.succeed(job, done);
});
  }

  jobs.push(function(done){
self.doneWorking(done);
  });

  async.series(jobs, function(error){
if(error){ self.emit('error', null, null, error); }
self.job = null;

if(self.options.looping){
...
```

#### <a name="apidoc.element.node-resque.worker.prototype.end"></a>[function <span class="apidocSignatureSpan">node-resque.worker.prototype.</span>end (callback)](#apidoc.element.node-resque.worker.prototype.end)
- description and source-code
```javascript
end = function (callback){
  var self = this;
  self.running = false;
  if(self.working === true){
    setTimeout(function(){
      self.end(callback);
    }, self.options.timeout);
  }else{
    self.untrack(self.name, self.stringQueues(), function(error){
      self.queueObject.end(function(error){
        self.emit('end');
        if(typeof callback === 'function'){ callback(error); }
      });
    });
  }
}
```
- example usage
```shell
...

worker.connect(function(){
  worker.start();
});
'''

## Notes
- Be sure to call 'worker.end(callback)', 'queue.end(callback)' and 'scheduler.end(callback)' before shutting down your application
 if you want to properly clear your worker status from resque
- When ending your application, be sure to allow your workers time to finish what they are working on
- This project implements the "scheduler" part of rescue-scheduler (the daemon which can promote enqueued delayed jobs into the
work queues when it is time), but not the CRON scheduler proxy.  To learn more about how to use a CRON-like scheduler, read the [
Job Schedules](#job-schedules) section of this document.
- If you are using any plugins which effect 'beforeEnqueue' or 'afterEnqueue', be sure to pass the 'jobs' argument to the 'new Queue
' constructor
- If a job fails, it will be added to a special 'failed' queue.  You can then inspect these jobs, write a plugin to manage them,
move them back to the normal queues, etc.  Failure behavior by default is just to enter the 'failed' queue, but there are many options
.  Check out these examples from the ruby ecosystem for inspiration:
  - https://github.com/lantins/resque-retry
  - https://github.com/resque/resque/wiki/Failure-Backends
- If you plan to run more than one worker per nodejs process, be sure to name them something distinct.  Names **must** follow the
 pattern 'hostname:pid+unique_id'.  For example:
...
```

#### <a name="apidoc.element.node-resque.worker.prototype.fail"></a>[function <span class="apidocSignatureSpan">node-resque.worker.prototype.</span>fail (err, callback)](#apidoc.element.node-resque.worker.prototype.fail)
- description and source-code
```javascript
fail = function (err, callback){
  var self = this;
  var jobs = [];
  var failingJob = self.job;

  jobs.push(function(done){
    self.connection.redis.incr(self.connection.key('stat', 'failed'), done);
  });

  jobs.push(function(done){
    self.connection.redis.incr(self.connection.key('stat', 'failed', self.name), done);
  });

  jobs.push(function(done){
    self.connection.redis.rpush(self.connection.key('failed'), JSON.stringify(self.failurePayload(err, failingJob)), done);
  });

  async.series(jobs, function(error){
    if(error){
      self.emit('error', null, null, error);
      if(typeof callback === 'function'){ return callback(error); }
    }else{
      self.emit('failure', self.queue, failingJob, err);
      if(typeof callback === 'function'){ return callback(); }
    }
  });
}
```
- example usage
```shell
...
- callback(error, failedJobs)
- 'failedJobs' is an array listing the data of the failed jobs.  Each element looks like:

### Failing a Job

It is *very* important that your jobs handle uncaughtRejections and other errors of this type properly.  As of 'node-resque' version
 4, we no longer use 'domains' to catch what would otherwise be crash-inducing errors in your jobs.  This means that a job which
 causes your application to crash WILL BE LOST FOREVER.  Please use 'catch()' on your promises, handle all of your callbacks, and
 otherwise write robust node.js applications.

If you choose to use 'domains', 'process.onExit', or any other method of "catching" a process crash, you can still move the job '
node-resque' was working on to the redis error queue with 'worker.fail(error, callback)'.

'''javascript
{ worker: 'busted-worker-3',
queue: 'busted-queue',
payload: { class: 'busted_job', queue: 'busted-queue', args: [ 1, 2, 3 ] },
exception: 'ERROR_NAME',
error: 'I broke',
...
```

#### <a name="apidoc.element.node-resque.worker.prototype.failurePayload"></a>[function <span class="apidocSignatureSpan">node-resque.worker.prototype.</span>failurePayload (err, job)](#apidoc.element.node-resque.worker.prototype.failurePayload)
- description and source-code
```javascript
failurePayload = function (err, job){
  var self = this;
  return {
    worker: self.name,
    queue: self.queue,
    payload: job,
    exception: err.name,
    error: err.message,
    backtrace: err.stack ? err.stack.split('\n').slice(1) : null,
    failed_at: (new Date()).toString()
  };
}
```
- example usage
```shell
...
});

jobs.push(function(done){
  self.connection.redis.incr(self.connection.key('stat', 'failed', self.name), done);
});

jobs.push(function(done){
  self.connection.redis.rpush(self.connection.key('failed'), JSON.stringify(self.failurePayload(err, failingJob)), done);
});

async.series(jobs, function(error){
  if(error){
    self.emit('error', null, null, error);
    if(typeof callback === 'function'){ return callback(error); }
  }else{
...
```

#### <a name="apidoc.element.node-resque.worker.prototype.getPids"></a>[function <span class="apidocSignatureSpan">node-resque.worker.prototype.</span>getPids (callback)](#apidoc.element.node-resque.worker.prototype.getPids)
- description and source-code
```javascript
getPids = function (callback){
  var cmd;
  if(process.platform === 'win32'){
    cmd = 'for /f "usebackq tokens=2 skip=2" %i in ('tasklist /nh') do @echo %i';
  }else{
    cmd = 'ps -ef | awk \'{print $2}\'';
  }

  var child = exec(cmd, function(error, stdout, stderr){
    var pids = [];
    stdout.split('\n').forEach(function(line){
      line = line.trim();
      if(line.length > 0){
        var pid = parseInt(line.split(' ')[0]);
        if(!isNaN(pid)){ pids.push(pid); }
      }
    });

    if(!error && stderr){ error = stderr; }
    callback(error, pids);
  });
}
```
- example usage
```shell
...
});
  });
};

worker.prototype.workerCleanup = function(callback){
  var self = this;
  var jobs = [];
  self.getPids(function(error, pids){
if(error){
  self.emit('error', null, null, error);
  if(typeof callback === 'function'){ callback(error); }
  return;
}

self.connection.redis.smembers(self.connection.key('workers'), function(error, workers){
...
```

#### <a name="apidoc.element.node-resque.worker.prototype.init"></a>[function <span class="apidocSignatureSpan">node-resque.worker.prototype.</span>init (callback)](#apidoc.element.node-resque.worker.prototype.init)
- description and source-code
```javascript
init = function (callback){
  var self = this;
  var args;
  var _ref;
  self.track(function(error){
    if(error){
      self.emit('error', null, null, error);
      if(typeof callback === 'function'){ callback(error); }
      return;
    }

    self.connection.redis.set(self.connection.key('worker', self.name, self.stringQueues(), 'started'), Math.round((new Date()).
getTime() / 1000), function(error){
      if(error){ self.emit('error', null, null, error); }
      if(typeof callback === 'function'){ callback(error); }
    });
  });
}
```
- example usage
```shell
...
});
};

worker.prototype.start = function(){
var self = this;
if(self.ready){
  self.emit('start');
  self.init(function(){
    self.poll();
  });
}
};

worker.prototype.end = function(callback){
var self = this;
...
```

#### <a name="apidoc.element.node-resque.worker.prototype.pause"></a>[function <span class="apidocSignatureSpan">node-resque.worker.prototype.</span>pause ()](#apidoc.element.node-resque.worker.prototype.pause)
- description and source-code
```javascript
pause = function (){
  var self = this;
  self.emit('pause');
  setTimeout(function(){
    if(!self.running){ return; }
    self.poll();
  }, self.options.timeout);
}
```
- example usage
```shell
...
if(!self.running){
  if(typeof callback === 'function'){ callback(); }
}else{
  self.queue = self.queues[nQueue];
  self.emit('poll', self.queue);
  if(self.queue === null || self.queue === undefined){
    self.checkQueues(function(){
      self.pause();
    });
  }else if(self.working === true){
    var error = new Error('refusing to get new job, already working');
    self.emit('error', self.queue, null, error);
  }else{
    self.working = true;
    self.connection.redis.lpop(self.connection.key('queue', self.queue), function(error, resp){
...
```

#### <a name="apidoc.element.node-resque.worker.prototype.perform"></a>[function <span class="apidocSignatureSpan">node-resque.worker.prototype.</span>perform (job, callback)](#apidoc.element.node-resque.worker.prototype.perform)
- description and source-code
```javascript
perform = function (job, callback){
  var self = this;
  var returnCounter = 0; // a state counter to prevent multiple returns from poor jobs or plugins
  var callbackError = new Error('refusing to continue with job, multiple callbacks detected');
  self.job = job;
  self.error = null;
  if(!self.jobs[job['class']]){
    self.error = new Error('No job defined for class "' + job['class'] + '"');
    self.completeJob(true, callback);
  }else{
    var cb = self.jobs[job['class']].perform;
    self.emit('job', self.queue, job);

    if(cb){
      pluginRunner.runPlugins(self, 'before_perform', job['class'], self.queue, self.jobs[job['class']], job.args, function(err,
toRun){
        returnCounter++;
        if(returnCounter !== 1){
          self.emit('failure', self.queue, job, callbackError);
        }else if(toRun === false){
          self.completeJob(false, callback);
        }else{
          self.error = err;
          self.workingOn(job);
          var args;
          if(job.args === undefined || (job.args instanceof Array) === true){
            args = job.args;
          }else{
            args = [job.args];
          }

          var combinedInputs = [].slice.call(args).concat([function(err, result){
            returnCounter++;
            if(returnCounter !== 2){
              self.emit('failure', self.queue, job, callbackError);
            }else{
              self.error = err;
              self.result = result;
              pluginRunner.runPlugins(self, 'after_perform', job['class'], self.queue, self.jobs[job['class']], job.args, function
(e, toRun){
                if(self.error === undefined && e){ self.error = e; }
                returnCounter++;
                if(returnCounter !== 3){
                  self.emit('failure', self.queue, job, callbackError);
                }else{
                  self.completeJob(true, callback);
                }
              });
            }
          }]);

          // When returning the payload back to redis (on error), it is important that the orignal payload is preserved
          // To help with this, we can stry to make the inputs to the job immutible
          // https://github.com/taskrabbit/node-resque/issues/99
          // Note: if an input is a string or a number, you CANNOT freeze it saddly.
          for(var i in combinedInputs){
            if((typeof combinedInputs[i] === 'object') && (combinedInputs[i] !== null)){
              Object.freeze(combinedInputs[i]);
            }
          }

          cb.apply(self, combinedInputs);
        }
      });

    }else{

      self.error = new Error('Missing Job: ' + job['class']);
      self.completeJob(true, callback);
    }
  }
}
```
- example usage
```shell
...
    }else{
self.working = true;
self.connection.redis.lpop(self.connection.key('queue', self.queue), function(error, resp){
  if(!error && resp){
    var currentJob = JSON.parse(resp.toString());
    if(self.options.looping){
      self.result = null;
      self.perform(currentJob);
    }else{
      if(typeof callback === 'function'){ callback(currentJob); }
    }
  }else{
    if(error){
      self.emit('error', self.queue, null, error);
    }
...
```

#### <a name="apidoc.element.node-resque.worker.prototype.performInline"></a>[function <span class="apidocSignatureSpan">node-resque.worker.prototype.</span>performInline (func, args, callback)](#apidoc.element.node-resque.worker.prototype.performInline)
- description and source-code
```javascript
performInline = function (func, args, callback){
  var self          = this;
  var q             = '_direct-queue-' + self.name;
  var returnCounter = 0; // a state counter to prevent multiple returns from poor jobs or plugins
  var callbackError = new Error('refusing to continue with job, multiple callbacks detected');

  if(args !== undefined && args !== null && args instanceof Array !== true){
    args = [args];
  }

  if(!self.jobs[func]){         return callback(new Error('No job defined for class "' + func + '"')); }
  if(!self.jobs[func].perform){ return callback(new Error('Missing Job: ' + func));                    }

  pluginRunner.runPlugins(self, 'before_perform', func, q, self.jobs[func], args, function(err, toRun){
    returnCounter++;
    if(err){ return callback(err); }
    if(returnCounter !== 1){ return callback(callbackError); }
    if(toRun === false){ return callback(); }

    var combinedInputs = [].slice.call(args).concat([function(err, result){
      self.result = result;
      self.error = err;
      returnCounter++;
      if(err){ return callback(err); }
      if(returnCounter !== 2){ return callback(callbackError); }

      pluginRunner.runPlugins(self, 'after_perform', func, q, self.jobs[func], args, function(err, toRun){
        returnCounter++;
        if(err){ return callback(err); }
        if(returnCounter !== 3){ return callback(callbackError); }
        return callback(null, result);
      });
    }]);

    self.jobs[func].perform.apply(self, combinedInputs);
  });

}
```
- example usage
```shell
...
'''javascript
var name = os.hostname() + ":" + process.pid + "+" + counter;
var worker = new NR.worker({connection: connectionDetails, queues: 'math', 'name' : name}, jobs);
'''

###  worker#performInline

**DO NOT USE THIS IN PRODUCTION**. In tests or special cases, you may want to process/work a job in-line. To do so, you can use '
worker.performInline(jobName, arguments, callback)'.  If you are planning on running a job via #performInline, this worker should
 also not be started, nor should be using event emitters to monitor this worker.  This method will also not write to redis at all
, including logging errors, modify resque's stats, etc.

## Queue Management

Additional methods provided on the 'queue' object:

- **queue.stats** = function(callback)
- callback(error, stats_from_your_cluster)
...
```

#### <a name="apidoc.element.node-resque.worker.prototype.poll"></a>[function <span class="apidocSignatureSpan">node-resque.worker.prototype.</span>poll (nQueue, callback)](#apidoc.element.node-resque.worker.prototype.poll)
- description and source-code
```javascript
poll = function (nQueue, callback){
  var self = this;
  if(nQueue === null || nQueue === undefined){
    nQueue = 0;
  }
  if(!self.running){
    if(typeof callback === 'function'){ callback(); }
  }else{
    self.queue = self.queues[nQueue];
    self.emit('poll', self.queue);
    if(self.queue === null || self.queue === undefined){
      self.checkQueues(function(){
        self.pause();
      });
    }else if(self.working === true){
      var error = new Error('refusing to get new job, already working');
      self.emit('error', self.queue, null, error);
    }else{
      self.working = true;
      self.connection.redis.lpop(self.connection.key('queue', self.queue), function(error, resp){
        if(!error && resp){
          var currentJob = JSON.parse(resp.toString());
          if(self.options.looping){
            self.result = null;
            self.perform(currentJob);
          }else{
            if(typeof callback === 'function'){ callback(currentJob); }
          }
        }else{
          if(error){
            self.emit('error', self.queue, null, error);
          }
          self.working = false;
          if(nQueue === self.queues.length - 1){
            process.nextTick(function(){
              if(self.options.looping){
                self.pause();
              }else{
                if(typeof callback === 'function'){ callback(); }
              }
            });
          }else{
            process.nextTick(function(){
              self.poll(nQueue + 1, callback);
            });
          }
        }
      });
    }
  }
}
```
- example usage
```shell
...
var self = this;
self.processing = false;

if(!self.running){
  self.emit('start');
  self.running = true;
  self.timer = setTimeout((function(){
    self.poll();
  }), self.options.timeout);
}
};

scheduler.prototype.end = function(callback){
var self = this;
self.running = false;
...
```

#### <a name="apidoc.element.node-resque.worker.prototype.start"></a>[function <span class="apidocSignatureSpan">node-resque.worker.prototype.</span>start ()](#apidoc.element.node-resque.worker.prototype.start)
- description and source-code
```javascript
start = function (){
  var self = this;
  if(self.ready){
    self.emit('start');
    self.init(function(){
      self.poll();
    });
  }
}
```
- example usage
```shell
...
////////////////////
// START A WORKER //
////////////////////

var worker = new NR.worker({connection: connectionDetails, queues: ['math', 'otherQueue']}, jobs);
worker.connect(function(){
  worker.workerCleanup(); // optional: cleanup any previous improperly shutdown workers on this host
  worker.start();
});

///////////////////////
// START A SCHEDULER //
///////////////////////

var scheduler = new NR.scheduler({connection: connectionDetails});
...
```

#### <a name="apidoc.element.node-resque.worker.prototype.stringQueues"></a>[function <span class="apidocSignatureSpan">node-resque.worker.prototype.</span>stringQueues ()](#apidoc.element.node-resque.worker.prototype.stringQueues)
- description and source-code
```javascript
stringQueues = function (){
  var self = this;
  if(self.queues.length === 0){
    return ['*'].join(',');
  }else{
    try{
      return self.queues.join(',');
    }catch(e){
      return '';
    }
  }
}
```
- example usage
```shell
...
  var self = this;
  self.running = false;
  if(self.working === true){
    setTimeout(function(){
      self.end(callback);
    }, self.options.timeout);
  }else{
    self.untrack(self.name, self.stringQueues(), function(error){
      self.queueObject.end(function(error){
        self.emit('end');
        if(typeof callback === 'function'){ callback(error); }
      });
    });
  }
};
...
```

#### <a name="apidoc.element.node-resque.worker.prototype.succeed"></a>[function <span class="apidocSignatureSpan">node-resque.worker.prototype.</span>succeed (job, callback)](#apidoc.element.node-resque.worker.prototype.succeed)
- description and source-code
```javascript
succeed = function (job, callback){
  var self = this;
  var jobs = [];

  jobs.push(function(done){
    self.connection.redis.incr(self.connection.key('stat', 'processed'), done);
  });

  jobs.push(function(done){
    self.connection.redis.incr(self.connection.key('stat', 'processed', self.name), done);
  });

  async.series(jobs, function(error){
    if(error){ self.emit('error', null, null, error); }
    else{ self.emit('success', self.queue, job, self.result); }

    if(typeof callback === 'function'){ return callback(); }
  });
}
```
- example usage
```shell
...

if(self.error){
  jobs.push(function(done){
    self.fail(self.error, done);
  });
}else if(toRespond){
  jobs.push(function(done){
    self.succeed(job, done);
  });
}

jobs.push(function(done){
  self.doneWorking(done);
});
...
```

#### <a name="apidoc.element.node-resque.worker.prototype.track"></a>[function <span class="apidocSignatureSpan">node-resque.worker.prototype.</span>track (callback)](#apidoc.element.node-resque.worker.prototype.track)
- description and source-code
```javascript
track = function (callback){
  var self = this;
  self.running = true;
  self.connection.redis.sadd(self.connection.key('workers'), (self.name + ':' + self.stringQueues()), function(error){
    if(error){ self.emit('error', null, null, error); }
    if(typeof callback === 'function'){ callback(error); }
  });
}
```
- example usage
```shell
...
  }
};

worker.prototype.init = function(callback){
  var self = this;
  var args;
  var _ref;
  self.track(function(error){
if(error){
  self.emit('error', null, null, error);
  if(typeof callback === 'function'){ callback(error); }
  return;
}

self.connection.redis.set(self.connection.key('worker', self.name, self.stringQueues(), 'started'), Math.round((new Date()).getTime
() / 1000), function(error){
...
```

#### <a name="apidoc.element.node-resque.worker.prototype.untrack"></a>[function <span class="apidocSignatureSpan">node-resque.worker.prototype.</span>untrack (name, queues, callback)](#apidoc.element.node-resque.worker.prototype.untrack)
- description and source-code
```javascript
untrack = function (name, queues, callback){
  var self = this;
  var jobs = [];

  if(self.connection && self.connection.redis){
    self.connection.redis.srem(self.connection.key('workers'), (name + ':' + queues), function(error){
      if(error){
        self.emit('error', null, null, error);
        if(typeof callback === 'function'){ callback(error); }
        return;
      }

      [
        self.connection.key('worker', name, self.stringQueues()),
        self.connection.key('worker', name, self.stringQueues(), 'started'),
        self.connection.key('stat', 'failed', name),
        self.connection.key('stat', 'processed', name)
      ].forEach(function(key){
        jobs.push(function(done){ self.connection.redis.del(key, done); });
      });

      async.series(jobs, function(error){
        if(error){ self.emit('error', null, null, error); }
        if(typeof callback === 'function'){ callback(error); }
      });
    });
  }else{
    callback();
  }
}
```
- example usage
```shell
...
  var self = this;
  self.running = false;
  if(self.working === true){
    setTimeout(function(){
      self.end(callback);
    }, self.options.timeout);
  }else{
    self.untrack(self.name, self.stringQueues(), function(error){
      self.queueObject.end(function(error){
        self.emit('end');
        if(typeof callback === 'function'){ callback(error); }
      });
    });
  }
};
...
```

#### <a name="apidoc.element.node-resque.worker.prototype.workerCleanup"></a>[function <span class="apidocSignatureSpan">node-resque.worker.prototype.</span>workerCleanup (callback)](#apidoc.element.node-resque.worker.prototype.workerCleanup)
- description and source-code
```javascript
workerCleanup = function (callback){
  var self = this;
  var jobs = [];
  self.getPids(function(error, pids){
    if(error){
      self.emit('error', null, null, error);
      if(typeof callback === 'function'){ callback(error); }
      return;
    }

    self.connection.redis.smembers(self.connection.key('workers'), function(error, workers){
      if(error){
        if(typeof callback === 'function'){ callback(error); }
        else{ self.emit('error', null, null, error); }
        return;
      }

      workers.forEach(function(w){
        var parts = w.split(':');
        var host = parts[0]; var pid = parseInt(parts[1]); var queues = parseInt(parts[2]);
        if(host === os.hostname() && pids.indexOf(pid) < 0){
          jobs.push(function(done){
            self.emit('cleaning_worker', w, pid);
            var parts = w.split(':');
            var queues = parts.splice(-1, 1);
            var pureName = parts.join(':');
            self.untrack(pureName, queues, done);
          });
        }
      });

      async.series(jobs, function(error){
        if(error){ self.emit('error', null, null, error); }
        if(typeof callback === 'function'){ callback(error); }
      });
    });
  });
}
```
- example usage
```shell
...

////////////////////
// START A WORKER //
////////////////////

var worker = new NR.worker({connection: connectionDetails, queues: ['math', 'otherQueue']}, jobs);
worker.connect(function(){
  worker.workerCleanup(); // optional: cleanup any previous improperly shutdown workers on this host
  worker.start();
});

///////////////////////
// START A SCHEDULER //
///////////////////////
...
```

#### <a name="apidoc.element.node-resque.worker.prototype.workingOn"></a>[function <span class="apidocSignatureSpan">node-resque.worker.prototype.</span>workingOn (job)](#apidoc.element.node-resque.worker.prototype.workingOn)
- description and source-code
```javascript
workingOn = function (job){
  var self = this;
  self.connection.redis.set(self.connection.key('worker', self.name, self.stringQueues()), JSON.stringify({
    run_at: (new Date()).toString(),
    queue: self.queue,
    payload: job,
    worker: self.name,
  }));
}
```
- example usage
```shell
...

  self.workers(function(error, workers){
if(error){ return callback(error); }

Object.keys(workers).forEach(function(w){
  jobs.push(function(done){
    results[w] = 'started';
    self.workingOn(w, workers[w], function(error, data){
      if(error){ return done(error); }
      if(data){
        data = JSON.parse(data);
        results[data.worker] = data;
      }
      done();
    });
...
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
