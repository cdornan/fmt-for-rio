# fmt-for-rio

To use this package (with
  [`rio`](https://hackage.haskell.org/package/enum-text-rio-1.0.0.0)):
```haskell
import Fmt
```

This package is just a repackaging of
[`enum-text-rio`](https://hackage.haskell.org/package/enum-text-rio) for
repackaging [`fmt`](https://hackage.haskell.org/package/fmt) to work
with the [`rio`](https://hackage.haskell.org/package/rio) prelude, relocating
the `fmt` modules to their standard locations:

  * `Text.Enum.RIO.Fmt` &rarr; `Fmt`
  * `Text.Enum.RIO.Fmt.Time` &rarr; `Fmt.Time`
  * `Text.Enum.RIO.Fmt.Internal` &rarr; `Fmt.Internal`

Note that this package cannot be combined with the `fmt` package because of the
module clash. If you need access to the original `fmt` you will have to use
`enum-text-rio` instead.

Please see the documentation for
[`fmt`](https://hackage.haskell.org/package/fmt) and
[`enum-text-rio`](https://hackage.haskell.org/package/enum-text-rio)
for details.
