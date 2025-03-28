# Performance in Warp

## Overview
This document provides a comparison of Warp's performance against other popular terminal emulator applications. The benchmarks focus on various performance metrics to help users understand how Warp stands in terms of speed and efficiency.

## Terminal Apps Selected for Benchmarking
The following terminal emulator applications were chosen for comparison based on their popularity and performance principles:

- **Terminal.app**: The default terminal app available on macOS.
- **iTerm2**: One of the most popular terminal emulators used by macOS users.
- **Alacritty**: A terminal emulator known for its speed and performance, written in Rust.
- **WezTerm**: Another Rust-based terminal known for its performance.

## Versions & Settings Used During the Comparison
| Terminal      | Version                                   | Terminal Size (cols / rows) |
|---------------|-------------------------------------------|------------------------------|
| Warp          | v0.2022.04.01.01.37.stable_03            | 208 cols / 54 rows           |
| Terminal.app  | Version 2.11 (440)                       | 188 cols / 72 rows           |
| iTerm2        | Build 3.4.15                             | 211 cols / 78 rows           |
| Alacritty     | alacritty 0.10.1 (2844606)               | 286 cols / 102 rows          |
| WezTerm       | 20220319-142410-0fcdea07                 | 243 cols / 80 rows           |

## About Benchmarks
The benchmarks are designed to evaluate how each terminal emulator behaves when dealing with significant input and output. The source code for each benchmark used is linked for reproducibility. 

### VTE Benchmark Results
| Test Type                          | Warp avg (ms) | Terminal.app avg (ms) | iTerm avg (ms) | Alacritty avg (ms) | WezTerm avg (ms) |
|------------------------------------|----------------|------------------------|-----------------|---------------------|-------------------|
| dense_cells                        | 43.88          | 24.91                  | 144.84          | 7.25                | 28.15             |
| scrolling                          | 30.06          | 283.34                 | 1257.57         | 31.75               | 687.77            |
| scrolling_bottom_region            | 117.34         | 257.23                 | 1294.25         | 29.1                | 672.67            |
| scrolling_bottom_small_region      | 114.52         | 227.75                 | 1251            | 25.98               | 669.93            |
| scrolling_fullscreen               | 37.4           | 307.03                 | 1565.17         | 37.36               | 1205              |
| scrolling_top_region               | 120.63         | 209.29                 | 2212.2          | 84.42               | 682.6             |
| scrolling_top_small_region         | 114.64         | 205.59                 | 1216.33         | 21.91               | 663.44            |
| unicode                            | 66.47          | 34.45                  | 93.01           | 16.78               | 1279.25           |

### Termbench Results
| Test Type                          | Warp (s)      | Terminal.app (s)      | iTerm (s)      | Alacritty (s)     | WezTerm (s)      |
|------------------------------------|----------------|------------------------|-----------------|---------------------|-------------------|
| ManyLine                           | 6.7854         | 2.6789                 | 8.7057          | 1.2532              | 8.9436            |
| LongLine                           | 9.0033         | 1.6473                 | 9.0849          | 0.8179              | 11.4587           |
| FGPerChar                          | 1.3716         | 453.9888               | 2.6625          | 0.2788              | 0.6487            |
| FGBGPerChar                        | 2.8403         | 908.894                | 4.5881          | 0.5931              | 0.7283            |
| Overall Result                     | 20.0006        | 1367.209               | 25.0413         | 2.943               | 21.7793           |

## Conclusion
The benchmarks indicate that Warp performs competitively against other terminal emulators, particularly in scenarios involving dense input and output. Future benchmarks may include latency measurements to provide a more comprehensive performance overview.

This guide will assist users in understanding the performance capabilities of Warp compared to other terminal applications.
