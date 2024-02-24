<!--

@license Apache-2.0

Copyright (c) 2020 The Stdlib Authors.

Licensed under the Apache License, Version 2.0 (the "License");
you may not use this file except in compliance with the License.
You may obtain a copy of the License at

   http://www.apache.org/licenses/LICENSE-2.0

Unless required by applicable law or agreed to in writing, software
distributed under the License is distributed on an "AS IS" BASIS,
WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
See the License for the specific language governing permissions and
limitations under the License.

-->


<details>
  <summary>
    About stdlib...
  </summary>
  <p>We believe in a future in which the web is a preferred environment for numerical computation. To help realize this future, we've built stdlib. stdlib is a standard library, with an emphasis on numerical and scientific computation, written in JavaScript (and C) for execution in browsers and in Node.js.</p>
  <p>The library is fully decomposable, being architected in such a way that you can swap out and mix and match APIs and functionality to cater to your exact preferences and use cases.</p>
  <p>When you use stdlib, you can be absolutely certain that you are using the most thorough, rigorous, well-written, studied, documented, tested, measured, and high-quality code out there.</p>
  <p>To join us in bringing numerical computing to the web, get started by checking us out on <a href="https://github.com/stdlib-js/stdlib">GitHub</a>, and please consider <a href="https://opencollective.com/stdlib">financially supporting stdlib</a>. We greatly appreciate your continued support!</p>
</details>

# Sequences

[![NPM version][npm-image]][npm-url] [![Build Status][test-image]][test-url] [![Coverage Status][coverage-image]][coverage-url] <!-- [![dependencies][dependencies-image]][dependencies-url] -->

> Math iterators for generating sequences.

<section class="installation">

## Installation

```bash
npm install @stdlib/math-iter-sequences
```

Alternatively,

-   To load the package in a website via a `script` tag without installation and bundlers, use the [ES Module][es-module] available on the [`esm`][esm-url] branch (see [README][esm-readme]).
-   If you are using Deno, visit the [`deno`][deno-url] branch (see [README][deno-readme] for usage intructions).
-   For use in Observable, or in browser/node environments, use the [Universal Module Definition (UMD)][umd] build available on the [`umd`][umd-url] branch (see [README][umd-readme]).

The [branches.md][branches-url] file summarizes the available branches and displays a diagram illustrating their relationships.

To view installation and usage instructions specific to each branch build, be sure to explicitly navigate to the respective README files on each branch, as linked to above.

</section>

<section class="usage">

## Usage

```javascript
var ns = require( '@stdlib/math-iter-sequences' );
```

#### ns

Namespace containing math iterators for generating sequences.

```javascript
var iterators = ns;
// returns {...}
```

The namespace contains the following functions for creating iterator protocol-compliant iterators:

<!-- <toc pattern="*"> -->

<div class="namespace-toc">

-   <span class="signature">[`iterCompositesSeq( [options] )`][@stdlib/math/iter/sequences/composites]</span><span class="delimiter">: </span><span class="description">create an iterator which generates a sequence of composite numbers.</span>
-   <span class="signature">[`iterContinuedFractionSeq( x, [options] )`][@stdlib/math/iter/sequences/continued-fraction]</span><span class="delimiter">: </span><span class="description">create an iterator which generates a list of all continued fraction terms which can be obtained given the precision of a provided number.</span>
-   <span class="signature">[`iterCubesSeq( [options] )`][@stdlib/math/iter/sequences/cubes]</span><span class="delimiter">: </span><span class="description">create an iterator which generates a sequence of cubes.</span>
-   <span class="signature">[`iterEvenIntegersSeq( [options] )`][@stdlib/math/iter/sequences/even-integers]</span><span class="delimiter">: </span><span class="description">create an iterator which generates an interleaved sequence of even integers.</span>
-   <span class="signature">[`iterFactorialsSeq( [options] )`][@stdlib/math/iter/sequences/factorials]</span><span class="delimiter">: </span><span class="description">create an iterator which generates a sequence of factorials.</span>
-   <span class="signature">[`iterFibonacciSeq( [options] )`][@stdlib/math/iter/sequences/fibonacci]</span><span class="delimiter">: </span><span class="description">create an iterator which generates a Fibonacci sequence.</span>
-   <span class="signature">[`iterFifthPowersSeq( [options] )`][@stdlib/math/iter/sequences/fifth-powers]</span><span class="delimiter">: </span><span class="description">create an iterator which generates a sequence of fifth powers.</span>
-   <span class="signature">[`iterFourthPowersSeq( [options] )`][@stdlib/math/iter/sequences/fourth-powers]</span><span class="delimiter">: </span><span class="description">create an iterator which generates a sequence of fourth powers.</span>
-   <span class="signature">[`iterIntegersSeq( [options] )`][@stdlib/math/iter/sequences/integers]</span><span class="delimiter">: </span><span class="description">create an iterator which generates an interleaved integer sequence.</span>
-   <span class="signature">[`iterLucasSeq( [options] )`][@stdlib/math/iter/sequences/lucas]</span><span class="delimiter">: </span><span class="description">create an iterator which generates a Lucas sequence.</span>
-   <span class="signature">[`iterNegaFibonacciSeq( [options] )`][@stdlib/math/iter/sequences/negafibonacci]</span><span class="delimiter">: </span><span class="description">create an iterator which generates a negaFibonacci sequence.</span>
-   <span class="signature">[`iterNegaLucasSeq( [options] )`][@stdlib/math/iter/sequences/negalucas]</span><span class="delimiter">: </span><span class="description">create an iterator which generates a negaLucas sequence.</span>
-   <span class="signature">[`iterNegativeEvenIntegersSeq( [options] )`][@stdlib/math/iter/sequences/negative-even-integers]</span><span class="delimiter">: </span><span class="description">create an iterator which generates a sequence of negative even integers.</span>
-   <span class="signature">[`iterNegativeIntegersSeq( [options] )`][@stdlib/math/iter/sequences/negative-integers]</span><span class="delimiter">: </span><span class="description">create an iterator which generates a negative integer sequence.</span>
-   <span class="signature">[`iterNegativeOddIntegersSeq( [options] )`][@stdlib/math/iter/sequences/negative-odd-integers]</span><span class="delimiter">: </span><span class="description">create an iterator which generates a sequence of negative odd integers.</span>
-   <span class="signature">[`iterNonFibonacciSeq( [options] )`][@stdlib/math/iter/sequences/nonfibonacci]</span><span class="delimiter">: </span><span class="description">create an iterator which generates a non-Fibonacci integer sequence.</span>
-   <span class="signature">[`iterNonNegativeEvenIntegersSeq( [options] )`][@stdlib/math/iter/sequences/nonnegative-even-integers]</span><span class="delimiter">: </span><span class="description">create an iterator which generates a sequence of nonnegative even integers.</span>
-   <span class="signature">[`iterNonNegativeIntegersSeq( [options] )`][@stdlib/math/iter/sequences/nonnegative-integers]</span><span class="delimiter">: </span><span class="description">create an iterator which generates a nonnegative integer sequence.</span>
-   <span class="signature">[`iterNonPositiveEvenIntegersSeq( [options] )`][@stdlib/math/iter/sequences/nonpositive-even-integers]</span><span class="delimiter">: </span><span class="description">create an iterator which generates a sequence of nonpositive even integers.</span>
-   <span class="signature">[`iterNonPositiveIntegersSeq( [options] )`][@stdlib/math/iter/sequences/nonpositive-integers]</span><span class="delimiter">: </span><span class="description">create an iterator which generates a nonpositive integer sequence.</span>
-   <span class="signature">[`iterNonSquaresSeq( [options] )`][@stdlib/math/iter/sequences/nonsquares]</span><span class="delimiter">: </span><span class="description">create an iterator which generates a sequence of nonsquares.</span>
-   <span class="signature">[`iterOddIntegersSeq( [options] )`][@stdlib/math/iter/sequences/odd-integers]</span><span class="delimiter">: </span><span class="description">create an iterator which generates an interleaved sequence of odd integers.</span>
-   <span class="signature">[`iterPositiveEvenIntegersSeq( [options] )`][@stdlib/math/iter/sequences/positive-even-integers]</span><span class="delimiter">: </span><span class="description">create an iterator which generates a sequence of positive even integers.</span>
-   <span class="signature">[`iterPositiveIntegersSeq( [options] )`][@stdlib/math/iter/sequences/positive-integers]</span><span class="delimiter">: </span><span class="description">create an iterator which generates a positive integer sequence.</span>
-   <span class="signature">[`iterPositiveOddIntegersSeq( [options] )`][@stdlib/math/iter/sequences/positive-odd-integers]</span><span class="delimiter">: </span><span class="description">create an iterator which generates a sequence of positive odd integers.</span>
-   <span class="signature">[`iterPrimesSeq( [options] )`][@stdlib/math/iter/sequences/primes]</span><span class="delimiter">: </span><span class="description">create an iterator which generates a sequence of prime numbers.</span>
-   <span class="signature">[`iterSquaredTriangularSeq( [options] )`][@stdlib/math/iter/sequences/squared-triangular]</span><span class="delimiter">: </span><span class="description">create an iterator which generates a sequence of squared triangular numbers.</span>
-   <span class="signature">[`iterSquaresSeq( [options] )`][@stdlib/math/iter/sequences/squares]</span><span class="delimiter">: </span><span class="description">create an iterator which generates a sequence of squares.</span>
-   <span class="signature">[`iterTriangularSeq( [options] )`][@stdlib/math/iter/sequences/triangular]</span><span class="delimiter">: </span><span class="description">create an iterator which generates a sequence of triangular numbers.</span>

</div>

<!-- </toc> -->

</section>

<!-- /.usage -->

<section class="examples">

## Examples

<!-- TODO: better examples -->

<!-- eslint no-undef: "error" -->

```javascript
var objectKeys = require( '@stdlib/utils-keys' );
var ns = require( '@stdlib/math-iter-sequences' );

console.log( objectKeys( ns ) );
```

</section>

<!-- /.examples -->

<!-- Section for related `stdlib` packages. Do not manually edit this section, as it is automatically populated. -->

<section class="related">

</section>

<!-- /.related -->

<!-- Section for all links. Make sure to keep an empty line after the `section` element and another before the `/section` close. -->


<section class="main-repo" >

* * *

## Notice

This package is part of [stdlib][stdlib], a standard library for JavaScript and Node.js, with an emphasis on numerical and scientific computing. The library provides a collection of robust, high performance libraries for mathematics, statistics, streams, utilities, and more.

For more information on the project, filing bug reports and feature requests, and guidance on how to develop [stdlib][stdlib], see the main project [repository][stdlib].

#### Community

[![Chat][chat-image]][chat-url]

---

## License

See [LICENSE][stdlib-license].


## Copyright

Copyright &copy; 2016-2024. The Stdlib [Authors][stdlib-authors].

</section>

<!-- /.stdlib -->

<!-- Section for all links. Make sure to keep an empty line after the `section` element and another before the `/section` close. -->

<section class="links">

[npm-image]: http://img.shields.io/npm/v/@stdlib/math-iter-sequences.svg
[npm-url]: https://npmjs.org/package/@stdlib/math-iter-sequences

[test-image]: https://github.com/stdlib-js/math-iter-sequences/actions/workflows/test.yml/badge.svg?branch=v0.2.1
[test-url]: https://github.com/stdlib-js/math-iter-sequences/actions/workflows/test.yml?query=branch:v0.2.1

[coverage-image]: https://img.shields.io/codecov/c/github/stdlib-js/math-iter-sequences/main.svg
[coverage-url]: https://codecov.io/github/stdlib-js/math-iter-sequences?branch=main

<!--

[dependencies-image]: https://img.shields.io/david/stdlib-js/math-iter-sequences.svg
[dependencies-url]: https://david-dm.org/stdlib-js/math-iter-sequences/main

-->

[chat-image]: https://img.shields.io/gitter/room/stdlib-js/stdlib.svg
[chat-url]: https://app.gitter.im/#/room/#stdlib-js_stdlib:gitter.im

[stdlib]: https://github.com/stdlib-js/stdlib

[stdlib-authors]: https://github.com/stdlib-js/stdlib/graphs/contributors

[umd]: https://github.com/umdjs/umd
[es-module]: https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Modules

[deno-url]: https://github.com/stdlib-js/math-iter-sequences/tree/deno
[deno-readme]: https://github.com/stdlib-js/math-iter-sequences/blob/deno/README.md
[umd-url]: https://github.com/stdlib-js/math-iter-sequences/tree/umd
[umd-readme]: https://github.com/stdlib-js/math-iter-sequences/blob/umd/README.md
[esm-url]: https://github.com/stdlib-js/math-iter-sequences/tree/esm
[esm-readme]: https://github.com/stdlib-js/math-iter-sequences/blob/esm/README.md
[branches-url]: https://github.com/stdlib-js/math-iter-sequences/blob/main/branches.md

[stdlib-license]: https://raw.githubusercontent.com/stdlib-js/math-iter-sequences/main/LICENSE

<!-- <toc-links> -->

[@stdlib/math/iter/sequences/composites]: https://github.com/stdlib-js/math-iter-sequences-composites

[@stdlib/math/iter/sequences/continued-fraction]: https://github.com/stdlib-js/math-iter-sequences-continued-fraction

[@stdlib/math/iter/sequences/cubes]: https://github.com/stdlib-js/math-iter-sequences-cubes

[@stdlib/math/iter/sequences/even-integers]: https://github.com/stdlib-js/math-iter-sequences-even-integers

[@stdlib/math/iter/sequences/factorials]: https://github.com/stdlib-js/math-iter-sequences-factorials

[@stdlib/math/iter/sequences/fibonacci]: https://github.com/stdlib-js/math-iter-sequences-fibonacci

[@stdlib/math/iter/sequences/fifth-powers]: https://github.com/stdlib-js/math-iter-sequences-fifth-powers

[@stdlib/math/iter/sequences/fourth-powers]: https://github.com/stdlib-js/math-iter-sequences-fourth-powers

[@stdlib/math/iter/sequences/integers]: https://github.com/stdlib-js/math-iter-sequences-integers

[@stdlib/math/iter/sequences/lucas]: https://github.com/stdlib-js/math-iter-sequences-lucas

[@stdlib/math/iter/sequences/negafibonacci]: https://github.com/stdlib-js/math-iter-sequences-negafibonacci

[@stdlib/math/iter/sequences/negalucas]: https://github.com/stdlib-js/math-iter-sequences-negalucas

[@stdlib/math/iter/sequences/negative-even-integers]: https://github.com/stdlib-js/math-iter-sequences-negative-even-integers

[@stdlib/math/iter/sequences/negative-integers]: https://github.com/stdlib-js/math-iter-sequences-negative-integers

[@stdlib/math/iter/sequences/negative-odd-integers]: https://github.com/stdlib-js/math-iter-sequences-negative-odd-integers

[@stdlib/math/iter/sequences/nonfibonacci]: https://github.com/stdlib-js/math-iter-sequences-nonfibonacci

[@stdlib/math/iter/sequences/nonnegative-even-integers]: https://github.com/stdlib-js/math-iter-sequences-nonnegative-even-integers

[@stdlib/math/iter/sequences/nonnegative-integers]: https://github.com/stdlib-js/math-iter-sequences-nonnegative-integers

[@stdlib/math/iter/sequences/nonpositive-even-integers]: https://github.com/stdlib-js/math-iter-sequences-nonpositive-even-integers

[@stdlib/math/iter/sequences/nonpositive-integers]: https://github.com/stdlib-js/math-iter-sequences-nonpositive-integers

[@stdlib/math/iter/sequences/nonsquares]: https://github.com/stdlib-js/math-iter-sequences-nonsquares

[@stdlib/math/iter/sequences/odd-integers]: https://github.com/stdlib-js/math-iter-sequences-odd-integers

[@stdlib/math/iter/sequences/positive-even-integers]: https://github.com/stdlib-js/math-iter-sequences-positive-even-integers

[@stdlib/math/iter/sequences/positive-integers]: https://github.com/stdlib-js/math-iter-sequences-positive-integers

[@stdlib/math/iter/sequences/positive-odd-integers]: https://github.com/stdlib-js/math-iter-sequences-positive-odd-integers

[@stdlib/math/iter/sequences/primes]: https://github.com/stdlib-js/math-iter-sequences-primes

[@stdlib/math/iter/sequences/squared-triangular]: https://github.com/stdlib-js/math-iter-sequences-squared-triangular

[@stdlib/math/iter/sequences/squares]: https://github.com/stdlib-js/math-iter-sequences-squares

[@stdlib/math/iter/sequences/triangular]: https://github.com/stdlib-js/math-iter-sequences-triangular

<!-- </toc-links> -->

</section>

<!-- /.links -->
