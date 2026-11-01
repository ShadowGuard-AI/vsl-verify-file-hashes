# vsl-verify-file-hashes
Calculates and compares the cryptographic hash of a file against a known or provided hash, to verify file integrity.

## Install
`git clone https://github.com/ShadowGuard-AI/vsl-verify-file-hashes`

## Usage
`python main.py filepath [-a algorithm] [-c compare_hash]`

## Parameters
- `filepath`: Path to the file to be verified (positional, required)
- `-h`: Show help message and exit
- `-a`, `--algorithm`: Hash algorithm to use, one of sha256, sha1, md5 (default: sha256)
- `-c`, `--compare_hash`: Hash value to compare against. Must be hexadecimal of the length the chosen algorithm produces. If not provided, only calculate the hash. A mismatch exits non-zero, and a malformed comparison value is rejected with an error at non-zero exit.

## License
Copyright (c) ShadowGuard-AI
