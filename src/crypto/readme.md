# Crypto wrappers

This directory contains minor convenience wrappers around
[libsodium](http://libsodium.org), a copy of which is stored in the
[lib/libsodium](stellar/libsodium/tree/c5e43f4c1cf62b4669b1f33516fc33ef2d005187) submodule of the `stellar-core`
distribution, and compiled along with it.

The crypto module also contains a small implementation to turn public/private
keys into human manageable strings (StrKey).

The crypto wrappers are intended to be minimal, transparent, safe and simple;
they should not "enhance", "customize" or otherwise alter any of the
cryptographic principles or primitives provided by libsodium. Any "surprising"
behavior, for a knowledgable user of libsodium, should be considered a bug.
