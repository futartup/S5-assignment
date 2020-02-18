# S5-assignment
S5 Assignment



### Trail 2 CNN Architecture

1. Dataset = MNIST

1. Padding = 0
1. Stride = 1
1. Max Pool Stride = 2

1. Best Test Accuracy = 99.45%
1. Best Train Accuracy = 99.50%



| Input | kernel | Output | GRF | Total Parameters | Jout |
| ------ | ------ | ------ | ------ | ------ | ------ |
| 28 * 28 * 1 | 3 * 3 * 1 * 10 | 26 * 26 * 10 | 3 | 90 | 1 |
| 26 * 26 * 10 | 3 * 3 * 10 * 16 | 24 * 24 * 16 | 5 | 1440 | 1 |
| Max Pool |  |  | 6 | 0 | 2 |
| 12 * 12 * 16 | 3 * 3 * 16 * 16 | 10 * 10 * 16 | 10 | 2304 | 2 |
| 10 * 10 * 16 | 3 * 3 * 16 * 16 | 8 * 8 * 16 | 14 | 2304 | 2 |
| 8 * 8 * 16 | 3 * 3 * 16 * 16 | 6 * 6 * 16 | 18 | 2304 | 2 |
| Max Pool |  |  | 22 | 0 | 4 |
| 3 * 3 * 16 | 3 * 3 * 16 * 10 | 1 * 1 * 10 | 30 | 1440 | 4 |
|  | | | | Total Parameters = 10030 |  |
