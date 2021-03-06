Cloud Storage Server
====================

An open source, extensible, self-hosted cloud storage API.  The base server implements a complete file system similar to Amazon Cloud Drive and other providers.  Just don't expect to build a competing service with this software.

Cloud Storage Server pairs quite nicely with [Cloud Backup](http://barebonescms.com/documentation/cloud_backup/).

Features
--------

* Completely self-contained.  No need for a separate web server or enterprise database engine - just install PHP and go.
* Works well with [Service Manager](https://github.com/cubiclesoft/service-manager/).  Automatically start Cloud Storage Server when the system boots up.
* Command-line driven user management interface.  Quickly set up API keys and access levels.
* The /files API implements everything needed in a file-based cloud storage provider:  Folder hierarchy management, file upload/download, copy, move, rename, trash and restore, delete, and guest access.
* User initialization for first time use of a specific server extension.  Useful for placing a 'welcome message' and/or initial folder setup in their account.
* Extensible. Only limited by your imagination.
* [Remoted API Server](https://github.com/cubiclesoft/remoted-api-server) capable.
* Standards-based, RESTful interface.  Also supports most operations over WebSocket.
* And much, much more.  See the official documentation for a more complete feature list.
* Also has a liberal open source license.  MIT or LGPL, your choice.
* Designed for relatively painless integration into your environment.
* Sits on GitHub for all of that pull request and issue tracker goodness to easily submit changes and ideas respectively.

Nifty Extensions
----------------

* [/feeds](https://github.com/cubiclesoft/cloud-storage-server-ext-feeds) - A powerful and flexible API to send and schedule notifications with data payloads attached.  The /feeds API allows for scheduling future notifications and has powerful filtering features to only return information that a monitoring application is interested in.
* [/scripts](https://github.com/cubiclesoft/cloud-storage-server-ext-scripts) - A powerful and flexible API to initiate named, long-running scripts as other users on a system (e.g. root/SYSTEM).  The /scripts API uses a crontab-like, per-user definition file to define what scripts can be run.  Parameter and limited 'stdin' passing support.  While scripts are running, track status and/or monitor start and completion of script runs.

More Information
----------------

Documentation, examples, and official downloads of this project sit on the Barebones CMS website:

http://barebonescms.com/documentation/cloud_storage_server/

Adding Extensions
-----------------

Got an idea for an extension that you would like to see included?  Open an issue on the issue tracker.  Due to Cloud Storage Server being a server product that is intended to be network-facing, all included extensions must pass rigorous CubicleSoft standards.  Extensions must also be dual licensed under MIT/LGPL.
