# @crypto/ring — Cryptography for Zeta

Auto-configured via Dark Factory from [ring](https://crates.io/crates/ring) v0.17.14.

## Features
| Category | Algorithms |
|----------|------------|
| **Symmetric** | AES-GCM, ChaCha20-Poly1305 |
| **Hashing** | SHA-2 (224/256/384/512), SHA-1 |
| **MAC** | HMAC (SHA-2 family) |
| **Key Agreement** | ECDH (P-256, P-384, X25519) |
| **Signing** | ECDSA (P-256, P-384), Ed25519, RSA PKCS#1 v1.5/PSS |
| **KDF** | PBKDF2, HKDF |
| **TLS** | TLS 1.3 primitives, QUIC header protection |

## Usage
```zeta
use @crypto/ring::{digest, hmac, rand};

let key = hmac::Key::generate();
let tag = hmac::sign(&key, b"message");
```

## Stats: ~10,419 lines across 153 source files, 0 unsupported items

## License
MIT