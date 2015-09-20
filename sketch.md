# Plan for world takeover by Tim and Michael :-)

## Design patterns in Haskell vs JavaScript

* Functor as a value that is packaged in a special way, and may be only transformed within the package
* Applicative as a Functor-like type with allowance for merging different streams of computation (zipping)
* Traversal as generator/transducer like in Clojure
* Foldable with fold/map/mapM/scan as basic example of structured recursion (reduction and mapping)
* Alternative/ArrowChoice as basic example of design by combinators
* Monad - promise computation pattern for streamlining asynchronous callbacks
* Free monad - command pattern
  - Abstract interpretation and execution of the same code
* Arrow - explicit dataflow graph

## Examples that we can run on

* We may use JavaScript Promises as an example of Monad.

* We may use ReactJS as example for pure Applicative.

* Use arrow for describing reactive values (React in JS, vs Netwire in Haskell), and then show how to extract dependency graph out of these.

* _We probably need a practical example of functor that is not a Monad/Applicative,
and Applicative that is not a Monad_

* Incremental parsing of asynchronously loaded [Test Anything Protocol](https://testanything.org/) output.

* Streams as a basic computation, where individual transformations are described within Monad, but composed using Arrow.
  - Unix pipes: grep | cut | uniq | sort
  - Or HashSort

* Check examples from PreludeJS
  - Standard library for LiveScript
  - CoffeeScript -> CocoJS -> PreludeJS = LiveScript -> CoffeeScript -> ECMAScript
  - Roy
    * Brian McKenna
      - https://github.com/fantasyland/fantasy-land - example translation of classes to JS
      - https://github.com/fantasyland/implementations.md - example instances

* Callback hell example

## Other aspects...

Ideally we could make a tutorial with Haskell and JavaScript side-to-side in the browser.

### Goals

* Tim: make a lasting project that will help in future work.
* Michal: learn how to make Haskell patterns more accessible to everyone.
