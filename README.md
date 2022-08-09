# Base32 encoder and decoder for PHP

A simple library that implements the capability of encoding and decoding for base32 and base16 in PHP, that ~~kind of~~ follows the RFC 4648.

# Usage
____

There is no secret on using this library it have just four functions two for base32 and two for base16, one to encode and the other one to decode. 

## Encoding Base32
```
include('base.php');

$data = 'hello';

echo Base::b32encode($data);
// Output: NBSWY3DP 
```

## Decoding Base32
```
include('base.php');

$data = 'NBSWY3DP';

echo Base::b32decode($data);
// Output: 'hello'
```

OBS.: This library do not increment padding with '='.

## Encoding Base16
```
include('base.php');

$data = 'hello';

echo Base::b16encode($data);
// Output: 68656C6C6F 
```

## Decoding Base32
```
include('base.php');

$data = '68656C6C6F';

echo Base::b16decode($data);
// Output: 'hello'
```
