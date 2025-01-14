# txt2html

Static Site Generator that converts .txt to .html

## Features

-   Support for custom stylesheets
-   Custom output directory

## Installation

To run this script you need to:

1. `git clone https://github.com/tcvan0707/txt2html.git && cd txt2html`
2. `npm install`

## Example

Running `npm start -- -i hello.txt` containing

```
Hello world!

This world is beautiful
```

will generate output file `dist/hello.html` containing

```
<!doctype html>
<html lang="en">
<head>
  <meta charset="utf-8">
  <title>hello</title>
  <meta name="viewport" content="width=device-width, initial-scale=1">

</head>
<body>
<p>Hello world!</p>
<p>This world is beautiful</p>
</body>
</html>
```

## Usage

```
Usage: txt2html.js [options]

Options:
  -h, --help        Show help message                                  [boolean]
  -v, --version     Show current version                               [boolean]
  -i, --input       Input txt file / directory with txt files         [required]
  -o, --output      Path to folder with generated files        [default: "dist"]
  -s, --stylesheet  Adds custom CSS to generated html
```
