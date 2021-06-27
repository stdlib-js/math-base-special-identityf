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

# Identity Function

[![NPM version][npm-image]][npm-url] [![Build Status][test-image]][test-url] [![Coverage Status][coverage-image]][coverage-url] [![dependencies][dependencies-image]][dependencies-url]

> Evaluate the [identity function][identity-function] of a single-precision floating-point number.

<section class="intro">

The [identity-function][identity-function] is defined as

<!-- <equation class="equation" label="eq:identity_function" align="center" raw="f(x) = x" alt="Identity function"> -->

<div class="equation" align="center" data-raw-text="f(x) = x" data-equation="eq:identity_function">
    <img src="https://cdn.rawgit.com/stdlib-js/stdlib/ad4524117c3cf89854aeb12d7210102220874d31/lib/node_modules/@stdlib/math/base/special/identityf/docs/img/equation_identity_function.svg" alt="Identity function">
    <br>
</div>

<!-- </equation> -->

for all `x`.

</section>

<!-- /.intro -->

<section class="installation">

## Installation

```bash
npm install @stdlib/math-base-special-identityf
```

</section>

<section class="usage">

## Usage

```javascript
var identityf = require( '@stdlib/math-base-special-identityf' );
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

```javascript
var randu = require( '@stdlib/random-base-randu' );
var round = require( '@stdlib/math-base-special-round' );
var identityf = require( '@stdlib/math-base-special-identityf' );

var rand;
var i;

for ( i = 0; i < 100; i++ ) {
    rand = round( randu() * 100.0 ) - 50.0;
    console.log( 'identity(%d) = %d', rand, identityf( rand ) );
}
```

</section>

<!-- /.examples -->

<!-- C interface documentation. -->

* * *

<section class="c">

## C APIs

<!-- Section to include introductory text. Make sure to keep an empty line after the intro `section` element and another before the `/section` close. -->

<section class="intro">

</section>

<!-- /.intro -->

<!-- C usage documentation. -->

<section class="installation">

## Installation

```bash
npm install @stdlib/math-base-special-identityf
```

</section>

<section class="usage">

### Usage

```c
#include "stdlib/math/base/special/identityf.h"
```

#### stdlib_base_identityf( x )

Evaluates the identity function for a single-precision floating-point number.

```c
float y = stdlib_base_identityf( 2.0f );
// returns 2.0f
```

The function accepts the following arguments:

-   **x**: `[in] float` input value.

```c
float stdlib_base_identityf( const float x );
```

</section>

<!-- /.usage -->

<!-- C API usage notes. Make sure to keep an empty line after the `section` element and another before the `/section` close. -->

<section class="notes">

</section>

<!-- /.notes -->

<!-- C API usage examples. -->

<section class="examples">

### Examples

```c
#include "stdlib/math/base/special/identityf.h"
#include <stdio.h>

int main() {
    float x[] = { 3.14f, -3.14f, 0.0f, 0.0f/0.0f };

    float y;
    int i;
    for ( i = 0; i < 4; i++ ) {
        y = stdlib_base_identityf( x[ i ] );
        printf( "f(%f) = %f\n", x[ i ], y );
    }
}
```

</section>

<!-- /.examples -->

</section>

<!-- /.c -->


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

Copyright &copy; 2016-2021. The Stdlib [Authors][stdlib-authors].

</section>

<!-- /.stdlib -->

<!-- Section for all links. Make sure to keep an empty line after the `section` element and another before the `/section` close. -->

<section class="links">

[npm-image]: http://img.shields.io/npm/v/@stdlib/math-base-special-identityf.svg
[npm-url]: https://npmjs.org/package/@stdlib/math-base-special-identityf

[test-image]: https://github.com/stdlib-js/math-base-special-identityf/actions/workflows/test.yml/badge.svg
[test-url]: https://github.com/stdlib-js/math-base-special-identityf/actions/workflows/test.yml

[coverage-image]: https://img.shields.io/codecov/c/github/stdlib-js/math-base-special-identityf/main.svg
[coverage-url]: https://codecov.io/github/stdlib-js/math-base-special-identityf?branch=main

[dependencies-image]: https://img.shields.io/david/stdlib-js/math-base-special-identityf.svg
[dependencies-url]: https://david-dm.org/stdlib-js/math-base-special-identityf/main

[chat-image]: https://img.shields.io/gitter/room/stdlib-js/stdlib.svg
[chat-url]: https://gitter.im/stdlib-js/stdlib/

[stdlib]: https://github.com/stdlib-js/stdlib

[stdlib-authors]: https://github.com/stdlib-js/stdlib/graphs/contributors

[stdlib-license]: https://raw.githubusercontent.com/stdlib-js/math-base-special-identityf/main/LICENSE

[identity-function]: https://en.wikipedia.org/wiki/Identity_function

</section>

<!-- /.links -->
