# libsignal-node

Signal protocol implementation for Node.js based on [libsignal-protocol-javascript](https://github.com/WhisperSystems/libsignal-protocol-javascript).

[![npm](https://img.shields.io/npm/v/libsignal.svg)](https://www.npmjs.com/package/libsignal)
[![npm](https://img.shields.io/npm/l/libsignal.svg)](https://github.com/ForstaLabs/libsignal-node)

### Overview

A forward secrecy protocol for secure messaging in both synchronous and asynchronous environments.

### PreKeys

PreKeys are ECPublicKeys with unique IDs stored on a server. Clients generate one signed PreKey and multiple unsigned PreKeys at install time.

### Sessions

Signal Protocol establishes a session for encryption, which remains active indefinitely. Sessions are created through:

1. PreKeyBundles – retrieved from the server.
2. PreKeySignalMessages – received from the recipient.

### State

Session state is stored in:

- Identity State (own and others' identity keys).
- PreKey State (generated PreKeys).
- Signed PreKey State.
- Session State (active sessions).

### License

GPLv3 License - [GPLv3](http://www.gnu.org/licenses/gpl-3.0.html)  
© 2015-2018 Open Whisper Systems & Forsta Inc.
