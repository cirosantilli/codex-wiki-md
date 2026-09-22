# Cache (computing)

↑ **Parent:** [Computer memory](computer-memory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Cache_(computing))

A store of selected information kept for faster reuse. A [translation lookaside buffer](translation-lookaside-buffer.md) is a [memory cache](cache-computing.md) of [address translations](address-translation.md); a [buffer cache](buffer-cache.md) instead holds device-block contents.

For a data [memory cache](cache-computing.md), the useful bargain is to keep a small selection of [computer memory](computer-memory.md) close to the [CPU](central-processing-unit.md). A [cache hit](cache-hit.md) serves a read from that selection; a [cache miss](cache-miss.md) requires obtaining the contents elsewhere. [Temporal locality](temporal-locality.md) helps a retained [cache block](cache-line.md) serve repeated reads, and [spatial locality](spatial-locality.md) helps one transferred [cache line](cache-line.md) serve neighbouring [bytes](byte.md). Placement, capacity and [LRU replacement](lru-replacement.md) determine whether that opportunity survives until the next read. [11.4. CPU Caches](dive-into-systems-by-suzanne-j-matthews-and-others/11-4-cpu-caches.md)

The worked [memory access trace](memory-access-trace.md) below uses twelve single-[byte](byte.md) reads at these decimal [physical addresses](physical-address.md), in this fixed order:

$$
0,4,32,0,16,32,4,48,52,0,16,0.
$$

Assume an initially empty [fully associative cache](fully-associative-cache.md), 16-[byte](byte.md) aligned [cache blocks](cache-line.md), and capacity two [cache slots](cache-slot.md): 32 [bytes](byte.md) of cached data, excluding metadata. Use exact [LRU replacement](lru-replacement.md), refreshing recency on every read, including [cache hits](cache-hit.md). Every [cache miss](cache-miss.md) fetches its requested [cache line](cache-line.md) completely before the next read; only a full [memory cache](cache-computing.md) needs an eviction. There are no writes, fetching ahead of requests, external invalidations, or overlapping reads. All addresses denote ordinary cacheable [computer memory](computer-memory.md), and [address translation](address-translation.md) is outside this model. These are deliberately synthetic assumptions, not specifications of a particular [CPU](central-processing-unit.md).

This makes the outcome reproducible from the [memory access trace](memory-access-trace.md), rather than from an informal impression that data are “nearby” or “recent”. The [cache line](cache-line.md) geometry below identifies the requested unit; [fully associative cache](fully-associative-cache.md) enumerates the resulting states; [average memory access time](average-memory-access-time.md) translates the counts into a simple timing calculation.

**Table of contents**

- [Cache line](cache-line.md)
  - [Cache slot](cache-slot.md)
    - [Cache tag](cache-tag.md)
- [Cache hit](cache-hit.md)
  - [Cache hit rate](cache-hit-rate.md)
- [Cache miss](cache-miss.md)
  - [Cache miss rate](cache-miss-rate.md)
  - [Capacity miss](capacity-miss.md)
  - [Conflict miss](conflict-miss.md)
  - [Cache miss penalty](cache-miss-penalty.md)
  - [Compulsory miss](compulsory-miss.md)
- [Fully associative cache](fully-associative-cache.md)
- [Direct-mapped cache](direct-mapped-cache.md)
- [Memory access latency](memory-access-latency.md)
  - [Average memory access time](average-memory-access-time.md)

## ↑ Ancestors (3)

1. [Computer memory](computer-memory.md)
2. [Computer science](computer-science-split.md)
3. [Codex Wiki](split.md)
