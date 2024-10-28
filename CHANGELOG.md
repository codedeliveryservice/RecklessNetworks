# Changelog

All notable changes to the project will be documented in this file.

## [Reckless NNUE v5] - 2024-10-16

### Changes

-   Regenerate the training data with the latest version of the engine
-   Remove output buckets
-   Architecture: `(768 -> 384)x2 -> 1`

### Benchmark

```
Elo   | 13.66 +- 7.33 (95%)
SPRT  | N=25000 Threads=1 Hash=32MB
LLR   | 3.01 (-2.25, 2.89) [0.00, 5.00]
Games | N: 4352 W: 1420 L: 1249 D: 1683
Penta | [129, 461, 860, 562, 164]
```

```
Elo   | 13.93 +- 6.73 (95%)
SPRT  | 20.0+0.20s Threads=1 Hash=64MB
LLR   | 2.89 (-2.25, 2.89) [0.00, 5.00]
Games | N: 3070 W: 827 L: 704 D: 1539
Penta | [21, 316, 740, 435, 23]
```

## [Reckless NNUE v4] - 2024-08-11

### Changes

-   Align parameters
-   Implement output buckets
-   Architecture: `(768 -> 384)x2 -> 1x4`

### Benchmark

```
Elo   | 3.03 +- 2.46 (95%)
SPRT  | 8.0+0.08s Threads=1 Hash=32MB
LLR   | 2.91 (-2.25, 2.89) [0.00, 5.00]
Games | N: 27152 W: 7242 L: 7005 D: 12905
Penta | [366, 3190, 6281, 3319, 420]
```

```
Elo   | 6.91 +- 4.56 (95%)
SPRT  | 20.0+0.20s Threads=1 Hash=128MB
LLR   | 2.90 (-2.25, 2.89) [0.00, 5.00]
Games | N: 7296 W: 1939 L: 1794 D: 3563
Penta | [59, 852, 1714, 931, 92]
```

## [Reckless NNUE v3] - 2024-06-30

### Changes

-   Increase the hidden layer size to 384
-   Architecture: `(768 -> 384)x2 -> 1`

### Benchmark

```
Elo   | 38.04 +- 13.14 (95%)
SPRT  | N=25000 Threads=1 Hash=32MB
LLR   | 3.06 (-2.25, 2.89) [0.00, 5.00]
Games | N: 1568 W: 614 L: 443 D: 511
Penta | [44, 141, 302, 194, 103]
```

```
Elo   | 21.06 +- 8.95 (95%)
SPRT  | 8.0+0.08s Threads=1 Hash=32MB
LLR   | 2.90 (-2.25, 2.89) [0.00, 5.00]
Games | N: 2246 W: 678 L: 542 D: 1026
Penta | [29, 232, 488, 322, 52]
```

## [Reckless NNUE v2] - 2024-04-24

### Changes

-   Increase the hidden layer size to 256
-   Architecture: `(768 -> 256)x2 -> 1`

### Benchmark

```
Elo   | 102.67 +- 23.28 (95%)
SPRT  | N=25000 Threads=1 Hash=32MB
LLR   | 3.07 (-2.25, 2.89) [0.00, 5.00]
Games | N: 672 W: 338 L: 145 D: 189
Penta | [16, 28, 111, 109, 72]
```

```
Elo   | 81.25 +- 20.46 (95%)
SPRT  | 8.0+0.08s Threads=1 Hash=32MB
LLR   | 2.92 (-2.25, 2.89) [0.00, 5.00]
Games | N: 640 W: 252 L: 105 D: 283
Penta | [2, 40, 128, 109, 41]
```

## [Reckless NNUE v1] - 2024-04-16

### Initial release

-   Baseline network model for Reckless
-   Architecture: `(768 -> 128)x2 -> 1`
