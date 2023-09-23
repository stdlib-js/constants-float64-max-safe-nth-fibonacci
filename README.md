<!--

@license Apache-2.0

Copyright (c) 2018 The Stdlib Authors.

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

# FLOAT64_MAX_SAFE_NTH_FIBONACCI

[![NPM version][npm-image]][npm-url] [![Build Status][test-image]][test-url] [![Coverage Status][coverage-image]][coverage-url] <!-- [![dependencies][dependencies-image]][dependencies-url] -->

> Maximum safe nth [Fibonacci number][fibonacci-number] when stored in [double-precision floating-point][ieee754] format.



<section class="usage">

## Usage

<!-- eslint-disable id-length -->

```javascript
import FLOAT64_MAX_SAFE_NTH_FIBONACCI from 'https://cdn.jsdelivr.net/gh/stdlib-js/constants-float64-max-safe-nth-fibonacci@esm/index.mjs';
```
The previous example will load the latest bundled code from the esm branch. Alternatively, you may load a specific version by loading the file from one of the [tagged bundles](https://github.com/stdlib-js/constants-float64-max-safe-nth-fibonacci/tags). For example,

```javascript
import FLOAT64_MAX_SAFE_NTH_FIBONACCI from 'https://cdn.jsdelivr.net/gh/stdlib-js/constants-float64-max-safe-nth-fibonacci@v0.1.0-esm/index.mjs';
```

#### FLOAT64_MAX_SAFE_NTH_FIBONACCI

The maximum [safe][safe-integers] nth [Fibonacci number][fibonacci-number] when stored in [double-precision floating-point][ieee754] format.

<!-- eslint-disable id-length -->

```javascript
var bool = ( FLOAT64_MAX_SAFE_NTH_FIBONACCI === 78 );
// returns true
```

</section>

<!-- /.usage -->

<section class="examples">

## Examples

<!-- eslint-disable id-length -->

<!-- eslint no-undef: "error" -->

```html
<!DOCTYPE html>
<html lang="en">
<body>
<script type="module">

import FLOAT64_MAX_SAFE_NTH_FIBONACCI from 'https://cdn.jsdelivr.net/gh/stdlib-js/constants-float64-max-safe-nth-fibonacci@esm/index.mjs';

var v;
var i;

function fibonacci( n ) {
    var a;
    var b;
    var c;
    var i;

    a = 1;
    b = 1;
    for ( i = 3; i <= n; i++ ) {
        c = a + b;
        a = b;
        b = c;
    }
    return b;
}

for ( i = 0; i < 100; i++ ) {
    v = fibonacci( i );
    if ( i > FLOAT64_MAX_SAFE_NTH_FIBONACCI ) {
        console.log( 'Unsafe: %d', v );
    } else {
        console.log( 'Safe:   %d', v );
    }
}

</script>
</body>
</html>
```

</section>

<!-- /.examples -->

<!-- C interface documentation. -->



<!-- Section for related `stdlib` packages. Do not manually edit this section, as it is automatically populated. -->

<section class="related">

* * *

## See Also

-   <span class="package-name">[`@stdlib/constants-float64/max-safe-fibonacci`][@stdlib/constants/float64/max-safe-fibonacci]</span><span class="delimiter">: </span><span class="description">maximum safe Fibonacci number when stored in double-precision floating-point format.</span>

</section>

<!-- /.related -->

<!-- Section for all links. Make sure to keep an empty line after the `section` element and another before the `/section` close. -->


<section class="main-repo" >

* * *

## Notice

This package is part of [stdlib][stdlib], a standard library with an emphasis on numerical and scientific computing. The library provides a collection of robust, high performance libraries for mathematics, statistics, streams, utilities, and more.

For more information on the project, filing bug reports and feature requests, and guidance on how to develop [stdlib][stdlib], see the main project [repository][stdlib].

#### Community

[![Chat][chat-image]][chat-url]

---

## License

See [LICENSE][stdlib-license].


## Copyright

Copyright &copy; 2016-2023. The Stdlib [Authors][stdlib-authors].

</section>

<!-- /.stdlib -->

<!-- Section for all links. Make sure to keep an empty line after the `section` element and another before the `/section` close. -->

<section class="links">

[npm-image]: http://img.shields.io/npm/v/@stdlib/constants-float64-max-safe-nth-fibonacci.svg
[npm-url]: https://npmjs.org/package/@stdlib/constants-float64-max-safe-nth-fibonacci

[test-image]: https://github.com/stdlib-js/constants-float64-max-safe-nth-fibonacci/actions/workflows/test.yml/badge.svg?branch=v0.1.0
[test-url]: https://github.com/stdlib-js/constants-float64-max-safe-nth-fibonacci/actions/workflows/test.yml?query=branch:v0.1.0

[coverage-image]: https://img.shields.io/codecov/c/github/stdlib-js/constants-float64-max-safe-nth-fibonacci/main.svg
[coverage-url]: https://codecov.io/github/stdlib-js/constants-float64-max-safe-nth-fibonacci?branch=main

<!--

[dependencies-image]: https://img.shields.io/david/stdlib-js/constants-float64-max-safe-nth-fibonacci.svg
[dependencies-url]: https://david-dm.org/stdlib-js/constants-float64-max-safe-nth-fibonacci/main

-->

[chat-image]: https://img.shields.io/gitter/room/stdlib-js/stdlib.svg
[chat-url]: https://app.gitter.im/#/room/#stdlib-js_stdlib:gitter.im

[stdlib]: https://github.com/stdlib-js/stdlib

[stdlib-authors]: https://github.com/stdlib-js/stdlib/graphs/contributors

[umd]: https://github.com/umdjs/umd
[es-module]: https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Modules

[deno-url]: https://github.com/stdlib-js/constants-float64-max-safe-nth-fibonacci/tree/deno
[umd-url]: https://github.com/stdlib-js/constants-float64-max-safe-nth-fibonacci/tree/umd
[esm-url]: https://github.com/stdlib-js/constants-float64-max-safe-nth-fibonacci/tree/esm
[branches-url]: https://github.com/stdlib-js/constants-float64-max-safe-nth-fibonacci/blob/main/branches.md

[stdlib-license]: https://raw.githubusercontent.com/stdlib-js/constants-float64-max-safe-nth-fibonacci/main/LICENSE

[safe-integers]: http://www.2ality.com/2013/10/safe-integers.html

[fibonacci-number]: https://en.wikipedia.org/wiki/Fibonacci_number

[ieee754]: https://en.wikipedia.org/wiki/IEEE_754-1985

<!-- <related-links> -->

[@stdlib/constants/float64/max-safe-fibonacci]: https://github.com/stdlib-js/constants-float64-max-safe-fibonacci/tree/esm

<!-- </related-links> -->

</section>

<!-- /.links -->
