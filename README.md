co.py.cat
=========

An implementation of [Douglas Hofstadter](http://prelectur.stanford.edu/lecturers/hofstadter/)'s copycat algorithm. The copycat algorithm is explained [on Wikipedia](https://en.wikipedia.org/wiki/Copycat_%28software%29), and that page has many links for deeper reading.

This implementation is a copycat of Scott Boland's [Java implementation](http://itee.uq.edu.au/~scottb/_Copycat/), but re-written into Python. It's not a direct translation - but based on his code. I did not carry over the GUI, as this version can more usefully be run from command line, or imported for use by other Python scripts.

In cases where I could not grok the Java implementation easily I took ideas from the [LISP implementation](http://web.cecs.pdx.edu/~mm/how-to-get-copycat.html), or directly from [Melanie Mitchell](https://en.wikipedia.org/wiki/Melanie_Mitchell)'s "[Analogy-Making as Perception](http://www.amazon.com/Analogy-Making-Perception-Computer-Melanie-Mitchell/dp/0262132893/ref=tmm_hrd_title_0?ie=UTF8&qid=1351269085&sr=1-3)"

I also tried to make the code more pythonic.

Installation
------------

There are no particular installation instructions, just clone and run, e.g.

```sh
$ git clone https://github.com/jalanb/co.py.cat.git
$ cd co.py.cat/copycat
$ python main.py abc abd ijk
```

Running
-------

The script takes three arguments.
    The first two are a pair of triplets with some change, for example "abc" and "abd".
    The third is a triplet which the script should try to change analogously

For example the following invocation will probably display "ijl"

```sh
$ python main.py abc abd ijk
```

Badges
------
[![Build Status](https://travis-ci.org/jalanb/co.py.cat.svg?branch=master)](https://travis-ci.org/jalanb/co.py.cat)

See Also
--------
1. "[The Copycat Project: An Experiment in Nondeterminism and Creative Analogies](http://dspace.mit.edu/handle/1721.1/5648)" by [Hofstadter, Douglas](https://en.wikipedia.org/wiki/Douglas_Hofstadter#Academic_career)
1. "[Analogy-Making as Perception](http://www.amazon.com/Analogy-Making-Perception-Computer-Melanie-Mitchell/dp/0262132893/ref=tmm_hrd_title_0?ie=UTF8&qid=1351269085&sr=1-3)" by [Mitchell, Melanie](https://en.wikipedia.org/wiki/Melanie_Mitchell)
1. Arthur O'Dwyer ([Quuxplusone on GitHub]()) has further cleaned and extended this code in a fork available [here](https://github.com/Quuxplusone/co.py.cat).
