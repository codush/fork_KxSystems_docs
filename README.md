```
Modified from README.md & mkdocs.yml
```

Documentation for kdb+ and q
============================



Version 2.0 of the documentation site at [code.kx.com/q](https://code.kx.com/q).



Platform
--------

This site is generated with the [MkDocs](https://mkdocs.org/) static-site generator, with the [Material for MkDocs](https://squidfunk.github.io/mkdocs-material/) theme. 

See [`install.md`](CONTRIBUTING/install.md) for how to compile the site. 


Not upwardly compatible
-----------------------

Version 2.0 substantially reorganizes the URL structure of the site. 
Most keywords and operators now have short URLs, e.g. code.kx.com/q/ref/aj and code.kx.com/q/ref/fill. 

This marks a break from [Version 1.0](https://github.com/kxsystems/docs-v1/). 
There is no Git continuity between the two repos. 

The terminology revision begun in Version 1.0 is complete: _adverbs_ are now _iterators_. The Reference material for them has been completely rewritten and the 2013 whitepaper “Efficient use of adverbs” re-issued as [“Iterators”](https://code.kx.com/q/wp/iterators/). The concept of _rank_ is extended from functions to all applicable values. _Variadic_ replaces _ambivalent_ for values (e.g. derived functions and matrixes) that may be applied as either unary or binary. 

The Cookbook articles are now in the [Knowledge Base](https://code.kx.com/q/kb/).



## Contact

This is a project of the [Kx Librarian](mailto:librarian@kx.com)

> A librarian’s job is to put information where people can find it. 




INHERIT: ./base-config.yml

copyright: 'This work is licensed under a <a rel="license" href="https://creativecommons.org/licenses/by/4.0/">Creative Commons Attribution 4.0 International License</a>.<br/>Kx and kdb+ are registered trademarks of <a href="https://kx.com">Kx Systems, Inc.</a>, a subsidiary of <a href="https://www.fdtechnologies.com/">FD Technologies plc</a>.'

extra_css:
  - https://code.kx.com/stylesheets/2021.css # DO NOT ALTER 
  - https://code.kx.com/stylesheets/prism.css # DO NOT ALTER 
  - https://code.kx.com/stylesheets/extra.css # MAY BE COMMENTED OUT
  - https://code.kx.com/stylesheets/hide-footer-nav.css # MAY BE COMMENTED OUT
  - stylesheets/q.css # site-specific style

extra_javascript:
  - https://code.kx.com/scripts/prism.js
  - https://code.kx.com/scripts/jquery-3.6.0.min.js # jQuery for scripts/qsearch.js
  - https://code.kx.com/scripts/extra.js # DO NOT ALTER 
  - https://code.kx.com/scripts/mathjax.js
  - https://code.kx.com/scripts/polyfill.min.js
  - https://code.kx.com/scripts/tex-mml-chtml.js
  - scripts/qsearch.js # site-specific search engine

remote_branch: master
repo_name: ''
repo_url: ''
edit_uri: ""

site_description: 'Documentation for kdb+ and the q programming language'
site_name: 'Kdb+ and q documentation'
site_url: https://code.kx.com/q

theme:
  features:
    - content.code.annotate # Insiders
    - content.tabs.link # Insiders
    - header.autohide
    - navigation.tabs
    - navigation.top
  static_templates:
    - 401.html # required by other subsites
    - 404.html # required by other subsites


nav ![Image](https://user-images.githubusercontent.com/7394636/221762461-c7d30368-243b-4083-adbe-ef4d65bd08d5.png)

  - # Home: https://code.kx.com/home
    - [KX Community](https://code.kx.com/home/community/)
    - [KX Form](https://community.kx.com/t5/Discussion-Forums/ct-p/discussion_forums) `#q&a`
    - Github
        - `#demo` keywords: [q](https://github.com/search?q=topic%3Aq) [kdb](https://github.com/search?q=topic%3Akdb) [kdb-q](https://github.com/search?q=topic%3Akdb-q)
    - [Youtube](https://www.youtube.com/playlist?list=PLypX5sYuDqvq3PRQWkgVu3Y5kSQD9Lkc4) `#tutorial`
    - [KX Academy](https://kx.com/academy) `#tutorial`
    - [Support](https://code.kx.com/home/support/)
    - [About KX](https://kx.com/)
  - # Learn:
    - [local](./docs/learn/index.md) [online](https://code.kx.com/q/learn) Get started
    - [local](./docs/learn/install.md) [online](https://code.kx.com/q/learn/install) Install
    - [local](./docs/learn/licensing.md) [online](https://code.kx.com/q/learn/licensing) Licenses
    - Mountain tour:
      - [local](./docs/learn/tour/tldr.md) [online](https://code.kx.com/q/learn/tour/tldr) TLDR
      - [local](./docs/learn/tour/index.md) [online](https://code.kx.com/q/learn/tour) Begin here
      - [local](./docs/learn/tour/session.md) [online](https://code.kx.com/q/learn/tour/session) The q session
      - [local](./docs/learn/tour/tables.md) [online](https://code.kx.com/q/learn/tour/tables) Tables
      - [local](./docs/learn/tour/csvs.md) [online](https://code.kx.com/q/learn/tour/csvs) CSVs
      - [local](./docs/learn/tour/datatypes.md) [online](https://code.kx.com/q/learn/tour/datatypes) Datatypes
      - [local](./docs/learn/tour/scripts.md) [online](https://code.kx.com/q/learn/tour/scripts) Scripts
      - [local](./docs/learn/tour/ide.md) [online](https://code.kx.com/q/learn/tour/ide) IDE
    - [local](./docs/learn/brief-introduction.md) [online](https://code.kx.com/q/learn/brief-introduction) Q for quants
    - [local](./docs/learn/q-by-examples.md) [online](https://code.kx.com/q/learn/q-by-examples) Q by Examples
    - [local](./docs/learn/q-for-all.md) [online](https://code.kx.com/q/learn/q-for-all) Q for All
    - Examples from Python:
      - [local](./docs/learn/python/examples/index.md) [online](https://code.kx.com/q/learn/python/examples) Basic
      - [local](./docs/learn/python/examples/array.md) [online](https://code.kx.com/q/learn/python/examples/array) Array
      - [local](./docs/learn/python/examples/list.md) [online](https://code.kx.com/q/learn/python/examples/list) List
      - [local](./docs/learn/python/examples/string.md) [online](https://code.kx.com/q/learn/python/examples/string) Strings
      - [local](./docs/learn/python/examples/dict.md) [online](https://code.kx.com/q/learn/python/examples/dict) Dictionaries
    - Q for Mortals 3: https://code.kx.com/q4m3/
    - Q by Puzzles:
      - [local](./docs/learn/pb/index.md) [online](https://code.kx.com/q/learn/pb) About
      - [local](./docs/learn/pb/xmas-days.md) [online](https://code.kx.com/q/learn/pb/xmas-days) 12 Days of Xmas
      - [local](./docs/learn/pb/abc-problem.md) [online](https://code.kx.com/q/learn/pb/abc-problem) ABC problem
      - [local](./docs/learn/pb/abundant-odds.md) [online](https://code.kx.com/q/learn/pb/abundant-odds) Abundant odds
      - [local](./docs/learn/pb/four-magic.md) [online](https://code.kx.com/q/learn/pb/four-magic) Four is magic
      - [local](./docs/learn/pb/name-game.md) [online](https://code.kx.com/q/learn/pb/name-game) Name Game
      - [local](./docs/learn/pb/sum-say.md) [online](https://code.kx.com/q/learn/pb/sum-say) Summarize and Say
      - [local](./docs/learn/pb/word-wheel.md) [online](https://code.kx.com/q/learn/pb/word-wheel) Word wheel
    - Reading room:
      - [local](./docs/learn/reading/index.md) [online](https://code.kx.com/q/learn/reading) Information desk
      - [local](./docs/learn/reading/boggle.md) [online](https://code.kx.com/q/learn/reading/boggle) Boggle
      - [local](./docs/learn/reading/strings.md) [online](https://code.kx.com/q/learn/reading/strings) Cats cradle
      - [local](./docs/learn/reading/fizzbuzz.md) [online](https://code.kx.com/q/learn/reading/fizzbuzz) Fizz buzz
      - [local](./docs/learn/reading/klondike.md) [online](https://code.kx.com/q/learn/reading/klondike) Klondike
      - Phrasebook: https://code.kx.com/phrases/
      - [local](./docs/learn/reading/scrabble.md) [online](https://code.kx.com/q/learn/reading/scrabble) Scrabble
    - Application examples:
      - [local](./docs/wp/astronomy.md) [online](https://code.kx.com/q/wp/astronomy) Astronomy (WP)
      - [local](./docs/wp/blockchain/index.md) [online](https://code.kx.com/q/wp/blockchain) Bitcoin blockchains (WP)
      - [local](./docs/wp/card-counters/index.md) [online](https://code.kx.com/q/wp/card-counters) Card counters (WP)
      - [local](./docs/wp/corporate-actions.md) [online](https://code.kx.com/q/wp/corporate-actions) Corporate actions (WP)
      - [local](./docs/wp/disaster-management/index.md) [online](https://code.kx.com/q/wp/disaster-management) Disaster management (WP)
      - [local](./docs/wp/exoplanets/index.md) [online](https://code.kx.com/q/wp/exoplanets) Exoplanets (WP)
      - [local](./docs/wp/market-depth/index.md) [online](https://code.kx.com/q/wp/market-depth) Market depth (WP)
      - [local](./docs/wp/market-fragmentation/index.md) [online](https://code.kx.com/q/wp/market-fragmentation) Market fragmentation (WP)
      - [local](./docs/wp/option-pricing/index.md) [online](https://code.kx.com/q/wp/option-pricing) Option pricing (WP)
      - [local](./docs/wp/disaster-floods/index.md) [online](https://code.kx.com/q/wp/disaster-floods) Predicting floods (WP)
      - [local](./docs/wp/signal-processing/index.md) [online](https://code.kx.com/q/wp/signal-processing) Signal processing (WP)
      - [local](./docs/wp/space-weather/index.md) [online](https://code.kx.com/q/wp/space-weather) Space weather (WP)
      - [local](./docs/wp/surveillance/index.md) [online](https://code.kx.com/q/wp/surveillance) Trading surveillance (WP)
      - [local](./docs/wp/transaction-cost.md) [online](https://code.kx.com/q/wp/transaction-cost) Transaction-cost analysis (WP)
      - [local](./docs/wp/trend-indicators/index.md) [online](https://code.kx.com/q/wp/trend-indicators) 😀Trend indicators (WP)
    - Advanced q:
      - Remarks on Style: https://github.com/qbists/style
      - [local](./docs/learn/shifts-scans.md) [online](https://code.kx.com/q/learn/shifts-scans) Shifts & scans
      - [local](./docs/learn/blogs.md) [online](https://code.kx.com/q/learn/blogs) Technical articles
      - [local](./docs/learn/views.md) [online](https://code.kx.com/q/learn/views) Views
      - [local](./docs/learn/archive.md) [online](https://code.kx.com/q/learn/archive) Origins
      - [local](./docs/about/terminology.md) [online](https://code.kx.com/q/about/terminology) Terminology
    - Starting kdb+:
      - [local](./docs/learn/startingkdb/index.md) [online](https://code.kx.com/q/learn/startingkdb) Overview
      - [local](./docs/learn/startingkdb/language.md) [online](https://code.kx.com/q/learn/startingkdb/language) The q language
      - [local](./docs/learn/startingkdb/ipc.md) [online](https://code.kx.com/q/learn/startingkdb/ipc) IPC
      - [local](./docs/learn/startingkdb/tables.md) [online](https://code.kx.com/q/learn/startingkdb/tables) Tables
      - [local](./docs/learn/startingkdb/hdb.md) [online](https://code.kx.com/q/learn/startingkdb/hdb) Historical database
      - [local](./docs/learn/startingkdb/tick.md) [online](https://code.kx.com/q/learn/startingkdb/tick) Realtime database
  - # kdb+ and q: 
    - [local](./docs/index.md) [online](https://code.kx.com/q) About
    - [local](./docs/ref/index.md) [online](https://code.kx.com/q/ref) Reference card
    - [local](./docs/devtools.md) [online](https://code.kx.com/q/devtools) Developer tools
    - Interfaces: 
      - [local](./docs/interfaces/index.md) [online](https://code.kx.com/q/interfaces) KX libraries
      - [local](./docs/interfaces/q-client-for-bloomberg.md) [online](https://code.kx.com/q/interfaces/q-client-for-bloomberg) Bloomberg
      - C/C++:
        - [local](./docs/interfaces/c-client-for-q.md) [online](https://code.kx.com/q/interfaces/c-client-for-q) Quick guide
        - [local](./docs/interfaces/capiref.md) [online](https://code.kx.com/q/interfaces/capiref) API reference
        - [local](./docs/wp/capi/index.md) [online](https://code.kx.com/q/wp/capi) C API for kdb+ (WP)
        - [local](./docs/interfaces/using-c-functions.md) [online](https://code.kx.com/q/interfaces/using-c-functions) Using C/C++ functions
      - [local](./docs/interfaces/excel-client-for-q.md) [online](https://code.kx.com/q/interfaces/excel-client-for-q) Excel
      - [local](./docs/wp/fix-messaging.md) [online](https://code.kx.com/q/wp/fix-messaging) FIX messaging (WP)
      - [local](./docs/interfaces/gpus.md) [online](https://code.kx.com/q/interfaces/gpus) GPUs
      - [local](./docs/wp/lightning-tickerplants/index.md) [online](https://code.kx.com/q/wp/lightning-tickerplants) Lightning tickerplants (WP)
      - [local](./docs/interfaces/matlab-client-for-q.md) [online](https://code.kx.com/q/interfaces/matlab-client-for-q) Matlab
      - [local](./docs/interfaces/q-server-for-odbc3.md) [online](https://code.kx.com/q/interfaces/q-server-for-odbc3) ODBC3
      - [local](./docs/interfaces/odbc-simba.md) [online](https://code.kx.com/q/interfaces/odbc-simba) ODBC/Simba
      - [local](./docs/interfaces/r.md) [online](https://code.kx.com/q/interfaces/r) R
      - [local](./docs/interfaces/scala-client-for-q.md) [online](https://code.kx.com/q/interfaces/scala-client-for-q) Scala
    - [local](./docs/github.md) [online](https://code.kx.com/q/github) Open source
    - [local](./docs/ml.md) [online](https://code.kx.com/q/ml) Machine learning
    - Cloud: https://code.kx.com/insights/core/
    - Community: https://code.kx.com/home/community/
    - kdb+ and q forum: https://community.kx.com/t5/kdb-and-q/bd-p/kdb-q-questions
    - [local](./docs/wp/index.md) [online](https://code.kx.com/q/wp) White papers
    - [local](./docs/about/thissite.md) [online](https://code.kx.com/q/about/thissite) About this site
  - # Architecture:
    - [local](./docs/architecture/index.md) [online](https://code.kx.com/q/architecture) About
    - [local](./docs/architecture/examples.md) [online](https://code.kx.com/q/architecture/examples) Examples
    - [local](./docs/kb/alternative-in-memory-layouts.md) [online](https://code.kx.com/q/kb/alternative-in-memory-layouts) Alternative in-memory layouts
    - [local](./docs/kb/chained-tickerplant.md) [online](https://code.kx.com/q/kb/chained-tickerplant) Chained tickerplant
    - [local](./docs/kb/client-server.md) [online](https://code.kx.com/q/kb/client-server) Client-server
    - [local](./docs/kb/corporate-actions.md) [online](https://code.kx.com/q/kb/corporate-actions) Corporate actions
    - [local](./docs/wp/data-recovery.md) [online](https://code.kx.com/q/wp/data-recovery) Data recovery for kdb+tick (WP)
    - [local](./docs/wp/disaster-recovery/index.md) [online](https://code.kx.com/q/wp/disaster-recovery) Disaster recovery (WP)
    - [local](./docs/wp/gateway-design/index.md) [online](https://code.kx.com/q/wp/gateway-design) Gateway design (WP)
    - [local](./docs/kb/kdb-tick.md) [online](https://code.kx.com/q/kb/kdb-tick) Kdb+tick configuration
    - [local](./docs/wp/tick-profiling.md) [online](https://code.kx.com/q/wp/tick-profiling) Kdb+tick profiling (WP)
    - Kubernetes: 'https://youtu.be/jqtkkCqBvr4'
    - [local](./docs/kb/load-balancing.md) [online](https://code.kx.com/q/kb/load-balancing) Load balancing
    - [local](./docs/basics/memory-backed.md) [online](https://code.kx.com/q/basics/memory-backed) Memory backed by files
    - Optane Memory:
      - [local](./docs/kb/optane.md) [online](https://code.kx.com/q/kb/optane) Optane Memory and kdb+
      - [local](./docs/architecture/optane-tests.md) [online](https://code.kx.com/q/architecture/optane-tests) Performance tests
    - [local](./docs/wp/order-book.md) [online](https://code.kx.com/q/wp/order-book) Order Book (WP)
    - [local](./docs/kb/publish-subscribe.md) [online](https://code.kx.com/q/kb/publish-subscribe) Publish and subscribe
    - [local](./docs/wp/solace/index.md) [online](https://code.kx.com/q/wp/solace) Pub/sub with Solace (WP)
    - [local](./docs/wp/query-routing/index.md) [online](https://code.kx.com/q/wp/query-routing) Query Routing (WP)
    - [local](./docs/wp/rt-tick/index.md) [online](https://code.kx.com/q/wp/rt-tick) Real-time tick subscribers (WP)
    - [local](./docs/wp/websockets/index.md) [online](https://code.kx.com/q/wp/websockets) WebSockets (WP)
    - [local](./docs/kb/w-q.md) [online](https://code.kx.com/q/kb/w-q) Write-only RDB
    - Advanced:
      - [local](./docs/wp/query-interface.md) [online](https://code.kx.com/q/wp/query-interface) Distributed systems (WP)
      - [local](./docs/wp/intraday-writedown/index.md) [online](https://code.kx.com/q/wp/intraday-writedown) Intraday writedown (WP)
  - # Database:
    - [local](./docs/database/index.md) [online](https://code.kx.com/q/database) Tables in the filesystem
    - Populating tables:
      - [local](./docs/kb/loading-from-large-files.md) [online](https://code.kx.com/q/kb/loading-from-large-files) Loading from large files
      - [local](./docs/wp/foreign-keys.md) [online](https://code.kx.com/q/wp/foreign-keys) Foreign keys (WP)
      - [local](./docs/kb/linking-columns.md) [online](https://code.kx.com/q/kb/linking-columns) Linking columns
      - [local](./docs/wp/data-loaders/index.md) [online](https://code.kx.com/q/wp/data-loaders) Data loaders (WP)
      - [local](./docs/database/mdb-odbc.md) [online](https://code.kx.com/q/database/mdb-odbc) From MDB via ODBC
    - Persisting tables:
      - [local](./docs/database/object.md) [online](https://code.kx.com/q/database/object) Serializing an object
      - [local](./docs/kb/splayed-tables.md) [online](https://code.kx.com/q/kb/splayed-tables) Splayed tables
      - [local](./docs/kb/partition.md) [online](https://code.kx.com/q/kb/partition) Partitioned tables
      - [local](./docs/database/segment.md) [online](https://code.kx.com/q/database/segment) Segmented databases
      - [local](./docs/wp/multi-partitioned-dbs/index.md) [online](https://code.kx.com/q/wp/multi-partitioned-dbs) Multiple partitions (WP)
    - Maintenance:
      - [local](./docs/wp/data-management.md) [online](https://code.kx.com/q/wp/data-management) Data management (WP)
      - [local](./docs/kb/dare.md) [online](https://code.kx.com/q/kb/dare) Data-At-Rest Encryption
      - [local](./docs/kb/file-compression.md) [online](https://code.kx.com/q/kb/file-compression) File compression
      - [local](./docs/wp/compress/index.md) [online](https://code.kx.com/q/wp/compress) Compression (WP)
      - [local](./docs/wp/permissions/index.md) [online](https://code.kx.com/q/wp/permissions) Permissions (WP)
      - [local](./docs/wp/columnar-database/index.md) [online](https://code.kx.com/q/wp/columnar-database) Query optimization (WP)
      - [local](./docs/wp/query-scaling.md) [online](https://code.kx.com/q/wp/query-scaling) Query scaling (WP)
      - [local](./docs/wp/ts-shrink/index.md) [online](https://code.kx.com/q/wp/ts-shrink) Time-series simplification (WP)
      - [local](./docs/kb/compacting-hdb-sym.md) [online](https://code.kx.com/q/kb/compacting-hdb-sym) Compacting HDB sym
      - [local](./docs/wp/symfiles.md) [online](https://code.kx.com/q/wp/symfiles) Working with sym files (WP)
  - # Developing:
    - IPC:
      - [local](./docs/basics/ipc.md) [online](https://code.kx.com/q/basics/ipc) Overview
      - [local](./docs/kb/callbacks.md) [online](https://code.kx.com/q/kb/callbacks) Callbacks
      - [local](./docs/basics/listening-port.md) [online](https://code.kx.com/q/basics/listening-port) Listening port
      - [local](./docs/kb/named-pipes.md) [online](https://code.kx.com/q/kb/named-pipes) Named pipes
      - [local](./docs/kb/serialization.md) [online](https://code.kx.com/q/kb/serialization) Serialization examples
      - [local](./docs/kb/server-calling-client.md) [online](https://code.kx.com/q/kb/server-calling-client) Server calling client
      - [local](./docs/wp/socket-sharding/index.md) [online](https://code.kx.com/q/wp/socket-sharding) Socket sharding (WP)
      - [local](./docs/kb/ssl.md) [online](https://code.kx.com/q/kb/ssl) SSL/TLS
      - [local](./docs/kb/websockets.md) [online](https://code.kx.com/q/kb/websockets) WebSockets
      - [local](./docs/wp/ipc/index.md) [online](https://code.kx.com/q/wp/ipc) Interprocess communication (WP)
    - Tools:
      - [local](./docs/kb/profiler.md) [online](https://code.kx.com/q/kb/profiler) Code profiler
      - [local](./docs/basics/debug.md) [online](https://code.kx.com/q/basics/debug) Debugging
      - [local](./docs/basics/errors.md) [online](https://code.kx.com/q/basics/errors) Errors
      - [local](./docs/about/man.md) [online](https://code.kx.com/q/about/man) man.q
      - [local](./docs/basics/syscmds.md) [online](https://code.kx.com/q/basics/syscmds) System commands
      - [local](./docs/kb/unit-tests.md) [online](https://code.kx.com/q/kb/unit-tests) Unit tests
      - [local](./docs/kb/using-dotz.md) [online](https://code.kx.com/q/kb/using-dotz) Using .z
    - Coding:
      - [local](./docs/wp/data-visualization/index.md) [online](https://code.kx.com/q/wp/data-visualization) Data visualization (WP)
      - [local](./docs/kb/deferred-response.md) [online](https://code.kx.com/q/kb/deferred-response) Deferred response
      - [local](./docs/kb/geospatial.md) [online](https://code.kx.com/q/kb/geospatial) Geospatial indexing
      - [local](./docs/kb/lp.md) [online](https://code.kx.com/q/kb/lp) Linear programming
      - [local](./docs/kb/multithreaded-input.md) [online](https://code.kx.com/q/kb/multithreaded-input) Multithreaded input
      - [local](./docs/kb/mt-primitives.md) [online](https://code.kx.com/q/kb/mt-primitives) Multithreaded primitives
      - [local](./docs/kb/pivoting-tables.md) [online](https://code.kx.com/q/kb/pivoting-tables) Pivoting tables
      - [local](./docs/basics/precision.md) [online](https://code.kx.com/q/basics/precision) Precision
      - [local](./docs/kb/programming-examples.md) [online](https://code.kx.com/q/kb/programming-examples) Programming examples
      - [local](./docs/kb/programming-idioms.md) [online](https://code.kx.com/q/kb/programming-idioms) Programming idioms
      - [local](./docs/kb/temporal-data.md) [online](https://code.kx.com/q/kb/temporal-data) Temporal data
      - [local](./docs/kb/timezones.md) [online](https://code.kx.com/q/kb/timezones) Timezones
      - [local](./docs/kb/unicode.md) [online](https://code.kx.com/q/kb/unicode) Unicode
    - DevOps:
      - [local](./docs/kb/authentication.md) [online](https://code.kx.com/q/kb/authentication) Authentication and access
      - [local](./docs/basics/cmdline.md) [online](https://code.kx.com/q/basics/cmdline) Command-line options
      - [local](./docs/kb/cpu-affinity.md) [online](https://code.kx.com/q/kb/cpu-affinity) CPU affinity
      - [local](./docs/kb/custom-web.md) [online](https://code.kx.com/q/kb/custom-web) Custom web server
      - [local](./docs/kb/daemon.md) [online](https://code.kx.com/q/kb/daemon) Daemon
      - [local](./docs/kb/firewalling.md) [online](https://code.kx.com/q/kb/firewalling) Firewalling
      - [local](./docs/kb/inetd.md) [online](https://code.kx.com/q/kb/inetd) inetd, xinetd
      - [local](./docs/kb/linux-production.md) [online](https://code.kx.com/q/kb/linux-production) Linux production notes
      - [local](./docs/kb/logging.md) [online](https://code.kx.com/q/kb/logging) Logging
      - [local](./docs/wp/multi-thread/index.md) [online](https://code.kx.com/q/wp/multi-thread) Multi-threading (WP)
      - [local](./docs/kb/versions.md) [online](https://code.kx.com/q/kb/versions) Multiple versions
      - [local](./docs/basics/peach.md) [online](https://code.kx.com/q/basics/peach) Parallel processing
      - [local](./docs/kb/performance-tips.md) [online](https://code.kx.com/q/kb/performance-tips) Performance tips
      - [local](./docs/kb/replay-log.md) [online](https://code.kx.com/q/kb/replay-log) Replay logfile
      - [local](./docs/develop/shebang.md) [online](https://code.kx.com/q/develop/shebang) Shebang script
      - [local](./docs/wp/surveillance-latency/index.md) [online](https://code.kx.com/q/wp/surveillance-latency) Surveillance latency (WP)
      - [local](./docs/kb/windows-service/index.md) [online](https://code.kx.com/q/kb/windows-service) Windows service
    - Release notes:
      - [local](./docs/releases/index.md) [online](https://code.kx.com/q/releases) History
      - [local](./docs/releases/ChangesIn4.0.md) [online](https://code.kx.com/q/releases/ChangesIn4.0) Changes in 4.0
      - [local](./docs/releases/ChangesIn3.6.md) [online](https://code.kx.com/q/releases/ChangesIn3.6) Changes in 3.6
      - [local](./docs/releases/ChangesIn3.5.md) [online](https://code.kx.com/q/releases/ChangesIn3.5) Changes in 3.5
      - [local](./docs/releases/ChangesIn3.4.md) [online](https://code.kx.com/q/releases/ChangesIn3.4) Changes in 3.4
      - [local](./docs/releases/ChangesIn3.3.md) [online](https://code.kx.com/q/releases/ChangesIn3.3) Changes in 3.3
      - [local](./docs/releases/ChangesIn3.2.md) [online](https://code.kx.com/q/releases/ChangesIn3.2) Changes in 3.2
      - [local](./docs/releases/ChangesIn3.1.md) [online](https://code.kx.com/q/releases/ChangesIn3.1) Changes in 3.1
      - [local](./docs/releases/ChangesIn3.0.md) [online](https://code.kx.com/q/releases/ChangesIn3.0) Changes in 3.0
      - [local](./docs/releases/ChangesIn2.8.md) [online](https://code.kx.com/q/releases/ChangesIn2.8) Changes in 2.8
      - [local](./docs/releases/ChangesIn2.7.md) [online](https://code.kx.com/q/releases/ChangesIn2.7) Changes in 2.7
      - [local](./docs/releases/ChangesIn2.6.md) [online](https://code.kx.com/q/releases/ChangesIn2.6) Changes in 2.6
      - [local](./docs/releases/ChangesIn2.5.md) [online](https://code.kx.com/q/releases/ChangesIn2.5) Changes in 2.5
      - [local](./docs/releases/ChangesIn2.4.md) [online](https://code.kx.com/q/releases/ChangesIn2.4) Changes in 2.4
      - [local](./docs/releases/withdrawn.md) [online](https://code.kx.com/q/releases/withdrawn) Withdrawn
    - [local](./docs/kb/faq-listbox.md) [online](https://code.kx.com/q/kb/faq-listbox) FAQ
  - # Language: 
    - [local](./docs/ref/index.md) [online](https://code.kx.com/q/ref) Reference card
    - [local](./docs/basics/by-topic.md) [online](https://code.kx.com/q/basics/by-topic) By topic
    - Iteration:
      - [local](./docs/basics/iteration.md) [online](https://code.kx.com/q/basics/iteration) Overview
      - [local](./docs/basics/implicit-iteration.md) [online](https://code.kx.com/q/basics/implicit-iteration) Implicit iteration
      - [local](./docs/ref/iterators.md) [online](https://code.kx.com/q/ref/iterators) Iterators
      - [local](./docs/ref/maps.md) [online](https://code.kx.com/q/ref/maps) Maps
      - [local](./docs/ref/accumulators.md) [online](https://code.kx.com/q/ref/accumulators) Accumulators
      - [local](./docs/wp/iterators/index.md) [online](https://code.kx.com/q/wp/iterators) Guide to iterators (WP)
    - Keywords:
      - [local](./docs/ref/abs.md) [online](https://code.kx.com/q/ref/abs) abs
      - [local](./docs/ref/aj.md) [online](https://code.kx.com/q/ref/aj) aj, aj0, ajf, ajf0
      - [local](./docs/ref/all-any.md) [online](https://code.kx.com/q/ref/all-any) all, any
      - [local](./docs/ref/and.md) [online](https://code.kx.com/q/ref/and) and
      - [local](./docs/ref/asc.md) [online](https://code.kx.com/q/ref/asc) asc, iasc, xasc
      - [local](./docs/ref/asof.md) [online](https://code.kx.com/q/ref/asof) asof
      - [local](./docs/ref/attr.md) [online](https://code.kx.com/q/ref/attr) attr
      - [local](./docs/ref/avg.md) [online](https://code.kx.com/q/ref/avg) avg, avgs, mavg, wavg
      - [local](./docs/ref/bin.md) [online](https://code.kx.com/q/ref/bin) bin, binr
      - [local](./docs/ref/ceiling.md) [online](https://code.kx.com/q/ref/ceiling) ceiling
      - [local](./docs/ref/count.md) [online](https://code.kx.com/q/ref/count) count, mcount
      - [local](./docs/ref/cols.md) [online](https://code.kx.com/q/ref/cols) cols, xcol, xcols
      - [local](./docs/ref/cor.md) [online](https://code.kx.com/q/ref/cor) cor
      - [local](./docs/ref/cos.md) [online](https://code.kx.com/q/ref/cos) cos, acos
      - [local](./docs/ref/cov.md) [online](https://code.kx.com/q/ref/cov) cov, scov
      - [local](./docs/ref/cross.md) [online](https://code.kx.com/q/ref/cross) cross
      - [local](./docs/ref/csv.md) [online](https://code.kx.com/q/ref/csv) csv
      - [local](./docs/ref/cut.md) [online](https://code.kx.com/q/ref/cut) cut
      - [local](./docs/ref/delete.md) [online](https://code.kx.com/q/ref/delete) delete
      - [local](./docs/ref/deltas.md) [online](https://code.kx.com/q/ref/deltas) deltas
      - [local](./docs/ref/desc.md) [online](https://code.kx.com/q/ref/desc) desc, idesc, xdesc
      - [local](./docs/ref/dev.md) [online](https://code.kx.com/q/ref/dev) dev, mdev, sdev
      - [local](./docs/ref/differ.md) [online](https://code.kx.com/q/ref/differ) differ
      - [local](./docs/ref/distinct.md) [online](https://code.kx.com/q/ref/distinct) distinct
      - [local](./docs/ref/div.md) [online](https://code.kx.com/q/ref/div) div
      - [local](./docs/ref/dsave.md) [online](https://code.kx.com/q/ref/dsave) dsave
      - [local](./docs/ref/each.md) [online](https://code.kx.com/q/ref/each) each, peach
      - [local](./docs/ref/ej.md) [online](https://code.kx.com/q/ref/ej) ej
      - [local](./docs/ref/ema.md) [online](https://code.kx.com/q/ref/ema) ema
      - [local](./docs/ref/enlist.md) [online](https://code.kx.com/q/ref/enlist) enlist
      - [local](./docs/ref/eval.md) [online](https://code.kx.com/q/ref/eval) eval, reval
      - [local](./docs/ref/except.md) [online](https://code.kx.com/q/ref/except) except
      - [local](./docs/ref/exec.md) [online](https://code.kx.com/q/ref/exec) exec
      - [local](./docs/ref/exit.md) [online](https://code.kx.com/q/ref/exit) exit
      - [local](./docs/ref/exp.md) [online](https://code.kx.com/q/ref/exp) exp, xexp
      - [local](./docs/ref/fby.md) [online](https://code.kx.com/q/ref/fby) fby
      - [local](./docs/ref/fill.md) [online](https://code.kx.com/q/ref/fill) fills
      - [local](./docs/ref/first.md) [online](https://code.kx.com/q/ref/first) first, last
      - [local](./docs/ref/fkeys.md) [online](https://code.kx.com/q/ref/fkeys) fkeys
      - [local](./docs/ref/flip.md) [online](https://code.kx.com/q/ref/flip) flip
      - [local](./docs/ref/floor.md) [online](https://code.kx.com/q/ref/floor) floor
      - [local](./docs/ref/get.md) [online](https://code.kx.com/q/ref/get) get, set
      - [local](./docs/ref/getenv.md) [online](https://code.kx.com/q/ref/getenv) getenv, setenv
      - [local](./docs/ref/group.md) [online](https://code.kx.com/q/ref/group) group
      - [local](./docs/ref/gtime.md) [online](https://code.kx.com/q/ref/gtime) gtime, ltime
      - [local](./docs/ref/hcount.md) [online](https://code.kx.com/q/ref/hcount) hcount
      - [local](./docs/ref/hdel.md) [online](https://code.kx.com/q/ref/hdel) hdel
      - [local](./docs/ref/hopen.md) [online](https://code.kx.com/q/ref/hopen) hopen, hclose
      - [local](./docs/ref/hsym.md) [online](https://code.kx.com/q/ref/hsym) hsym
      - [local](./docs/ref/ij.md) [online](https://code.kx.com/q/ref/ij) ij, ijf
      - [local](./docs/ref/in.md) [online](https://code.kx.com/q/ref/in) in
      - [local](./docs/ref/insert.md) [online](https://code.kx.com/q/ref/insert) insert
      - [local](./docs/ref/inter.md) [online](https://code.kx.com/q/ref/inter) inter
      - [local](./docs/ref/inv.md) [online](https://code.kx.com/q/ref/inv) inv
      - [local](./docs/ref/key.md) [online](https://code.kx.com/q/ref/key) key
      - [local](./docs/ref/keys.md) [online](https://code.kx.com/q/ref/keys) keys, xkey
      - [local](./docs/ref/like.md) [online](https://code.kx.com/q/ref/like) like
      - [local](./docs/ref/lj.md) [online](https://code.kx.com/q/ref/lj) lj, ljf
      - [local](./docs/ref/load.md) [online](https://code.kx.com/q/ref/load) load, rload
      - [local](./docs/ref/log.md) [online](https://code.kx.com/q/ref/log) log, xlog
      - [local](./docs/ref/lower.md) [online](https://code.kx.com/q/ref/lower) lower
      - [local](./docs/ref/lsq.md) [online](https://code.kx.com/q/ref/lsq) lsq
      - [local](./docs/ref/max.md) [online](https://code.kx.com/q/ref/max) max, maxs, mmax
      - [local](./docs/ref/md5.md) [online](https://code.kx.com/q/ref/md5) md5
      - [local](./docs/ref/med.md) [online](https://code.kx.com/q/ref/med) med
      - [local](./docs/ref/meta.md) [online](https://code.kx.com/q/ref/meta) meta
      - [local](./docs/ref/min.md) [online](https://code.kx.com/q/ref/min) min, mins, mmin
      - [local](./docs/ref/mmu.md) [online](https://code.kx.com/q/ref/mmu) mmu
      - [local](./docs/ref/mod.md) [online](https://code.kx.com/q/ref/mod) mod
      - [local](./docs/ref/neg.md) [online](https://code.kx.com/q/ref/neg) neg
      - [local](./docs/ref/next.md) [online](https://code.kx.com/q/ref/next) next, prev, xprev
      - [local](./docs/ref/not.md) [online](https://code.kx.com/q/ref/not) not
      - [local](./docs/ref/null.md) [online](https://code.kx.com/q/ref/null) 'null'
      - [local](./docs/ref/or.md) [online](https://code.kx.com/q/ref/or) or
      - [local](./docs/ref/over.md) [online](https://code.kx.com/q/ref/over) over, scan
      - [local](./docs/ref/parse.md) [online](https://code.kx.com/q/ref/parse) parse
      - [local](./docs/ref/pj.md) [online](https://code.kx.com/q/ref/pj) pj
      - [local](./docs/ref/prd.md) [online](https://code.kx.com/q/ref/prd) prd, prds
      - [local](./docs/ref/prior.md) [online](https://code.kx.com/q/ref/prior) prior
      - [local](./docs/ref/rand.md) [online](https://code.kx.com/q/ref/rand) rand
      - [local](./docs/ref/rank.md) [online](https://code.kx.com/q/ref/rank) rank
      - [local](./docs/ref/ratios.md) [online](https://code.kx.com/q/ref/ratios) ratios
      - [local](./docs/ref/raze.md) [online](https://code.kx.com/q/ref/raze) raze
      - [local](./docs/ref/read0.md) [online](https://code.kx.com/q/ref/read0) read0
      - [local](./docs/ref/read1.md) [online](https://code.kx.com/q/ref/read1) read1
      - [local](./docs/ref/reciprocal.md) [online](https://code.kx.com/q/ref/reciprocal) reciprocal
      - [local](./docs/ref/reverse.md) [online](https://code.kx.com/q/ref/reverse) reverse
      - [local](./docs/ref/rotate.md) [online](https://code.kx.com/q/ref/rotate) rotate
      - [local](./docs/ref/save.md) [online](https://code.kx.com/q/ref/save) save, rsave
      - [local](./docs/ref/select.md) [online](https://code.kx.com/q/ref/select) select
      - [local](./docs/ref/show.md) [online](https://code.kx.com/q/ref/show) show
      - [local](./docs/ref/signum.md) [online](https://code.kx.com/q/ref/signum) signum
      - [local](./docs/ref/sin.md) [online](https://code.kx.com/q/ref/sin) sin, asin
      - [local](./docs/ref/sqrt.md) [online](https://code.kx.com/q/ref/sqrt) sqrt
      - [local](./docs/ref/ss.md) [online](https://code.kx.com/q/ref/ss) ss, ssr
      - [local](./docs/ref/string.md) [online](https://code.kx.com/q/ref/string) string
      - [local](./docs/ref/sublist.md) [online](https://code.kx.com/q/ref/sublist) sublist
      - [local](./docs/ref/sum.md) [online](https://code.kx.com/q/ref/sum) sum, sums, msum, wsum
      - [local](./docs/ref/sv.md) [online](https://code.kx.com/q/ref/sv) sv
      - [local](./docs/ref/system.md) [online](https://code.kx.com/q/ref/system) system
      - [local](./docs/ref/tables.md) [online](https://code.kx.com/q/ref/tables) tables
      - [local](./docs/ref/tan.md) [online](https://code.kx.com/q/ref/tan) tan, atan
      - [local](./docs/ref/til.md) [online](https://code.kx.com/q/ref/til) til
      - [local](./docs/ref/trim.md) [online](https://code.kx.com/q/ref/trim) trim, ltrim, rtrim
      - [local](./docs/ref/type.md) [online](https://code.kx.com/q/ref/type) type
      - [local](./docs/ref/uj.md) [online](https://code.kx.com/q/ref/uj) uj, ujf
      - [local](./docs/ref/union.md) [online](https://code.kx.com/q/ref/union) union
      - [local](./docs/ref/ungroup.md) [online](https://code.kx.com/q/ref/ungroup) ungroup
      - [local](./docs/ref/update.md) [online](https://code.kx.com/q/ref/update) update
      - [local](./docs/ref/upsert.md) [online](https://code.kx.com/q/ref/upsert) upsert
      - [local](./docs/ref/value.md) [online](https://code.kx.com/q/ref/value) value
      - [local](./docs/ref/var.md) [online](https://code.kx.com/q/ref/var) var, svar
      - [local](./docs/ref/view.md) [online](https://code.kx.com/q/ref/view) view, views
      - [local](./docs/ref/vs.md) [online](https://code.kx.com/q/ref/vs) vs
      - [local](./docs/ref/where.md) [online](https://code.kx.com/q/ref/where) where
      - [local](./docs/ref/within.md) [online](https://code.kx.com/q/ref/within) within
      - [local](./docs/ref/wj.md) [online](https://code.kx.com/q/ref/wj) wj, wj1
      - [local](./docs/ref/xbar.md) [online](https://code.kx.com/q/ref/xbar) xbar
      - [local](./docs/ref/xgroup.md) [online](https://code.kx.com/q/ref/xgroup) xgroup
      - [local](./docs/ref/xrank.md) [online](https://code.kx.com/q/ref/xrank) xrank
    - [local](./docs/ref/overloads.md) [online](https://code.kx.com/q/ref/overloads) Overloaded glyphs
    - Operators:
      - [local](./docs/ref/add.md) [online](https://code.kx.com/q/ref/add) Add
      - [local](./docs/ref/amend.md) [online](https://code.kx.com/q/ref/amend) Amend
      - [local](./docs/ref/apply.md) [online](https://code.kx.com/q/ref/apply) Apply, Index, Trap
      - [local](./docs/ref/assign.md) [online](https://code.kx.com/q/ref/assign) Assign
      - [local](./docs/ref/cast.md) [online](https://code.kx.com/q/ref/cast) Cast
      - [local](./docs/ref/coalesce.md) [online](https://code.kx.com/q/ref/coalesce) Coalesce
      - [local](./docs/ref/compose.md) [online](https://code.kx.com/q/ref/compose) Compose
      - [local](./docs/ref/cut.md) [online](https://code.kx.com/q/ref/cut) Cut
      - [local](./docs/ref/deal.md) [online](https://code.kx.com/q/ref/deal) Deal, Roll, Permute
      - [local](./docs/ref/delete.md) [online](https://code.kx.com/q/ref/delete) Delete
      - [local](./docs/ref/display.md) [online](https://code.kx.com/q/ref/display) Display
      - [local](./docs/ref/dict.md) [online](https://code.kx.com/q/ref/dict) Dict
      - [local](./docs/ref/divide.md) [online](https://code.kx.com/q/ref/divide) Divide
      - [local](./docs/ref/dynamic-load.md) [online](https://code.kx.com/q/ref/dynamic-load) Dynamic Load
      - [local](./docs/ref/drop.md) [online](https://code.kx.com/q/ref/drop) Drop
      - [local](./docs/ref/enkey.md) [online](https://code.kx.com/q/ref/enkey) Enkey, Unkey
      - [local](./docs/ref/enumerate.md) [online](https://code.kx.com/q/ref/enumerate) Enumerate
      - [local](./docs/ref/enumeration.md) [online](https://code.kx.com/q/ref/enumeration) Enumeration
      - [local](./docs/ref/enum-extend.md) [online](https://code.kx.com/q/ref/enum-extend) Enum Extend
      - [local](./docs/ref/equal.md) [online](https://code.kx.com/q/ref/equal) Equal
      - [local](./docs/ref/exec.md) [online](https://code.kx.com/q/ref/exec) Exec
      - [local](./docs/ref/file-binary.md) [online](https://code.kx.com/q/ref/file-binary) File Binary
      - [local](./docs/ref/file-text.md) [online](https://code.kx.com/q/ref/file-text) File Text
      - [local](./docs/ref/fill.md) [online](https://code.kx.com/q/ref/fill) Fill
      - [local](./docs/ref/find.md) [online](https://code.kx.com/q/ref/find) Find
      - [local](./docs/ref/flip-splayed.md) [online](https://code.kx.com/q/ref/flip-splayed) Flip Splayed
      - [local](./docs/ref/greater.md) [online](https://code.kx.com/q/ref/greater) Greater
      - [local](./docs/ref/greater-than.md) [online](https://code.kx.com/q/ref/greater-than) Greater Than
      - [local](./docs/ref/identity.md) [online](https://code.kx.com/q/ref/identity) Identity, Null
      - [local](./docs/ref/join.md) [online](https://code.kx.com/q/ref/join) Join
      - [local](./docs/ref/less-than.md) [online](https://code.kx.com/q/ref/less-than) Less Than
      - [local](./docs/ref/lesser.md) [online](https://code.kx.com/q/ref/lesser) Lesser
      - [local](./docs/ref/match.md) [online](https://code.kx.com/q/ref/match) Match
      - [local](./docs/ref/mmu.md) [online](https://code.kx.com/q/ref/mmu) Matrix Multiply
      - [local](./docs/ref/multiply.md) [online](https://code.kx.com/q/ref/multiply) Multiply
      - [local](./docs/ref/not-equal.md) [online](https://code.kx.com/q/ref/not-equal) Not Equal
      - [local](./docs/ref/pad.md) [online](https://code.kx.com/q/ref/pad) Pad
      - [local](./docs/ref/select.md) [online](https://code.kx.com/q/ref/select) Select
      - [local](./docs/ref/set-attribute.md) [online](https://code.kx.com/q/ref/set-attribute) Set Attribute
      - [local](./docs/ref/simple-exec.md) [online](https://code.kx.com/q/ref/simple-exec) Simple Exec
      - [local](./docs/ref/signal.md) [online](https://code.kx.com/q/ref/signal) Signal
      - [local](./docs/ref/subtract.md) [online](https://code.kx.com/q/ref/subtract) Subtract
      - [local](./docs/ref/take.md) [online](https://code.kx.com/q/ref/take) Take
      - [local](./docs/ref/tok.md) [online](https://code.kx.com/q/ref/tok) Tok
      - [local](./docs/ref/update.md) [online](https://code.kx.com/q/ref/update) Update
      - [local](./docs/ref/vector-conditional.md) [online](https://code.kx.com/q/ref/vector-conditional) Vector Conditional
    - Control constructs:
      - [local](./docs/ref/cond.md) [online](https://code.kx.com/q/ref/cond) Cond
      - [local](./docs/ref/do.md) [online](https://code.kx.com/q/ref/do) do
      - [local](./docs/ref/if.md) [online](https://code.kx.com/q/ref/if) if
      - [local](./docs/ref/while.md) [online](https://code.kx.com/q/ref/while) while
    - Namespaces:
      - [local](./docs/ref/doth.md) [online](https://code.kx.com/q/ref/doth) .h
      - [local](./docs/ref/dotj.md) [online](https://code.kx.com/q/ref/dotj) .j
      - [local](./docs/ref/dotm.md) [online](https://code.kx.com/q/ref/dotm) .m
      - [local](./docs/ref/dotq.md) [online](https://code.kx.com/q/ref/dotq) .Q
      - [local](./docs/ref/dotz.md) [online](https://code.kx.com/q/ref/dotz) .z
    - [local](./docs/basics/application.md) [online](https://code.kx.com/q/basics/application) Application
    - [local](./docs/basics/atomic.md) [online](https://code.kx.com/q/basics/atomic) Atomic functions
    - [local](./docs/basics/comparison.md) [online](https://code.kx.com/q/basics/comparison) Comparison
    - [local](./docs/basics/conformable.md) [online](https://code.kx.com/q/basics/conformable) Conformability
    - [local](./docs/basics/handles.md) [online](https://code.kx.com/q/basics/handles) Connection handles
    - [local](./docs/basics/datatypes.md) [online](https://code.kx.com/q/basics/datatypes) Datatypes
    - [local](./docs/basics/dictsandtables.md) [online](https://code.kx.com/q/basics/dictsandtables) Dictionaries
    - [local](./docs/basics/enumerations.md) [online](https://code.kx.com/q/basics/enumerations) Enumerations
    - [local](./docs/basics/control.md) [online](https://code.kx.com/q/basics/control) Evaluation control
    - [local](./docs/basics/exposed-infrastructure.md) [online](https://code.kx.com/q/basics/exposed-infrastructure) Exposed infrastructure
    - [local](./docs/basics/files.md) [online](https://code.kx.com/q/basics/files) File system
    - [local](./docs/basics/function-notation.md) [online](https://code.kx.com/q/basics/function-notation) Function notation
    - [local](./docs/basics/funsql.md) [online](https://code.kx.com/q/basics/funsql) Functional qSQL
    - [local](./docs/basics/glossary.md) [online](https://code.kx.com/q/basics/glossary) Glossary
    - [local](./docs/basics/internal.md) [online](https://code.kx.com/q/basics/internal) Internal functions
    - [local](./docs/basics/joins.md) [online](https://code.kx.com/q/basics/joins) Joins
    - [local](./docs/basics/math.md) [online](https://code.kx.com/q/basics/math) Mathematics
    - [local](./docs/basics/metadata.md) [online](https://code.kx.com/q/basics/metadata) Metadata
    - [local](./docs/basics/namespaces.md) [online](https://code.kx.com/q/basics/namespaces) Namespaces
    - [local](./docs/basics/parsetrees.md) [online](https://code.kx.com/q/basics/parsetrees) Parse trees
    - [local](./docs/wp/parse-trees.md) [online](https://code.kx.com/q/wp/parse-trees) Parse trees, functional SQL (WP)
    - [local](./docs/basics/qsql.md) [online](https://code.kx.com/q/basics/qsql) QSQL queries
    - [local](./docs/basics/regex.md) [online](https://code.kx.com/q/basics/regex) Regular Expressions
    - [local](./docs/basics/syntax.md) [online](https://code.kx.com/q/basics/syntax) Syntax
    - [local](./docs/kb/faq.md) [online](https://code.kx.com/q/kb/faq) Tables
    - [local](./docs/basics/variadic.md) [online](https://code.kx.com/q/basics/variadic) Variadic syntax
  - # kdb Insights: https://code.kx.com/insights/insights
  - # kdb Insights Enterprise: https://code.kx.com/insights/platform
  - # Help: https://code.kx.com/home/support/