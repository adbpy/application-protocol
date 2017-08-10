# application-protocol

[![Build Status](https://travis-ci.org/adbpy/application-protocol.svg?branch=master)](https://travis-ci.org/adbpy/application-protocol)
[![Test Coverage](https://codeclimate.com/github/adbpy/application-protocol/badges/coverage.svg)](https://codeclimate.com/github/adbpy/application-protocol/coverage)
[![Code Climate](https://codeclimate.com/github/adbpy/application-protocol/badges/gpa.svg)](https://codeclimate.com/github/adbpy/application-protocol)
[![Issue Count](https://codeclimate.com/github/adbpy/application-protocol/badges/issue_count.svg)](https://codeclimate.com/github/adbpy/application-protocol)

[![Stories in Ready](https://badge.waffle.io/adbpy/application-protocol.svg?label=ready&title=Ready)](http://waffle.io/adbpy/application-protocol)

Android Debug Bridge (ADB) Application Protocol

## Status

This project is actively maintained and under development.

## Installation

To install application-protocol from [pip](https://pypi.python.org/pypi/pip):
```bash
    $ pip install adbap
```

To install application-protocol from source:
```bash
    $ git clone git@github.com:adbpy/application-protocol.git
    $ cd application-protocol && python setup.py install
```

## Goals/Scope

A standalone library that can be used for providing high level actions for communicating with devices. The application protocol
is the single merge point of [transport-protocol](https://github.com/adbpy/transport-protocoll) and message serialization
in [wire-protocol](https://github.com/adbpy/wire-protocol).
The application protocol should care about:

* Synchronous vs. Asynchronous constructs
* Creating connections between devices
* Cryptographic handshake during authentication
* High level interfaces (services)

The application protocol should not care about:

* Byte layout on the wire
* Communication transport idiosyncrasies (UDP vs. TCP vs. USB)

## Contributing

If you would like to contribute, simply fork the repository, push your changes and send a pull request.
Pull requests will be brought into the `master` branch via a rebase and fast-forward merge with the goal of having a linear branch history with no merge commits.

## License

[Apache 2.0](LICENSE)
