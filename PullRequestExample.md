# What this PR does?
* Fixes build on Ubuntu and MacOS
* Extracts QubeCppUtils as an external project
* Introduces unit tests for LibDCP

# Dependencies
* cmake > 2.8
* boost
* openssl
* xerces-c
* xml-security-c

# How to test
* `mkdir build`
* `cd build`
* `cmake .. -DBUILD_ALL=1` (for MacOS we should define something like this: -DOPENSSL_ROOT_DIR=/usr/local/Cellar/openssl/1.0.2j)
* `make`
* `make test` (if it was built with '-DBUILD_ALL=1')
