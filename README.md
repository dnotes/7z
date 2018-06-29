# Docker command-line 7zip image

This docker app is built from alpine:edge with the most recent p7zip package; thus, it should keep relatively up-to-date with the latest advancements in 7zip format.

## Requirements

- Docker :whale:

# Usage

`docker run --rm -v $(pwd):/app dnotes/7z [cmd]`
