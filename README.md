Watcher
=======

Watcher observes and controls maintenance access on production IT assets, like databases and servers. It acts as man-in-the-middle between the maintainer and the TI asset, logging actions, filtering commands and recording outputs.

Usage scenario
--------------

Imagine troubles on a software and the developer needs production access to fix the bug. What happens if you can't trust the developer a credential to the production database server? You can give him a Watcher credential and fine grain control and monitor their queries. And if ssh access is also needed? You can use Watcher again.

*Disclaimer: Keep in mind that Watcher is in development.*
