Atom Dataset Producer
=====================

[![Build Status](https://secure.travis-ci.org/tjdett/atom-dataset-provider.png)](http://travis-ci.org/tjdett/atom-dataset-provider)

About
-----

This app provides a tiny web-server for exposing a directory via an Atom feed.
It is intended to act as a producer for the [MyTardis Atom app][atom-app].

Platform Support
----------------

This app is targeted at [Node.js][nodejs] 0.6.x on Linux and Windows.

Due to a lack of uid support in Windows (and the relatively immature APIs
currently available) performance will be MUCH better on Linux.


Installing
----------

Once you've checked out the latest version of this app from Github, you can 
install the dependencies with [NPM][npm] (which is bundled with Node.js) 
and run the tests:

    npm install
    npm test

Usage
-----

To serve up the directory `~/mydir` on port 8001:

    bin/atom-dataset-provider -d ~/mydir -p 8001

Run `bin/atom-dataset-provider --help` for a full list of options.

[atom-app]: https://github.com/tjdett/mytardis-app-atom
[nodejs]: http://nodejs.org/
[npm]: http://npmjs.org/
