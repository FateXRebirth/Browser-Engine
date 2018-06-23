# Browser-Engine

I am going to build a HTML rendering engine by using a new language called [Rust](https://www.rust-lang.org/en-US/).

You can build your own, you can follow [Matt Brubeck's tutorial](https://limpet.net/mbrubeck/2014/08/08/toy-layout-engine-1.html) if you have no idea.

Instructions
------------

1. [Install Rust.](http://www.rust-lang.org/install.html)

2. Run `cargo build` to build robinson, and `cargo run` to run it.

To build and run with optimizations enabled, use `cargo build --release` and
`cargo run --release`.

By default, rust-browser-engine will load test.html and test.css from the `examples`
directory.  You can use the `--html` and `--css` arguments to the rust-browser-engine
executable to change the input files:

    ./target/debug/rust-browser-engine --html examples/test.html --css examples/test.css

The rendered page will be saved to a file named `output.png`.  To change the
output filename, use the `-o` option.  To switch to PDF output, use add
`--format pdf`.
