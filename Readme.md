# watch-run(2)

Re-execute a given command everytime something changes in a specific directory.

## Installation

	$ npm install -g watch-run

## Usage

Via --help:

```
Usage: watch <cmd>

Options:

  -h, --help               output usage information
  -p, --pattern <pattern>  glob pattern


Examples:

  # watch dir and execute cmd
  $ watch-run -p 'lib/**' cat package.json
```

`--pattern` can be a glob pattern, a normal directory or just simply a file. For more information on glob patterns take a look at [isaacs minimatch documentation](https://github.com/isaacs/minimatch) which this module is build upon.

`command` can be anything you like. The posibilities are endless here, you can watch for `.sass` files and run the sass cli everytime something changes or you can even bundle your browserify modules.

## Example

	$ watch-run -p 'js/modules/**/*.js' browserify main.js -o public/build.js

## License

MIT