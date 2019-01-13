# Usage

## Syntax

General syntax is:

```bash
docker run -it -v /path/where/to/download:/app yle-dl
url-to-download-from
```

## Example

For instance, downloading a file to current directory:

```bash
docker run -it -v $(pwd):/app yle-dl
https://areena.yle.fi/1-50026988
```