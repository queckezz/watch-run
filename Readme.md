# watch-run(2)

Watch specific files or directories based on a pattern and re-execute a given command everytime something changes, beeing added or removed.

![](https://i.cloudup.com/uwoCuagFjWg/V5m7Kg.png)

## Installation

	$ npm install -g watch-run

## Usage

	$ watch-run <pattern> <command>

And to get awesome debug messages use the `DEBUG` environment variable.
  
	$ DEBUG=watch watch-run <pattern> <command>

`pattern` can be a glob pattern, a normal directory or just simply a file. For example, you can watch only for `js` changes in your `lib` folder like this `lib/**/*.js`. For more information on glob patterns take a look at [isaacs minimatch documentation](https://github.com/isaacs/minimatch).

`command` can be anything you like. The posibilities are endless here, you can watch for `.sass` files and run the sass cli everytime something changes or you can even bundle your browserify modules. Get creative!

## License

MIT



