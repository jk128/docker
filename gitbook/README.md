## Usage

GitBook container image with PDF, ePub and Mobi exports through Calibre library.

Example:

```bash
docker run -it -v ./:/data madkom/gitbook
```

## Serving documentation with watch support

Just run container, optionally add ports, format and log level params:

```bash
docker run -it -v ./:/data madkom/gitbook serve --port=4000 --lrport=35729 --watch --format=[website, json, ebook] --log=[debug, info, warn, error, disabled]
```

## Building documentation

Run container with build command, optionally add format and log level params:

```bash
docker run -it -v ./:/data madkom/gitbook build --format=[website, json, ebook] --log=[debug, info, warn, error, disabled]
```

## Development

```bash
make build
```

## License

The MIT License (MIT)

Copyright (c) 2015 Madkom

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.
