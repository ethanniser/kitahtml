# Benchmark

- 2023-09-14T21:20:07.035Z
- Node: v18.15.0
- V8: 10.2.154.26-node.25
- OS: linux
- Arch: x64

## Hello World

| Runs   | @kitajs/html | typed-html | +     | .compile() | + / @kitajs/html | + / typed-html |
| ------ | ------------ | ---------- | ----- | ---------- | ---------------- | -------------- |
| 10     | 0.0094ms     | 0.0164ms   | 1.74x | 0.0038ms   | 2.5x             | 4.34x          |
| 10000  | 1.1723ms     | 2.9252ms   | 2.5x  | 1.278ms    | 0.92x            | 2.29x          |
| 100000 | 8.8428ms     | 20.1493ms  | 2.28x | 2.7031ms   | 3.27x            | 7.45x          |

## Many Props

| Runs   | @kitajs/html | typed-html | +     | .compile() | + / @kitajs/html | + / typed-html |
| ------ | ------------ | ---------- | ----- | ---------- | ---------------- | -------------- |
| 10     | 0.1971ms     | 1.3064ms   | 6.63x | 0.0036ms   | 54.09x           | 358.62x        |
| 10000  | 166.2978ms   | 938.6489ms | 5.64x | 0.9456ms   | 175.87x          | 992.66x        |
| 100000 | 1693.7948ms  | 8952.945ms | 5.29x | 4.292ms    | 394.64x          | 2085.96x       |

## Many Components

| Runs   | @kitajs/html | typed-html  | +     | .compile() | + / @kitajs/html | + / typed-html |
| ------ | ------------ | ----------- | ----- | ---------- | ---------------- | -------------- |
| 10     | 0.2237ms     | 0.7488ms    | 3.35x | 0.0072ms   | 31.14x           | 104.22x        |
| 10000  | 171.0714ms   | 500.6814ms  | 2.93x | 1.449ms    | 118.06x          | 345.53x        |
| 100000 | 1818.6258ms  | 5277.3456ms | 2.9x  | 9.2505ms   | 196.6x           | 570.49x        |

## Big Component

| Runs   | @kitajs/html | typed-html  | +     | .compile() | + / @kitajs/html | + / typed-html |
| ------ | ------------ | ----------- | ----- | ---------- | ---------------- | -------------- |
| 10     | 0.5231ms     | 0.9827ms    | 1.88x | 0.0059ms   | 88.03x           | 165.38x        |
| 10000  | 131.2238ms   | 829.1856ms  | 6.32x | 0.9444ms   | 138.95x          | 878x           |
| 100000 | 1346.2388ms  | 7372.6771ms | 5.48x | 4.6654ms   | 288.56x          | 1580.29x       |
