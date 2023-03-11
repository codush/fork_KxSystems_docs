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
    - [L](./docs/learn/index.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/learn/index.md) [O](https://code.kx.com/q/learn) Get started
    - [L](./docs/learn/install.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/learn/install.md) [O](https://code.kx.com/q/learn/install) 😀Install
    - [L](./docs/learn/licensing.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/learn/licensing.md) [O](https://code.kx.com/q/learn/licensing) Licenses
    - Mountain tour:
      - [L](./docs/learn/tour/tldr.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/learn/tour/tldr.md) [O](https://code.kx.com/q/learn/tour/tldr) TLDR
      - [L](./docs/learn/tour/index.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/learn/tour/index.md) [O](https://code.kx.com/q/learn/tour) Begin here
      - [L](./docs/learn/tour/session.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/learn/tour/session.md) [O](https://code.kx.com/q/learn/tour/session) The q session
      - [L](./docs/learn/tour/tables.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/learn/tour/tables.md) [O](https://code.kx.com/q/learn/tour/tables) Tables
      - [L](./docs/learn/tour/csvs.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/learn/tour/csvs.md) [O](https://code.kx.com/q/learn/tour/csvs) CSVs
      - [L](./docs/learn/tour/datatypes.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/learn/tour/datatypes.md) [O](https://code.kx.com/q/learn/tour/datatypes) Datatypes
      - [L](./docs/learn/tour/scripts.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/learn/tour/scripts.md) [O](https://code.kx.com/q/learn/tour/scripts) Scripts
      - [L](./docs/learn/tour/ide.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/learn/tour/ide.md) [O](https://code.kx.com/q/learn/tour/ide) IDE
    - [L](./docs/learn/brief-introduction.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/learn/brief-introduction.md) [O](https://code.kx.com/q/learn/brief-introduction) Q for quants
    - [L](./docs/learn/q-by-examples.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/learn/q-by-examples.md) [O](https://code.kx.com/q/learn/q-by-examples) Q by Examples
    - [L](./docs/learn/q-for-all.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/learn/q-for-all.md) [O](https://code.kx.com/q/learn/q-for-all) Q for All
    - Examples from Python:
      - [L](./docs/learn/python/examples/index.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/learn/python/examples/index.md) [O](https://code.kx.com/q/learn/python/examples) Basic
      - [L](./docs/learn/python/examples/array.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/learn/python/examples/array.md) [O](https://code.kx.com/q/learn/python/examples/array) Array
      - [L](./docs/learn/python/examples/list.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/learn/python/examples/list.md) [O](https://code.kx.com/q/learn/python/examples/list) List
      - [L](./docs/learn/python/examples/string.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/learn/python/examples/string.md) [O](https://code.kx.com/q/learn/python/examples/string) Strings
      - [L](./docs/learn/python/examples/dict.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/learn/python/examples/dict.md) [O](https://code.kx.com/q/learn/python/examples/dict) Dictionaries
    - Q for Mortals 3: https://code.kx.com/q4m3/
    - Q by Puzzles:
      - [L](./docs/learn/pb/index.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/learn/pb/index.md) [O](https://code.kx.com/q/learn/pb) About
      - [L](./docs/learn/pb/xmas-days.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/learn/pb/xmas-days.md) [O](https://code.kx.com/q/learn/pb/xmas-days) 12 Days of Xmas
      - [L](./docs/learn/pb/abc-problem.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/learn/pb/abc-problem.md) [O](https://code.kx.com/q/learn/pb/abc-problem) ABC problem
      - [L](./docs/learn/pb/abundant-odds.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/learn/pb/abundant-odds.md) [O](https://code.kx.com/q/learn/pb/abundant-odds) Abundant odds
      - [L](./docs/learn/pb/four-magic.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/learn/pb/four-magic.md) [O](https://code.kx.com/q/learn/pb/four-magic) Four is magic
      - [L](./docs/learn/pb/name-game.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/learn/pb/name-game.md) [O](https://code.kx.com/q/learn/pb/name-game) Name Game
      - [L](./docs/learn/pb/sum-say.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/learn/pb/sum-say.md) [O](https://code.kx.com/q/learn/pb/sum-say) Summarize and Say
      - [L](./docs/learn/pb/word-wheel.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/learn/pb/word-wheel.md) [O](https://code.kx.com/q/learn/pb/word-wheel) Word wheel
    - Reading room:
      - [L](./docs/learn/reading/index.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/learn/reading/index.md) [O](https://code.kx.com/q/learn/reading) Information desk
      - [L](./docs/learn/reading/boggle.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/learn/reading/boggle.md) [O](https://code.kx.com/q/learn/reading/boggle) Boggle
      - [L](./docs/learn/reading/strings.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/learn/reading/strings.md) [O](https://code.kx.com/q/learn/reading/strings) Cats cradle
      - [L](./docs/learn/reading/fizzbuzz.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/learn/reading/fizzbuzz.md) [O](https://code.kx.com/q/learn/reading/fizzbuzz) Fizz buzz
      - [L](./docs/learn/reading/klondike.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/learn/reading/klondike.md) [O](https://code.kx.com/q/learn/reading/klondike) Klondike
      - Phrasebook: https://code.kx.com/phrases/
      - [L](./docs/learn/reading/scrabble.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/learn/reading/scrabble.md) [O](https://code.kx.com/q/learn/reading/scrabble) Scrabble
    - Application examples:
      - [L](./docs/wp/astronomy.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/wp/astronomy.md) [O](https://code.kx.com/q/wp/astronomy) Astronomy (WP)
      - [L](./docs/wp/blockchain/index.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/wp/blockchain/index.md) [O](https://code.kx.com/q/wp/blockchain) Bitcoin blockchains (WP)
      - [L](./docs/wp/card-counters/index.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/wp/card-counters/index.md) [O](https://code.kx.com/q/wp/card-counters) Card counters (WP)
      - [L](./docs/wp/corporate-actions.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/wp/corporate-actions.md) [O](https://code.kx.com/q/wp/corporate-actions) Corporate actions (WP)
      - [L](./docs/wp/disaster-management/index.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/wp/disaster-management/index.md) [O](https://code.kx.com/q/wp/disaster-management) Disaster management (WP)
      - [L](./docs/wp/exoplanets/index.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/wp/exoplanets/index.md) [O](https://code.kx.com/q/wp/exoplanets) Exoplanets (WP)
      - [L](./docs/wp/market-depth/index.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/wp/market-depth/index.md) [O](https://code.kx.com/q/wp/market-depth) Market depth (WP)
      - [L](./docs/wp/market-fragmentation/index.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/wp/market-fragmentation/index.md) [O](https://code.kx.com/q/wp/market-fragmentation) Market fragmentation (WP)
      - [L](./docs/wp/option-pricing/index.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/wp/option-pricing/index.md) [O](https://code.kx.com/q/wp/option-pricing) Option pricing (WP)
      - [L](./docs/wp/disaster-floods/index.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/wp/disaster-floods/index.md) [O](https://code.kx.com/q/wp/disaster-floods) Predicting floods (WP)
      - [L](./docs/wp/signal-processing/index.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/wp/signal-processing/index.md) [O](https://code.kx.com/q/wp/signal-processing) Signal processing (WP)
      - [L](./docs/wp/space-weather/index.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/wp/space-weather/index.md) [O](https://code.kx.com/q/wp/space-weather) Space weather (WP)
      - [L](./docs/wp/surveillance/index.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/wp/surveillance/index.md) [O](https://code.kx.com/q/wp/surveillance) Trading surveillance (WP)
      - [L](./docs/wp/transaction-cost.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/wp/transaction-cost.md) [O](https://code.kx.com/q/wp/transaction-cost) Transaction-cost analysis (WP)
      - [L](./docs/wp/trend-indicators/index.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/wp/trend-indicators/index.md) [O](https://code.kx.com/q/wp/trend-indicators) 😀Trend indicators (WP)
    - Advanced q:
      - Remarks on Style: https://github.com/qbists/style
      - [L](./docs/learn/shifts-scans.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/learn/shifts-scans.md) [O](https://code.kx.com/q/learn/shifts-scans) Shifts & scans
      - [L](./docs/learn/blogs.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/learn/blogs.md) [O](https://code.kx.com/q/learn/blogs) Technical articles
      - [L](./docs/learn/views.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/learn/views.md) [O](https://code.kx.com/q/learn/views) Views
      - [L](./docs/learn/archive.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/learn/archive.md) [O](https://code.kx.com/q/learn/archive) Origins
      - [L](./docs/about/terminology.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/about/terminology.md) [O](https://code.kx.com/q/about/terminology) Terminology
    - Starting kdb+:
      - [L](./docs/learn/startingkdb/index.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/learn/startingkdb/index.md) [O](https://code.kx.com/q/learn/startingkdb) Overview
      - [L](./docs/learn/startingkdb/language.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/learn/startingkdb/language.md) [O](https://code.kx.com/q/learn/startingkdb/language) The q language
      - [L](./docs/learn/startingkdb/ipc.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/learn/startingkdb/ipc.md) [O](https://code.kx.com/q/learn/startingkdb/ipc) IPC
      - [L](./docs/learn/startingkdb/tables.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/learn/startingkdb/tables.md) [O](https://code.kx.com/q/learn/startingkdb/tables) Tables
      - [L](./docs/learn/startingkdb/hdb.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/learn/startingkdb/hdb.md) [O](https://code.kx.com/q/learn/startingkdb/hdb) Historical database
      - [L](./docs/learn/startingkdb/tick.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/learn/startingkdb/tick.md) [O](https://code.kx.com/q/learn/startingkdb/tick) Realtime database
  - # kdb+ and q: 
    - [L](./docs/index.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/index.md) [O](https://code.kx.com/q) About
    - [L](./docs/ref/index.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/ref/index.md) [O](https://code.kx.com/q/ref) Reference card
    - [L](./docs/devtools.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/devtools.md) [O](https://code.kx.com/q/devtools) Developer tools
    - Interfaces: 
      - [L](./docs/interfaces/index.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/interfaces/index.md) [O](https://code.kx.com/q/interfaces) KX libraries
      - [L](./docs/interfaces/q-client-for-bloomberg.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/interfaces/q-client-for-bloomberg.md) [O](https://code.kx.com/q/interfaces/q-client-for-bloomberg) Bloomberg
      - C/C++:
        - [L](./docs/interfaces/c-client-for-q.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/interfaces/c-client-for-q.md) [O](https://code.kx.com/q/interfaces/c-client-for-q) Quick guide
        - [L](./docs/interfaces/capiref.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/interfaces/capiref.md) [O](https://code.kx.com/q/interfaces/capiref) API reference
        - [L](./docs/wp/capi/index.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/wp/capi/index.md) [O](https://code.kx.com/q/wp/capi) C API for kdb+ (WP)
        - [L](./docs/interfaces/using-c-functions.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/interfaces/using-c-functions.md) [O](https://code.kx.com/q/interfaces/using-c-functions) Using C/C++ functions
      - [L](./docs/interfaces/excel-client-for-q.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/interfaces/excel-client-for-q.md) [O](https://code.kx.com/q/interfaces/excel-client-for-q) Excel
      - [L](./docs/wp/fix-messaging.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/wp/fix-messaging.md) [O](https://code.kx.com/q/wp/fix-messaging) FIX messaging (WP)
      - [L](./docs/interfaces/gpus.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/interfaces/gpus.md) [O](https://code.kx.com/q/interfaces/gpus) GPUs
      - [L](./docs/wp/lightning-tickerplants/index.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/wp/lightning-tickerplants/index.md) [O](https://code.kx.com/q/wp/lightning-tickerplants) Lightning tickerplants (WP)
      - [L](./docs/interfaces/matlab-client-for-q.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/interfaces/matlab-client-for-q.md) [O](https://code.kx.com/q/interfaces/matlab-client-for-q) Matlab
      - [L](./docs/interfaces/q-server-for-odbc3.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/interfaces/q-server-for-odbc3.md) [O](https://code.kx.com/q/interfaces/q-server-for-odbc3) ODBC3
      - [L](./docs/interfaces/odbc-simba.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/interfaces/odbc-simba.md) [O](https://code.kx.com/q/interfaces/odbc-simba) ODBC/Simba
      - [L](./docs/interfaces/r.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/interfaces/r.md) [O](https://code.kx.com/q/interfaces/r) R
      - [L](./docs/interfaces/scala-client-for-q.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/interfaces/scala-client-for-q.md) [O](https://code.kx.com/q/interfaces/scala-client-for-q) Scala
    - [L](./docs/github.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/github.md) [O](https://code.kx.com/q/github) Open source
    - [L](./docs/ml.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/ml.md) [O](https://code.kx.com/q/ml) Machine learning
    - Cloud: https://code.kx.com/insights/core/
    - Community: https://code.kx.com/home/community/
    - kdb+ and q forum: https://community.kx.com/t5/kdb-and-q/bd-p/kdb-q-questions
    - [L](./docs/wp/index.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/wp/index.md) [O](https://code.kx.com/q/wp) White papers
    - [L](./docs/about/thissite.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/about/thissite.md) [O](https://code.kx.com/q/about/thissite) About this site
  - # Architecture:
    - [L](./docs/architecture/index.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/architecture/index.md) [O](https://code.kx.com/q/architecture) About
    - [L](./docs/architecture/examples.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/architecture/examples.md) [O](https://code.kx.com/q/architecture/examples) Examples
    - [L](./docs/kb/alternative-in-memory-layouts.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/kb/alternative-in-memory-layouts.md) [O](https://code.kx.com/q/kb/alternative-in-memory-layouts) Alternative in-memory layouts
    - [L](./docs/kb/chained-tickerplant.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/kb/chained-tickerplant.md) [O](https://code.kx.com/q/kb/chained-tickerplant) Chained tickerplant
    - [L](./docs/kb/client-server.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/kb/client-server.md) [O](https://code.kx.com/q/kb/client-server) Client-server
    - [L](./docs/kb/corporate-actions.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/kb/corporate-actions.md) [O](https://code.kx.com/q/kb/corporate-actions) Corporate actions
    - [L](./docs/wp/data-recovery.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/wp/data-recovery.md) [O](https://code.kx.com/q/wp/data-recovery) Data recovery for kdb+tick (WP)
    - [L](./docs/wp/disaster-recovery/index.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/wp/disaster-recovery/index.md) [O](https://code.kx.com/q/wp/disaster-recovery) Disaster recovery (WP)
    - [L](./docs/wp/gateway-design/index.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/wp/gateway-design/index.md) [O](https://code.kx.com/q/wp/gateway-design) Gateway design (WP)
    - [L](./docs/kb/kdb-tick.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/kb/kdb-tick.md) [O](https://code.kx.com/q/kb/kdb-tick) Kdb+tick configuration
    - [L](./docs/wp/tick-profiling.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/wp/tick-profiling.md) [O](https://code.kx.com/q/wp/tick-profiling) Kdb+tick profiling (WP)
    - Kubernetes: 'https://youtu.be/jqtkkCqBvr4'
    - [L](./docs/kb/load-balancing.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/kb/load-balancing.md) [O](https://code.kx.com/q/kb/load-balancing) Load balancing
    - [L](./docs/basics/memory-backed.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/basics/memory-backed.md) [O](https://code.kx.com/q/basics/memory-backed) Memory backed by files
    - Optane Memory:
      - [L](./docs/kb/optane.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/kb/optane.md) [O](https://code.kx.com/q/kb/optane) Optane Memory and kdb+
      - [L](./docs/architecture/optane-tests.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/architecture/optane-tests.md) [O](https://code.kx.com/q/architecture/optane-tests) Performance tests
    - [L](./docs/wp/order-book.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/wp/order-book.md) [O](https://code.kx.com/q/wp/order-book) Order Book (WP)
    - [L](./docs/kb/publish-subscribe.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/kb/publish-subscribe.md) [O](https://code.kx.com/q/kb/publish-subscribe) Publish and subscribe
    - [L](./docs/wp/solace/index.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/wp/solace/index.md) [O](https://code.kx.com/q/wp/solace) Pub/sub with Solace (WP)
    - [L](./docs/wp/query-routing/index.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/wp/query-routing/index.md) [O](https://code.kx.com/q/wp/query-routing) Query Routing (WP)
    - [L](./docs/wp/rt-tick/index.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/wp/rt-tick/index.md) [O](https://code.kx.com/q/wp/rt-tick) Real-time tick subscribers (WP)
    - [L](./docs/wp/websockets/index.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/wp/websockets/index.md) [O](https://code.kx.com/q/wp/websockets) WebSockets (WP)
    - [L](./docs/kb/w-q.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/kb/w-q.md) [O](https://code.kx.com/q/kb/w-q) Write-only RDB
    - Advanced:
      - [L](./docs/wp/query-interface.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/wp/query-interface.md) [O](https://code.kx.com/q/wp/query-interface) Distributed systems (WP)
      - [L](./docs/wp/intraday-writedown/index.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/wp/intraday-writedown/index.md) [O](https://code.kx.com/q/wp/intraday-writedown) Intraday writedown (WP)
  - # Database:
    - [L](./docs/database/index.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/database/index.md) [O](https://code.kx.com/q/database) Tables in the filesystem
    - Populating tables:
      - [L](./docs/kb/loading-from-large-files.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/kb/loading-from-large-files.md) [O](https://code.kx.com/q/kb/loading-from-large-files) Loading from large files
      - [L](./docs/wp/foreign-keys.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/wp/foreign-keys.md) [O](https://code.kx.com/q/wp/foreign-keys) Foreign keys (WP)
      - [L](./docs/kb/linking-columns.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/kb/linking-columns.md) [O](https://code.kx.com/q/kb/linking-columns) Linking columns
      - [L](./docs/wp/data-loaders/index.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/wp/data-loaders/index.md) [O](https://code.kx.com/q/wp/data-loaders) Data loaders (WP)
      - [L](./docs/database/mdb-odbc.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/database/mdb-odbc.md) [O](https://code.kx.com/q/database/mdb-odbc) From MDB via ODBC
    - Persisting tables:
      - [L](./docs/database/object.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/database/object.md) [O](https://code.kx.com/q/database/object) Serializing an object
      - [L](./docs/kb/splayed-tables.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/kb/splayed-tables.md) [O](https://code.kx.com/q/kb/splayed-tables) Splayed tables
      - [L](./docs/kb/partition.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/kb/partition.md) [O](https://code.kx.com/q/kb/partition) Partitioned tables
      - [L](./docs/database/segment.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/database/segment.md) [O](https://code.kx.com/q/database/segment) Segmented databases
      - [L](./docs/wp/multi-partitioned-dbs/index.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/wp/multi-partitioned-dbs/index.md) [O](https://code.kx.com/q/wp/multi-partitioned-dbs) Multiple partitions (WP)
    - Maintenance:
      - [L](./docs/wp/data-management.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/wp/data-management.md) [O](https://code.kx.com/q/wp/data-management) Data management (WP)
      - [L](./docs/kb/dare.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/kb/dare.md) [O](https://code.kx.com/q/kb/dare) Data-At-Rest Encryption
      - [L](./docs/kb/file-compression.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/kb/file-compression.md) [O](https://code.kx.com/q/kb/file-compression) File compression
      - [L](./docs/wp/compress/index.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/wp/compress/index.md) [O](https://code.kx.com/q/wp/compress) Compression (WP)
      - [L](./docs/wp/permissions/index.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/wp/permissions/index.md) [O](https://code.kx.com/q/wp/permissions) Permissions (WP)
      - [L](./docs/wp/columnar-database/index.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/wp/columnar-database/index.md) [O](https://code.kx.com/q/wp/columnar-database) Query optimization (WP)
      - [L](./docs/wp/query-scaling.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/wp/query-scaling.md) [O](https://code.kx.com/q/wp/query-scaling) Query scaling (WP)
      - [L](./docs/wp/ts-shrink/index.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/wp/ts-shrink/index.md) [O](https://code.kx.com/q/wp/ts-shrink) Time-series simplification (WP)
      - [L](./docs/kb/compacting-hdb-sym.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/kb/compacting-hdb-sym.md) [O](https://code.kx.com/q/kb/compacting-hdb-sym) Compacting HDB sym
      - [L](./docs/wp/symfiles.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/wp/symfiles.md) [O](https://code.kx.com/q/wp/symfiles) Working with sym files (WP)
  - # Developing:
    - IPC:
      - [L](./docs/basics/ipc.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/basics/ipc.md) [O](https://code.kx.com/q/basics/ipc) Overview
      - [L](./docs/kb/callbacks.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/kb/callbacks.md) [O](https://code.kx.com/q/kb/callbacks) Callbacks
      - [L](./docs/basics/listening-port.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/basics/listening-port.md) [O](https://code.kx.com/q/basics/listening-port) Listening port
      - [L](./docs/kb/named-pipes.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/kb/named-pipes.md) [O](https://code.kx.com/q/kb/named-pipes) Named pipes
      - [L](./docs/kb/serialization.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/kb/serialization.md) [O](https://code.kx.com/q/kb/serialization) Serialization examples
      - [L](./docs/kb/server-calling-client.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/kb/server-calling-client.md) [O](https://code.kx.com/q/kb/server-calling-client) Server calling client
      - [L](./docs/wp/socket-sharding/index.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/wp/socket-sharding/index.md) [O](https://code.kx.com/q/wp/socket-sharding) Socket sharding (WP)
      - [L](./docs/kb/ssl.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/kb/ssl.md) [O](https://code.kx.com/q/kb/ssl) SSL/TLS
      - [L](./docs/kb/websockets.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/kb/websockets.md) [O](https://code.kx.com/q/kb/websockets) WebSockets
      - [L](./docs/wp/ipc/index.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/wp/ipc/index.md) [O](https://code.kx.com/q/wp/ipc) Interprocess communication (WP)
    - Tools:
      - [L](./docs/kb/profiler.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/kb/profiler.md) [O](https://code.kx.com/q/kb/profiler) Code profiler
      - [L](./docs/basics/debug.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/basics/debug.md) [O](https://code.kx.com/q/basics/debug) Debugging
      - [L](./docs/basics/errors.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/basics/errors.md) [O](https://code.kx.com/q/basics/errors) Errors
      - [L](./docs/about/man.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/about/man.md) [O](https://code.kx.com/q/about/man) man.q
      - [L](./docs/basics/syscmds.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/basics/syscmds.md) [O](https://code.kx.com/q/basics/syscmds) System commands
      - [L](./docs/kb/unit-tests.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/kb/unit-tests.md) [O](https://code.kx.com/q/kb/unit-tests) Unit tests
      - [L](./docs/kb/using-dotz.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/kb/using-dotz.md) [O](https://code.kx.com/q/kb/using-dotz) Using .z
    - Coding:
      - [L](./docs/wp/data-visualization/index.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/wp/data-visualization/index.md) [O](https://code.kx.com/q/wp/data-visualization) Data visualization (WP)
      - [L](./docs/kb/deferred-response.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/kb/deferred-response.md) [O](https://code.kx.com/q/kb/deferred-response) Deferred response
      - [L](./docs/kb/geospatial.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/kb/geospatial.md) [O](https://code.kx.com/q/kb/geospatial) Geospatial indexing
      - [L](./docs/kb/lp.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/kb/lp.md) [O](https://code.kx.com/q/kb/lp) Linear programming
      - [L](./docs/kb/multithreaded-input.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/kb/multithreaded-input.md) [O](https://code.kx.com/q/kb/multithreaded-input) Multithreaded input
      - [L](./docs/kb/mt-primitives.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/kb/mt-primitives.md) [O](https://code.kx.com/q/kb/mt-primitives) Multithreaded primitives
      - [L](./docs/kb/pivoting-tables.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/kb/pivoting-tables.md) [O](https://code.kx.com/q/kb/pivoting-tables) Pivoting tables
      - [L](./docs/basics/precision.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/basics/precision.md) [O](https://code.kx.com/q/basics/precision) Precision
      - [L](./docs/kb/programming-examples.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/kb/programming-examples.md) [O](https://code.kx.com/q/kb/programming-examples) Programming examples
      - [L](./docs/kb/programming-idioms.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/kb/programming-idioms.md) [O](https://code.kx.com/q/kb/programming-idioms) Programming idioms
      - [L](./docs/kb/temporal-data.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/kb/temporal-data.md) [O](https://code.kx.com/q/kb/temporal-data) Temporal data
      - [L](./docs/kb/timezones.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/kb/timezones.md) [O](https://code.kx.com/q/kb/timezones) Timezones
      - [L](./docs/kb/unicode.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/kb/unicode.md) [O](https://code.kx.com/q/kb/unicode) Unicode
    - DevOps:
      - [L](./docs/kb/authentication.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/kb/authentication.md) [O](https://code.kx.com/q/kb/authentication) Authentication and access
      - [L](./docs/basics/cmdline.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/basics/cmdline.md) [O](https://code.kx.com/q/basics/cmdline) Command-line options
      - [L](./docs/kb/cpu-affinity.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/kb/cpu-affinity.md) [O](https://code.kx.com/q/kb/cpu-affinity) CPU affinity
      - [L](./docs/kb/custom-web.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/kb/custom-web.md) [O](https://code.kx.com/q/kb/custom-web) Custom web server
      - [L](./docs/kb/daemon.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/kb/daemon.md) [O](https://code.kx.com/q/kb/daemon) Daemon
      - [L](./docs/kb/firewalling.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/kb/firewalling.md) [O](https://code.kx.com/q/kb/firewalling) Firewalling
      - [L](./docs/kb/inetd.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/kb/inetd.md) [O](https://code.kx.com/q/kb/inetd) inetd, xinetd
      - [L](./docs/kb/linux-production.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/kb/linux-production.md) [O](https://code.kx.com/q/kb/linux-production) Linux production notes
      - [L](./docs/kb/logging.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/kb/logging.md) [O](https://code.kx.com/q/kb/logging) Logging
      - [L](./docs/wp/multi-thread/index.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/wp/multi-thread/index.md) [O](https://code.kx.com/q/wp/multi-thread) Multi-threading (WP)
      - [L](./docs/kb/versions.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/kb/versions.md) [O](https://code.kx.com/q/kb/versions) Multiple versions
      - [L](./docs/basics/peach.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/basics/peach.md) [O](https://code.kx.com/q/basics/peach) Parallel processing
      - [L](./docs/kb/performance-tips.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/kb/performance-tips.md) [O](https://code.kx.com/q/kb/performance-tips) Performance tips
      - [L](./docs/kb/replay-log.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/kb/replay-log.md) [O](https://code.kx.com/q/kb/replay-log) Replay logfile
      - [L](./docs/develop/shebang.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/develop/shebang.md) [O](https://code.kx.com/q/develop/shebang) Shebang script
      - [L](./docs/wp/surveillance-latency/index.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/wp/surveillance-latency/index.md) [O](https://code.kx.com/q/wp/surveillance-latency) Surveillance latency (WP)
      - [L](./docs/kb/windows-service/index.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/kb/windows-service/index.md) [O](https://code.kx.com/q/kb/windows-service) Windows service
    - Release notes:
      - [L](./docs/releases/index.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/releases/index.md) [O](https://code.kx.com/q/releases) History
      - [L](./docs/releases/ChangesIn4.0.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/releases/ChangesIn4.0.md) [O](https://code.kx.com/q/releases/ChangesIn4.0) Changes in 4.0
      - [L](./docs/releases/ChangesIn3.6.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/releases/ChangesIn3.6.md) [O](https://code.kx.com/q/releases/ChangesIn3.6) Changes in 3.6
      - [L](./docs/releases/ChangesIn3.5.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/releases/ChangesIn3.5.md) [O](https://code.kx.com/q/releases/ChangesIn3.5) Changes in 3.5
      - [L](./docs/releases/ChangesIn3.4.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/releases/ChangesIn3.4.md) [O](https://code.kx.com/q/releases/ChangesIn3.4) Changes in 3.4
      - [L](./docs/releases/ChangesIn3.3.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/releases/ChangesIn3.3.md) [O](https://code.kx.com/q/releases/ChangesIn3.3) Changes in 3.3
      - [L](./docs/releases/ChangesIn3.2.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/releases/ChangesIn3.2.md) [O](https://code.kx.com/q/releases/ChangesIn3.2) Changes in 3.2
      - [L](./docs/releases/ChangesIn3.1.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/releases/ChangesIn3.1.md) [O](https://code.kx.com/q/releases/ChangesIn3.1) Changes in 3.1
      - [L](./docs/releases/ChangesIn3.0.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/releases/ChangesIn3.0.md) [O](https://code.kx.com/q/releases/ChangesIn3.0) Changes in 3.0
      - [L](./docs/releases/ChangesIn2.8.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/releases/ChangesIn2.8.md) [O](https://code.kx.com/q/releases/ChangesIn2.8) Changes in 2.8
      - [L](./docs/releases/ChangesIn2.7.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/releases/ChangesIn2.7.md) [O](https://code.kx.com/q/releases/ChangesIn2.7) Changes in 2.7
      - [L](./docs/releases/ChangesIn2.6.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/releases/ChangesIn2.6.md) [O](https://code.kx.com/q/releases/ChangesIn2.6) Changes in 2.6
      - [L](./docs/releases/ChangesIn2.5.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/releases/ChangesIn2.5.md) [O](https://code.kx.com/q/releases/ChangesIn2.5) Changes in 2.5
      - [L](./docs/releases/ChangesIn2.4.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/releases/ChangesIn2.4.md) [O](https://code.kx.com/q/releases/ChangesIn2.4) Changes in 2.4
      - [L](./docs/releases/withdrawn.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/releases/withdrawn.md) [O](https://code.kx.com/q/releases/withdrawn) Withdrawn
    - [L](./docs/kb/faq-listbox.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/kb/faq-listbox.md) [O](https://code.kx.com/q/kb/faq-listbox) FAQ
  - # Language: 
    - [L](./docs/ref/index.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/ref/index.md) [O](https://code.kx.com/q/ref) Reference card
    - [L](./docs/basics/by-topic.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/basics/by-topic.md) [O](https://code.kx.com/q/basics/by-topic) By topic
    - Iteration:
      - [L](./docs/basics/iteration.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/basics/iteration.md) [O](https://code.kx.com/q/basics/iteration) Overview
      - [L](./docs/basics/implicit-iteration.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/basics/implicit-iteration.md) [O](https://code.kx.com/q/basics/implicit-iteration) Implicit iteration
      - [L](./docs/ref/iterators.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/ref/iterators.md) [O](https://code.kx.com/q/ref/iterators) Iterators
      - [L](./docs/ref/maps.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/ref/maps.md) [O](https://code.kx.com/q/ref/maps) Maps
      - [L](./docs/ref/accumulators.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/ref/accumulators.md) [O](https://code.kx.com/q/ref/accumulators) Accumulators
      - [L](./docs/wp/iterators/index.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/wp/iterators/index.md) [O](https://code.kx.com/q/wp/iterators) Guide to iterators (WP)
    - Keywords:
      - [L](./docs/ref/abs.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/ref/abs.md) [O](https://code.kx.com/q/ref/abs) abs
      - [L](./docs/ref/aj.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/ref/aj.md) [O](https://code.kx.com/q/ref/aj) aj, aj0, ajf, ajf0
      - [L](./docs/ref/all-any.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/ref/all-any.md) [O](https://code.kx.com/q/ref/all-any) all, any
      - [L](./docs/ref/and.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/ref/and.md) [O](https://code.kx.com/q/ref/and) and
      - [L](./docs/ref/asc.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/ref/asc.md) [O](https://code.kx.com/q/ref/asc) asc, iasc, xasc
      - [L](./docs/ref/asof.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/ref/asof.md) [O](https://code.kx.com/q/ref/asof) asof
      - [L](./docs/ref/attr.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/ref/attr.md) [O](https://code.kx.com/q/ref/attr) attr
      - [L](./docs/ref/avg.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/ref/avg.md) [O](https://code.kx.com/q/ref/avg) avg, avgs, mavg, wavg
      - [L](./docs/ref/bin.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/ref/bin.md) [O](https://code.kx.com/q/ref/bin) bin, binr
      - [L](./docs/ref/ceiling.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/ref/ceiling.md) [O](https://code.kx.com/q/ref/ceiling) ceiling
      - [L](./docs/ref/count.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/ref/count.md) [O](https://code.kx.com/q/ref/count) count, mcount
      - [L](./docs/ref/cols.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/ref/cols.md) [O](https://code.kx.com/q/ref/cols) cols, xcol, xcols
      - [L](./docs/ref/cor.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/ref/cor.md) [O](https://code.kx.com/q/ref/cor) cor
      - [L](./docs/ref/cos.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/ref/cos.md) [O](https://code.kx.com/q/ref/cos) cos, acos
      - [L](./docs/ref/cov.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/ref/cov.md) [O](https://code.kx.com/q/ref/cov) cov, scov
      - [L](./docs/ref/cross.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/ref/cross.md) [O](https://code.kx.com/q/ref/cross) cross
      - [L](./docs/ref/csv.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/ref/csv.md) [O](https://code.kx.com/q/ref/csv) csv
      - [L](./docs/ref/cut.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/ref/cut.md) [O](https://code.kx.com/q/ref/cut) cut
      - [L](./docs/ref/delete.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/ref/delete.md) [O](https://code.kx.com/q/ref/delete) delete
      - [L](./docs/ref/deltas.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/ref/deltas.md) [O](https://code.kx.com/q/ref/deltas) deltas
      - [L](./docs/ref/desc.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/ref/desc.md) [O](https://code.kx.com/q/ref/desc) desc, idesc, xdesc
      - [L](./docs/ref/dev.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/ref/dev.md) [O](https://code.kx.com/q/ref/dev) dev, mdev, sdev
      - [L](./docs/ref/differ.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/ref/differ.md) [O](https://code.kx.com/q/ref/differ) differ
      - [L](./docs/ref/distinct.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/ref/distinct.md) [O](https://code.kx.com/q/ref/distinct) distinct
      - [L](./docs/ref/div.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/ref/div.md) [O](https://code.kx.com/q/ref/div) div
      - [L](./docs/ref/dsave.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/ref/dsave.md) [O](https://code.kx.com/q/ref/dsave) dsave
      - [L](./docs/ref/each.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/ref/each.md) [O](https://code.kx.com/q/ref/each) each, peach
      - [L](./docs/ref/ej.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/ref/ej.md) [O](https://code.kx.com/q/ref/ej) ej
      - [L](./docs/ref/ema.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/ref/ema.md) [O](https://code.kx.com/q/ref/ema) ema
      - [L](./docs/ref/enlist.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/ref/enlist.md) [O](https://code.kx.com/q/ref/enlist) enlist
      - [L](./docs/ref/eval.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/ref/eval.md) [O](https://code.kx.com/q/ref/eval) eval, reval
      - [L](./docs/ref/except.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/ref/except.md) [O](https://code.kx.com/q/ref/except) except
      - [L](./docs/ref/exec.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/ref/exec.md) [O](https://code.kx.com/q/ref/exec) exec
      - [L](./docs/ref/exit.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/ref/exit.md) [O](https://code.kx.com/q/ref/exit) exit
      - [L](./docs/ref/exp.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/ref/exp.md) [O](https://code.kx.com/q/ref/exp) exp, xexp
      - [L](./docs/ref/fby.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/ref/fby.md) [O](https://code.kx.com/q/ref/fby) fby
      - [L](./docs/ref/fill.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/ref/fill.md) [O](https://code.kx.com/q/ref/fill) fills
      - [L](./docs/ref/first.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/ref/first.md) [O](https://code.kx.com/q/ref/first) first, last
      - [L](./docs/ref/fkeys.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/ref/fkeys.md) [O](https://code.kx.com/q/ref/fkeys) fkeys
      - [L](./docs/ref/flip.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/ref/flip.md) [O](https://code.kx.com/q/ref/flip) flip
      - [L](./docs/ref/floor.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/ref/floor.md) [O](https://code.kx.com/q/ref/floor) floor
      - [L](./docs/ref/get.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/ref/get.md) [O](https://code.kx.com/q/ref/get) get, set
      - [L](./docs/ref/getenv.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/ref/getenv.md) [O](https://code.kx.com/q/ref/getenv) getenv, setenv
      - [L](./docs/ref/group.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/ref/group.md) [O](https://code.kx.com/q/ref/group) group
      - [L](./docs/ref/gtime.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/ref/gtime.md) [O](https://code.kx.com/q/ref/gtime) gtime, ltime
      - [L](./docs/ref/hcount.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/ref/hcount.md) [O](https://code.kx.com/q/ref/hcount) hcount
      - [L](./docs/ref/hdel.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/ref/hdel.md) [O](https://code.kx.com/q/ref/hdel) hdel
      - [L](./docs/ref/hopen.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/ref/hopen.md) [O](https://code.kx.com/q/ref/hopen) hopen, hclose
      - [L](./docs/ref/hsym.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/ref/hsym.md) [O](https://code.kx.com/q/ref/hsym) hsym
      - [L](./docs/ref/ij.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/ref/ij.md) [O](https://code.kx.com/q/ref/ij) ij, ijf
      - [L](./docs/ref/in.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/ref/in.md) [O](https://code.kx.com/q/ref/in) in
      - [L](./docs/ref/insert.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/ref/insert.md) [O](https://code.kx.com/q/ref/insert) insert
      - [L](./docs/ref/inter.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/ref/inter.md) [O](https://code.kx.com/q/ref/inter) inter
      - [L](./docs/ref/inv.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/ref/inv.md) [O](https://code.kx.com/q/ref/inv) inv
      - [L](./docs/ref/key.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/ref/key.md) [O](https://code.kx.com/q/ref/key) key
      - [L](./docs/ref/keys.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/ref/keys.md) [O](https://code.kx.com/q/ref/keys) keys, xkey
      - [L](./docs/ref/like.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/ref/like.md) [O](https://code.kx.com/q/ref/like) like
      - [L](./docs/ref/lj.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/ref/lj.md) [O](https://code.kx.com/q/ref/lj) lj, ljf
      - [L](./docs/ref/load.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/ref/load.md) [O](https://code.kx.com/q/ref/load) load, rload
      - [L](./docs/ref/log.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/ref/log.md) [O](https://code.kx.com/q/ref/log) log, xlog
      - [L](./docs/ref/lower.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/ref/lower.md) [O](https://code.kx.com/q/ref/lower) lower
      - [L](./docs/ref/lsq.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/ref/lsq.md) [O](https://code.kx.com/q/ref/lsq) lsq
      - [L](./docs/ref/max.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/ref/max.md) [O](https://code.kx.com/q/ref/max) max, maxs, mmax
      - [L](./docs/ref/md5.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/ref/md5.md) [O](https://code.kx.com/q/ref/md5) md5
      - [L](./docs/ref/med.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/ref/med.md) [O](https://code.kx.com/q/ref/med) med
      - [L](./docs/ref/meta.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/ref/meta.md) [O](https://code.kx.com/q/ref/meta) meta
      - [L](./docs/ref/min.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/ref/min.md) [O](https://code.kx.com/q/ref/min) min, mins, mmin
      - [L](./docs/ref/mmu.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/ref/mmu.md) [O](https://code.kx.com/q/ref/mmu) mmu
      - [L](./docs/ref/mod.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/ref/mod.md) [O](https://code.kx.com/q/ref/mod) mod
      - [L](./docs/ref/neg.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/ref/neg.md) [O](https://code.kx.com/q/ref/neg) neg
      - [L](./docs/ref/next.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/ref/next.md) [O](https://code.kx.com/q/ref/next) next, prev, xprev
      - [L](./docs/ref/not.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/ref/not.md) [O](https://code.kx.com/q/ref/not) not
      - [L](./docs/ref/null.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/ref/null.md) [O](https://code.kx.com/q/ref/null) 'null'
      - [L](./docs/ref/or.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/ref/or.md) [O](https://code.kx.com/q/ref/or) or
      - [L](./docs/ref/over.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/ref/over.md) [O](https://code.kx.com/q/ref/over) over, scan
      - [L](./docs/ref/parse.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/ref/parse.md) [O](https://code.kx.com/q/ref/parse) parse
      - [L](./docs/ref/pj.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/ref/pj.md) [O](https://code.kx.com/q/ref/pj) pj
      - [L](./docs/ref/prd.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/ref/prd.md) [O](https://code.kx.com/q/ref/prd) prd, prds
      - [L](./docs/ref/prior.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/ref/prior.md) [O](https://code.kx.com/q/ref/prior) prior
      - [L](./docs/ref/rand.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/ref/rand.md) [O](https://code.kx.com/q/ref/rand) rand
      - [L](./docs/ref/rank.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/ref/rank.md) [O](https://code.kx.com/q/ref/rank) rank
      - [L](./docs/ref/ratios.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/ref/ratios.md) [O](https://code.kx.com/q/ref/ratios) ratios
      - [L](./docs/ref/raze.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/ref/raze.md) [O](https://code.kx.com/q/ref/raze) raze
      - [L](./docs/ref/read0.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/ref/read0.md) [O](https://code.kx.com/q/ref/read0) read0
      - [L](./docs/ref/read1.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/ref/read1.md) [O](https://code.kx.com/q/ref/read1) read1
      - [L](./docs/ref/reciprocal.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/ref/reciprocal.md) [O](https://code.kx.com/q/ref/reciprocal) reciprocal
      - [L](./docs/ref/reverse.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/ref/reverse.md) [O](https://code.kx.com/q/ref/reverse) reverse
      - [L](./docs/ref/rotate.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/ref/rotate.md) [O](https://code.kx.com/q/ref/rotate) rotate
      - [L](./docs/ref/save.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/ref/save.md) [O](https://code.kx.com/q/ref/save) save, rsave
      - [L](./docs/ref/select.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/ref/select.md) [O](https://code.kx.com/q/ref/select) select
      - [L](./docs/ref/show.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/ref/show.md) [O](https://code.kx.com/q/ref/show) show
      - [L](./docs/ref/signum.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/ref/signum.md) [O](https://code.kx.com/q/ref/signum) signum
      - [L](./docs/ref/sin.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/ref/sin.md) [O](https://code.kx.com/q/ref/sin) sin, asin
      - [L](./docs/ref/sqrt.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/ref/sqrt.md) [O](https://code.kx.com/q/ref/sqrt) sqrt
      - [L](./docs/ref/ss.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/ref/ss.md) [O](https://code.kx.com/q/ref/ss) ss, ssr
      - [L](./docs/ref/string.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/ref/string.md) [O](https://code.kx.com/q/ref/string) string
      - [L](./docs/ref/sublist.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/ref/sublist.md) [O](https://code.kx.com/q/ref/sublist) sublist
      - [L](./docs/ref/sum.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/ref/sum.md) [O](https://code.kx.com/q/ref/sum) sum, sums, msum, wsum
      - [L](./docs/ref/sv.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/ref/sv.md) [O](https://code.kx.com/q/ref/sv) sv
      - [L](./docs/ref/system.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/ref/system.md) [O](https://code.kx.com/q/ref/system) system
      - [L](./docs/ref/tables.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/ref/tables.md) [O](https://code.kx.com/q/ref/tables) tables
      - [L](./docs/ref/tan.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/ref/tan.md) [O](https://code.kx.com/q/ref/tan) tan, atan
      - [L](./docs/ref/til.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/ref/til.md) [O](https://code.kx.com/q/ref/til) til
      - [L](./docs/ref/trim.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/ref/trim.md) [O](https://code.kx.com/q/ref/trim) trim, ltrim, rtrim
      - [L](./docs/ref/type.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/ref/type.md) [O](https://code.kx.com/q/ref/type) type
      - [L](./docs/ref/uj.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/ref/uj.md) [O](https://code.kx.com/q/ref/uj) uj, ujf
      - [L](./docs/ref/union.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/ref/union.md) [O](https://code.kx.com/q/ref/union) union
      - [L](./docs/ref/ungroup.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/ref/ungroup.md) [O](https://code.kx.com/q/ref/ungroup) ungroup
      - [L](./docs/ref/update.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/ref/update.md) [O](https://code.kx.com/q/ref/update) update
      - [L](./docs/ref/upsert.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/ref/upsert.md) [O](https://code.kx.com/q/ref/upsert) upsert
      - [L](./docs/ref/value.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/ref/value.md) [O](https://code.kx.com/q/ref/value) value
      - [L](./docs/ref/var.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/ref/var.md) [O](https://code.kx.com/q/ref/var) var, svar
      - [L](./docs/ref/view.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/ref/view.md) [O](https://code.kx.com/q/ref/view) view, views
      - [L](./docs/ref/vs.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/ref/vs.md) [O](https://code.kx.com/q/ref/vs) vs
      - [L](./docs/ref/where.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/ref/where.md) [O](https://code.kx.com/q/ref/where) where
      - [L](./docs/ref/within.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/ref/within.md) [O](https://code.kx.com/q/ref/within) within
      - [L](./docs/ref/wj.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/ref/wj.md) [O](https://code.kx.com/q/ref/wj) wj, wj1
      - [L](./docs/ref/xbar.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/ref/xbar.md) [O](https://code.kx.com/q/ref/xbar) xbar
      - [L](./docs/ref/xgroup.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/ref/xgroup.md) [O](https://code.kx.com/q/ref/xgroup) xgroup
      - [L](./docs/ref/xrank.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/ref/xrank.md) [O](https://code.kx.com/q/ref/xrank) xrank
    - [L](./docs/ref/overloads.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/ref/overloads.md) [O](https://code.kx.com/q/ref/overloads) Overloaded glyphs
    - Operators:
      - [L](./docs/ref/add.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/ref/add.md) [O](https://code.kx.com/q/ref/add) Add
      - [L](./docs/ref/amend.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/ref/amend.md) [O](https://code.kx.com/q/ref/amend) Amend
      - [L](./docs/ref/apply.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/ref/apply.md) [O](https://code.kx.com/q/ref/apply) Apply, Index, Trap
      - [L](./docs/ref/assign.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/ref/assign.md) [O](https://code.kx.com/q/ref/assign) Assign
      - [L](./docs/ref/cast.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/ref/cast.md) [O](https://code.kx.com/q/ref/cast) Cast
      - [L](./docs/ref/coalesce.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/ref/coalesce.md) [O](https://code.kx.com/q/ref/coalesce) Coalesce
      - [L](./docs/ref/compose.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/ref/compose.md) [O](https://code.kx.com/q/ref/compose) Compose
      - [L](./docs/ref/cut.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/ref/cut.md) [O](https://code.kx.com/q/ref/cut) Cut
      - [L](./docs/ref/deal.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/ref/deal.md) [O](https://code.kx.com/q/ref/deal) Deal, Roll, Permute
      - [L](./docs/ref/delete.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/ref/delete.md) [O](https://code.kx.com/q/ref/delete) Delete
      - [L](./docs/ref/display.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/ref/display.md) [O](https://code.kx.com/q/ref/display) Display
      - [L](./docs/ref/dict.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/ref/dict.md) [O](https://code.kx.com/q/ref/dict) Dict
      - [L](./docs/ref/divide.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/ref/divide.md) [O](https://code.kx.com/q/ref/divide) Divide
      - [L](./docs/ref/dynamic-load.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/ref/dynamic-load.md) [O](https://code.kx.com/q/ref/dynamic-load) Dynamic Load
      - [L](./docs/ref/drop.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/ref/drop.md) [O](https://code.kx.com/q/ref/drop) Drop
      - [L](./docs/ref/enkey.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/ref/enkey.md) [O](https://code.kx.com/q/ref/enkey) Enkey, Unkey
      - [L](./docs/ref/enumerate.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/ref/enumerate.md) [O](https://code.kx.com/q/ref/enumerate) Enumerate
      - [L](./docs/ref/enumeration.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/ref/enumeration.md) [O](https://code.kx.com/q/ref/enumeration) Enumeration
      - [L](./docs/ref/enum-extend.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/ref/enum-extend.md) [O](https://code.kx.com/q/ref/enum-extend) Enum Extend
      - [L](./docs/ref/equal.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/ref/equal.md) [O](https://code.kx.com/q/ref/equal) Equal
      - [L](./docs/ref/exec.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/ref/exec.md) [O](https://code.kx.com/q/ref/exec) Exec
      - [L](./docs/ref/file-binary.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/ref/file-binary.md) [O](https://code.kx.com/q/ref/file-binary) File Binary
      - [L](./docs/ref/file-text.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/ref/file-text.md) [O](https://code.kx.com/q/ref/file-text) File Text
      - [L](./docs/ref/fill.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/ref/fill.md) [O](https://code.kx.com/q/ref/fill) Fill
      - [L](./docs/ref/find.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/ref/find.md) [O](https://code.kx.com/q/ref/find) Find
      - [L](./docs/ref/flip-splayed.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/ref/flip-splayed.md) [O](https://code.kx.com/q/ref/flip-splayed) Flip Splayed
      - [L](./docs/ref/greater.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/ref/greater.md) [O](https://code.kx.com/q/ref/greater) Greater
      - [L](./docs/ref/greater-than.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/ref/greater-than.md) [O](https://code.kx.com/q/ref/greater-than) Greater Than
      - [L](./docs/ref/identity.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/ref/identity.md) [O](https://code.kx.com/q/ref/identity) Identity, Null
      - [L](./docs/ref/join.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/ref/join.md) [O](https://code.kx.com/q/ref/join) Join
      - [L](./docs/ref/less-than.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/ref/less-than.md) [O](https://code.kx.com/q/ref/less-than) Less Than
      - [L](./docs/ref/lesser.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/ref/lesser.md) [O](https://code.kx.com/q/ref/lesser) Lesser
      - [L](./docs/ref/match.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/ref/match.md) [O](https://code.kx.com/q/ref/match) Match
      - [L](./docs/ref/mmu.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/ref/mmu.md) [O](https://code.kx.com/q/ref/mmu) Matrix Multiply
      - [L](./docs/ref/multiply.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/ref/multiply.md) [O](https://code.kx.com/q/ref/multiply) Multiply
      - [L](./docs/ref/not-equal.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/ref/not-equal.md) [O](https://code.kx.com/q/ref/not-equal) Not Equal
      - [L](./docs/ref/pad.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/ref/pad.md) [O](https://code.kx.com/q/ref/pad) Pad
      - [L](./docs/ref/select.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/ref/select.md) [O](https://code.kx.com/q/ref/select) Select
      - [L](./docs/ref/set-attribute.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/ref/set-attribute.md) [O](https://code.kx.com/q/ref/set-attribute) Set Attribute
      - [L](./docs/ref/simple-exec.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/ref/simple-exec.md) [O](https://code.kx.com/q/ref/simple-exec) Simple Exec
      - [L](./docs/ref/signal.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/ref/signal.md) [O](https://code.kx.com/q/ref/signal) Signal
      - [L](./docs/ref/subtract.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/ref/subtract.md) [O](https://code.kx.com/q/ref/subtract) Subtract
      - [L](./docs/ref/take.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/ref/take.md) [O](https://code.kx.com/q/ref/take) Take
      - [L](./docs/ref/tok.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/ref/tok.md) [O](https://code.kx.com/q/ref/tok) Tok
      - [L](./docs/ref/update.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/ref/update.md) [O](https://code.kx.com/q/ref/update) Update
      - [L](./docs/ref/vector-conditional.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/ref/vector-conditional.md) [O](https://code.kx.com/q/ref/vector-conditional) Vector Conditional
    - Control constructs:
      - [L](./docs/ref/cond.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/ref/cond.md) [O](https://code.kx.com/q/ref/cond) Cond
      - [L](./docs/ref/do.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/ref/do.md) [O](https://code.kx.com/q/ref/do) do
      - [L](./docs/ref/if.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/ref/if.md) [O](https://code.kx.com/q/ref/if) if
      - [L](./docs/ref/while.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/ref/while.md) [O](https://code.kx.com/q/ref/while) while
    - Namespaces:
      - [L](./docs/ref/doth.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/ref/doth.md) [O](https://code.kx.com/q/ref/doth) .h
      - [L](./docs/ref/dotj.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/ref/dotj.md) [O](https://code.kx.com/q/ref/dotj) .j
      - [L](./docs/ref/dotm.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/ref/dotm.md) [O](https://code.kx.com/q/ref/dotm) .m
      - [L](./docs/ref/dotq.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/ref/dotq.md) [O](https://code.kx.com/q/ref/dotq) .Q
      - [L](./docs/ref/dotz.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/ref/dotz.md) [O](https://code.kx.com/q/ref/dotz) .z
    - [L](./docs/basics/application.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/basics/application.md) [O](https://code.kx.com/q/basics/application) Application
    - [L](./docs/basics/atomic.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/basics/atomic.md) [O](https://code.kx.com/q/basics/atomic) Atomic functions
    - [L](./docs/basics/comparison.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/basics/comparison.md) [O](https://code.kx.com/q/basics/comparison) Comparison
    - [L](./docs/basics/conformable.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/basics/conformable.md) [O](https://code.kx.com/q/basics/conformable) Conformability
    - [L](./docs/basics/handles.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/basics/handles.md) [O](https://code.kx.com/q/basics/handles) Connection handles
    - [L](./docs/basics/datatypes.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/basics/datatypes.md) [O](https://code.kx.com/q/basics/datatypes) Datatypes
    - [L](./docs/basics/dictsandtables.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/basics/dictsandtables.md) [O](https://code.kx.com/q/basics/dictsandtables) Dictionaries
    - [L](./docs/basics/enumerations.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/basics/enumerations.md) [O](https://code.kx.com/q/basics/enumerations) Enumerations
    - [L](./docs/basics/control.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/basics/control.md) [O](https://code.kx.com/q/basics/control) Evaluation control
    - [L](./docs/basics/exposed-infrastructure.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/basics/exposed-infrastructure.md) [O](https://code.kx.com/q/basics/exposed-infrastructure) Exposed infrastructure
    - [L](./docs/basics/files.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/basics/files.md) [O](https://code.kx.com/q/basics/files) File system
    - [L](./docs/basics/function-notation.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/basics/function-notation.md) [O](https://code.kx.com/q/basics/function-notation) Function notation
    - [L](./docs/basics/funsql.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/basics/funsql.md) [O](https://code.kx.com/q/basics/funsql) Functional qSQL
    - [L](./docs/basics/glossary.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/basics/glossary.md) [O](https://code.kx.com/q/basics/glossary) Glossary
    - [L](./docs/basics/internal.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/basics/internal.md) [O](https://code.kx.com/q/basics/internal) Internal functions
    - [L](./docs/basics/joins.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/basics/joins.md) [O](https://code.kx.com/q/basics/joins) Joins
    - [L](./docs/basics/math.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/basics/math.md) [O](https://code.kx.com/q/basics/math) Mathematics
    - [L](./docs/basics/metadata.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/basics/metadata.md) [O](https://code.kx.com/q/basics/metadata) Metadata
    - [L](./docs/basics/namespaces.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/basics/namespaces.md) [O](https://code.kx.com/q/basics/namespaces) Namespaces
    - [L](./docs/basics/parsetrees.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/basics/parsetrees.md) [O](https://code.kx.com/q/basics/parsetrees) Parse trees
    - [L](./docs/wp/parse-trees.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/wp/parse-trees.md) [O](https://code.kx.com/q/wp/parse-trees) Parse trees, functional SQL (WP)
    - [L](./docs/basics/qsql.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/basics/qsql.md) [O](https://code.kx.com/q/basics/qsql) QSQL queries
    - [L](./docs/basics/regex.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/basics/regex.md) [O](https://code.kx.com/q/basics/regex) Regular Expressions
    - [L](./docs/basics/syntax.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/basics/syntax.md) [O](https://code.kx.com/q/basics/syntax) Syntax
    - [L](./docs/kb/faq.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/kb/faq.md) [O](https://code.kx.com/q/kb/faq) Tables
    - [L](./docs/basics/variadic.md) [R](https://github.com/codush/fork_KxSystems_docs/blob/forvenus/docs/basics/variadic.md) [O](https://code.kx.com/q/basics/variadic) Variadic syntax
  - # kdb Insights: https://code.kx.com/insights/insights
  - # kdb Insights Enterprise: https://code.kx.com/insights/platform
  - # Help: https://code.kx.com/home/support/