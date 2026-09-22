# DMA buffer synchronization

↑ **Parent:** [Direct memory access](direct-memory-access.md)

Coordinating [CPU](central-processing-unit.md) and device access to a [DMA buffer](dma-buffer.md), including any required [memory cache](cache-computing.md) maintenance and ordering. A completed device write must be made visible before the [CPU](central-processing-unit.md) consumes it. The [Linux kernel](linux-kernel.md) distinguishes coherent mappings from streaming mappings needing synchronization at ownership changes; even coherent mappings can require ordering of writes. [Linux kernel documentation, Dynamic DMA mapping Guide: types of DMA mappings and using streaming DMA mappings](https://docs.kernel.org/core-api/dma-api-howto.html)[James E. J. Bottomley, Linux DMA API, part Ia: coherent buffers and write ordering](https://docs.kernel.org/core-api/dma-api.html)

## ↑ Ancestors (4)

1. [Direct memory access](direct-memory-access.md)
2. [Computer bus](computer-bus.md)
3. [Computer science](computer-science-split.md)
4. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Direct memory access](direct-memory-access.md)
- [DMA buffer](dma-buffer.md)
