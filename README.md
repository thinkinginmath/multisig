# multisig

A few files for prototyping on multi-party signature for possible use in blockchain consensus 
algorithms or cryptocurrency.


https://github.com/enzoh/go-bls provides a simple Go wrapper of pbc C library.
It does not provide proper serialziation support (e.g., for key pair and other parameters).
If we were to use this library, we need to amend many methods.

An alternative would be to extend the Go PBC, a more generic pair-based crypto library. 
It is at https://github.com/Nik-U/pbc

Another point of reference is https://github.com/dfinity/go-dfinity-crypto from the DFINITY
project. However, the BLS wrapper does not provide  signature aggregate support. 