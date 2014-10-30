# Evan Sosenko's curriculum vitae

This is the LaTeX source for my curriculum vitae.

My curriculum vitae with a link to the PDF version
can be found at [evansosenko.com/cv/](https://evansosenko.com/cv/).

## Requirements

- `xelatex` and [`latexmk`](http://www.ctan.org/pkg/latexmk/),
  packaged with a modern LaTeX distribution,
  e.g., [TeX Live](http://www.tug.org/texlive/).
- [Font Awesome](http://fortawesome.github.io/Font-Awesome/).
- [Ruby 2](https://www.ruby-lang.org/)
  with [Bundler](http://bundler.io/) (optional).

## Building

### With Ruby

If you have Ruby with Bundler, install the needed gems with

````bash
$ bundle
````

To build all targets,

````bash
$ rake
````

Output files will be saved in the `build` directory.

To see other rake tasks,

````bash
$ rake -D
````

You can run

````bash
$ guard
````

which will automatically rebuild on changes.

### Without Ruby

To build the tex source,

````bash
$ cd tex
$ latexmk -xelatex curriculum_vitae.tex
````

## License

This work is Copyright © 2013-2014 Evan Sosenko.

## Warranty

This work is provided "as is" and without any express or
implied warranties, including, without limitation, the implied
warranties of merchantibility and fitness for a particular
purpose.
