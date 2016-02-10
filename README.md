hdkey
=====

[![build status](https://secure.travis-ci.org/cryptocoinjs/hdkey.png)](http://travis-ci.org/cryptocoinjs/hdkey)
[![Coverage Status](https://img.shields.io/coveralls/cryptocoinjs/hdkey.svg)](https://coveralls.io/r/cryptocoinjs/hdkey)

A JavaScript component for [BIP32](https://github.com/bitcoin/bips/blob/master/bip-0032.mediawiki)(hierarchical deterministic keys).

Thanks to the active BitcoinJS team and their hard work - some code borrowed from it.

**Note: Will be deprecating and replacing with** https://github.com/bitcoinjs/bip32

Installation
------------

    npm i --save hdkey


Usage
-----

**example:**

```js
var HDKey = require('hdkey')
var seed = 'a0c42a9c3ac6abf2ba6a9946ae83af18f51bf1c9fa7dacc4c92513cc4dd015834341c775dcd4c0fac73547c5662d81a9e9361a0aac604a73a321bd9103bce8af'
var hdkey = HDKey.fromMasterSeed(new Buffer(seed, 'hex'))
console.log(mk.privateExtendedKey)
// => 'xprv9s21ZrQH143K2SKJK9EYRW3Vsg8tWVHRS54hAJasj1eGsQXeWDHLeuu5hpLHRbeKedDJM4Wj9wHHMmuhPF8dQ3bzyup6R7qmMQ1i1FtzNEW'
console.log(mk.publicExtendedKey)
// => 'xpub661MyMwAqRbcEvPmRAmYndzERhyNux1GoHzHxgzVHMBFkCro3kbbCiDZZ5XabZDyXPj5mH3hktvkjhhUdCQxie5e1g4t2GuAWNbPmsSfDp2'
```



References
----------
- https://github.com/bitcoinjs/bitcoinjs-lib/blob/master/src/hdnode.js
- http://bip32.org/
- http://blog.richardkiss.com/?p=313
- https://github.com/bitcoin/bips/blob/master/bip-0032.mediawiki
- http://bitcoinmagazine.com/8396/deterministic-wallets-advantages-flaw/
