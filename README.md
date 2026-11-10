# OxideTerm media

Public screenshots and benchmark charts for [OxideTerm](https://github.com/AnalyseDeCircuit/oxideterm), used in its README, website and announcement posts.

## Benchmark charts

- [Terminal throughput comparison](https://analysedecircuit.github.io/oxideterm-media/benchmarks/2.3.1/throughput.png)
- [Terminal history memory comparison](https://analysedecircuit.github.io/oxideterm-media/benchmarks/2.3.1/history-memory.png)

The throughput chart compares an early release-build baseline with a 2.3.1 run. Both use 16 MiB per workload, one warm-up and the median of three measured runs. The early record does not identify an exact application version, and the historical summaries do not preserve complete matched machine and window settings. This measures process-to-PTY output throughput, excluding final rendering, input latency and SSH network transfer. The early baseline is documented in the [2.0.23 release notes](https://github.com/AnalyseDeCircuit/oxideterm/blob/f6776c83656a3fe5108ee8bae6a67577e87e53d0/.github/release-notes/stable-changelog.md#2023); the [benchmark guide](https://github.com/AnalyseDeCircuit/oxideterm/blob/v2.3.1/benchmark/README.md) describes the harness.

The memory chart shows the cumulative change across consecutive October 26 storage stages, using 20,000 history rows at 400 columns plus 40 screen rows. It counts retained requested heap allocations owned by the terminal and parser, excluding the desktop UI, GPU, prebuilt input and allocator overhead. See the [measurement records](https://github.com/AnalyseDeCircuit/oxideterm/blob/v2.3.1/docs/development/performance-and-benchmarking.md#text-run-history-and-sequential-reads-2026-10-26).

## Screenshots

- Terminal workspace and Docker tools: [framed PNG](https://analysedecircuit.github.io/oxideterm-media/screenshots/2.3.1/workspace-docker-framed.png) · [transparent original](https://analysedecircuit.github.io/oxideterm-media/screenshots/2.3.1/workspace-docker.png)
- Mixed four-pane workspace: [framed PNG](https://analysedecircuit.github.io/oxideterm-media/screenshots/2.3.1/mixed-workspace-framed.png) · [transparent original](https://analysedecircuit.github.io/oxideterm-media/screenshots/2.3.1/mixed-workspace.png)

Screenshot account names, hosts, addresses, paths, file entries and monitoring values have been replaced with demonstration data. PNG screenshots retain transparent window corners without an outer black matte.

Framed versions add a dark gradient background and soft shadow for articles with a light background. Screenshot contents and resolution are preserved; transparent originals remain available at their published paths.

## Asset conventions

- Upload only final, sanitized assets. Keep original captures, credentials and temporary processing files outside this repository.
- Group assets by type and application version.
- Keep published paths unchanged. Use a new filename or version directory for revisions.
- Keep large videos outside Git history.

GitHub Pages serves the files directly from the root of `main`; no application build is required.
