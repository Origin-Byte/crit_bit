# Critbit

A critical bit (critbit) tree is a compact binary prefix tree,
similar to a binary search tree, that stores a prefix-free set of
bitstrings, like n-bit integers or variable-length 0-terminated byte
strings.

Critbit trees support fast insertion, deletion and iteration operations
as they do not need to be rebalanced.

## References

- [Bernstein 2006](https://cr.yp.to/critbit.html)
- [Langley 2008](https://www.imperialviolet.org/2008/09/29/critbit-trees.html)
- [Langley 2012](https://github.com/agl/critbit)
- [Tcler's Wiki 2021](https://wiki.tcl-lang.org/page/critbit)

## Implementation

This package re-exports
[Deepbook's critbit implementation](https://github.com/MystenLabs/sui/tree/main/crates/sui-framework/packages/deepbook)
which uses a dynamic-field backed structure to allow large tree structures
that don't exceed Sui's object size limit.
