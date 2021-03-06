# Dash Crypto
The cryptographic primitives (ECDSA and HMAC) implementations in this package have been reviewed on the upstream repository, no changes have been done since then, however, more audits and reviews are welcomed.

## Random
The `pacglobal.crypto.Random` namespace contains a single function, named `getRandomBuffer(size)` that returns a `Buffer` instance with random bytes. It may not work depending on the engine that Pacglobal is running on (doesn't work with IE versions lesser than 11).

## BN
The `pacglobal.crypto.BN` class contains a wrapper around [bn.js](https://github.com/indutny/bn.js), the bignum library used internally in Pacglobal.

## Point
The `pacglobal.crypto.Point` class contains a wrapper around the class Point of [elliptic.js](https://github.com/indutny/elliptic), the elliptic curve library used internally in Pacglobal.

## Hash
The `pacglobal.crypto.Hash` namespace contains a set of hashes and utilities. These are either the native `crypto` hash functions from `node.js` or their respective browser shims as provided by the `browserify` library.

## ECDSA
`pacglobal.crypto.ECDSA` contains a pure JavaScript implementation of the elliptic curve DSA signature scheme based on [elliptic.js](https://github.com/indutny/elliptic).
