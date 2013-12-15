# watch-run(2)

watch specific files or directories and re-execute a given command

## Installation

	$ npm install -g watch-run

## Usage

	$ watch-run <folder> <command>

`folder` can be a glob pattern or just a normal directory or file. For example, you can watch only for `js` changes in your directory like this `lib/**/*.js`. For more information on glob patterns take a look at [isaacs minimatch](https://github.com/isaacs/minimatch).

`command` can be anything you like. The Posibilities are endless here, you can watch for `.sass` files and run the sass cli everytime something changes or you can even bundle your browserify modules. Get creative!

## License

MIT



