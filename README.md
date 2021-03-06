# Difference Lists in Haskell

The `NonEmpty` version of difference lists: list-like type supporting O(1) append ans snoc operations.

This is a fork of a [`dlist`](http://hackage.haskell.org/package/dlist) package.

```
benchmarking append 1000/List
time                 27.66 ms   (27.30 ms .. 28.01 ms)
                     0.999 R²   (0.999 R² .. 1.000 R²)
mean                 28.39 ms   (28.21 ms .. 28.58 ms)
std dev              391.5 μs   (311.7 μs .. 510.3 μs)

benchmarking append 1000/NonEmpty
time                 33.67 ms   (33.01 ms .. 34.27 ms)
                     0.999 R²   (0.999 R² .. 1.000 R²)
mean                 34.07 ms   (33.90 ms .. 34.29 ms)
std dev              419.3 μs   (308.9 μs .. 549.3 μs)

benchmarking append 1000/DList
time                 57.46 μs   (56.95 μs .. 58.12 μs)
                     0.999 R²   (0.998 R² .. 0.999 R²)
mean                 57.98 μs   (57.61 μs .. 58.41 μs)
std dev              1.398 μs   (1.115 μs .. 1.871 μs)
variance introduced by outliers: 22% (moderately inflated)

benchmarking append 1000/NonEmptyDList
time                 90.37 μs   (89.09 μs .. 91.44 μs)
                     0.999 R²   (0.998 R² .. 0.999 R²)
mean                 89.31 μs   (88.61 μs .. 89.96 μs)
std dev              2.244 μs   (1.763 μs .. 2.988 μs)
variance introduced by outliers: 22% (moderately inflated)
```
