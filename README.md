# Base32 encoder and decoder for PHP

A simple library that implements the capability of encoding and decoding base32 in PHP, that ~~kind of~~ follows the RFC 4648.

# Usage
____

There is no secret on using this library it have just two functions(for now), one to encode and the other one to decode. 

## Encoding
```
include('base.php');

$data = 'hello';

echo Base::b32encode($data);
// Output: NBSWY3DP 
```

## Decoding
```
include('base.php');

$data = 'NBSWY3DP';

echo Base::b32decode($data);
// Output: 'hello'
```

OBS.: This library do not increment padding with '='.
