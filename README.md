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

# Identity Function

[![NPM version][npm-image]][npm-url] [![Build Status][test-image]][test-url] [![Coverage Status][coverage-image]][coverage-url] <!-- [![dependencies][dependencies-image]][dependencies-url] -->

> Evaluate the [identity function][identity-function] of a single-precision floating-point number.

<section class="intro">

The [identity-function][identity-function] is defined as

<!-- <equation class="equation" label="eq:identity_function" align="center" raw="f(x) = x" alt="Identity function"> -->

```math
f(x) = x
```

<!-- <div class="equation" align="center" data-raw-text="f(x) = x" data-equation="eq:identity_function">
    <img src="https://cdn.jsdelivr.net/gh/stdlib-js/stdlib@ad4524117c3cf89854aeb12d7210102220874d31/lib/node_modules/@stdlib/math/base/special/identityf/docs/img/equation_identity_function.svg" alt="Identity function">
    <br>
</div> -->

<!-- </equation> -->

for all `x`.

</section>

<!-- /.intro -->



<section class="usage">

## Usage

```javascript
import identityf from 'https://cdn.jsdelivr.net/gh/stdlib-js/math-base-special-identityf@v0.2.0-esm/index.mjs';
```

#### identityf( x )

Evaluates the [identity function][identity-function] for a single-precision floating-point number.

```javascript
var v = identityf( -1.0 );
// returns -1.0

v = identityf( 2.0 );
// returns 2.0

v = identityf( 0.0 );
// returns 0.0

v = identityf( -0.0 );
// returns -0.0

v = identityf( NaN );
// returns NaN
```

</section>

<!-- /.usage -->

<section class="examples">

## Examples

<!-- eslint no-undef: "error" -->

```html
<!DOCTYPE html>
<html lang="en">
<body>
<script type="module">

import randu from 'https://cdn.jsdelivr.net/gh/stdlib-js/random-base-randu@esm/index.mjs';
import round from 'https://cdn.jsdelivr.net/gh/stdlib-js/math-base-special-round@esm/index.mjs';
import identityf from 'https://cdn.jsdelivr.net/gh/stdlib-js/math-base-special-identityf@v0.2.0-esm/index.mjs';

var rand;
var i;

for ( i = 0; i < 100; i++ ) {
    rand = round( randu() * 100.0 ) - 50.0;
    console.log( 'identity(%d) = %d', rand, identityf( rand ) );
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

-   <span class="package-name">[`@stdlib/math-base/special/identityf`][@stdlib/math/base/special/identityf]</span><span class="delimiter">: </span><span class="description">evaluate the identity function for a single-precision floating-point number.</span>

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

Copyright &copy; 2016-2024. The Stdlib [Authors][stdlib-authors].

</section>

<!-- /.stdlib -->

<!-- Section for all links. Make sure to keep an empty line after the `section` element and another before the `/section` close. -->

<section class="links">

[npm-image]: http://img.shields.io/npm/v/@stdlib/math-base-special-identityf.svg
[npm-url]: https://npmjs.org/package/@stdlib/math-base-special-identityf

[test-image]: https://github.com/stdlib-js/math-base-special-identityf/actions/workflows/test.yml/badge.svg?branch=v0.2.0
[test-url]: https://github.com/stdlib-js/math-base-special-identityf/actions/workflows/test.yml?query=branch:v0.2.0

[coverage-image]: https://img.shields.io/codecov/c/github/stdlib-js/math-base-special-identityf/main.svg
[coverage-url]: https://codecov.io/github/stdlib-js/math-base-special-identityf?branch=main

<!--

[dependencies-image]: https://img.shields.io/david/stdlib-js/math-base-special-identityf.svg
[dependencies-url]: https://david-dm.org/stdlib-js/math-base-special-identityf/main

-->

[chat-image]: https://img.shields.io/gitter/room/stdlib-js/stdlib.svg
[chat-url]: https://app.gitter.im/#/room/#stdlib-js_stdlib:gitter.im

[stdlib]: https://github.com/stdlib-js/stdlib

[stdlib-authors]: https://github.com/stdlib-js/stdlib/graphs/contributors

[umd]: https://github.com/umdjs/umd
[es-module]: https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Modules

[deno-url]: https://github.com/stdlib-js/math-base-special-identityf/tree/deno
[deno-readme]: https://github.com/stdlib-js/math-base-special-identityf/blob/deno/README.md
[umd-url]: https://github.com/stdlib-js/math-base-special-identityf/tree/umd
[umd-readme]: https://github.com/stdlib-js/math-base-special-identityf/blob/umd/README.md
[esm-url]: https://github.com/stdlib-js/math-base-special-identityf/tree/esm
[esm-readme]: https://github.com/stdlib-js/math-base-special-identityf/blob/esm/README.md
[branches-url]: https://github.com/stdlib-js/math-base-special-identityf/blob/main/branches.md

[stdlib-license]: https://raw.githubusercontent.com/stdlib-js/math-base-special-identityf/main/LICENSE

[identity-function]: https://en.wikipedia.org/wiki/Identity_function

<!-- <related-links> -->

[@stdlib/math/base/special/identityf]: https://github.com/stdlib-js/math-base-special-identityf/tree/esm

<!-- </related-links> -->

</section>

<!-- /.links -->
