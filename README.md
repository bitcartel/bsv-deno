# bsv

This is the Bitcoin SV Deno library to help developers write Bitcoin SV apps.  Currently this is a wrapper around the [Bitcoin SV javascript library](https://github.com/moneybutton/bsv) so that you can port existing javscript code and apps to Deno.

The goal is to build a friendly Deno / Typescript library, making it easy for developers to write stable and performant Bitcoin SV apps.  Current roadmap includes migrating code and tests to the Deno standard library, evaluating and replacing components where it makes sense with existing best-in-class modules e.g. crypto, wasm, audited.

This project is experimental and unstable -- use at your own risk!  

## Import

```ts
import { bsv } from 'https://deno.land/x/bsv/mod.ts'
```

## Usage

```ts
import { bsv } from 'https://deno.land/x/bsv/mod.ts';
import { Buffer } from 'https://cdn.pika.dev/buffer';

var str = "this is my string"
var base58 = bsv.encoding.Base58.fromBuffer(Buffer.from(str)).toString()
console.log(base58)
```

## Issues

For any bug reports or feature requests, please create an issue on [GitHub](https://github.com/bitcartel/bsv-deno/issues).

## License

MIT