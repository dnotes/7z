# Docker command-line 7zip image

This docker app is built from alpine:edge with the most recent p7zip package; thus, it should keep relatively up-to-date with the latest advancements in 7zip format.

## Requirements

- Docker :whale:

## Usage

Run the image, mounting the folder containing your data as /app, and then work with files as if you are currently in /app. So:

    docker run -it --rm -v $(pwd):/app dnotes/7z [cmd]

As an example, to extract `/home/dnotes/file.7z`, you would run one of the following:

    docker run -it --rm -v /home/dnotes:/app dnotes/7z x file.7z` 

or

    cd /home/dnotes
    docker run -it --rm -v $(pwd):/app dnotes/7z x file.7z
