# False sharing

↑ **Parent:** [Cache coherence](cache-coherence.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/False_sharing)

Independent data in the same [cache line](cache-line.md) cause unnecessary ownership transfers or invalidations when different [CPU cores](cpu-core.md) access them. A frequently written lock beside stable reader data can invalidate those data despite no logical conflict.

## ↑ Ancestors (5)

1. [Cache coherence](cache-coherence.md)
2. [Cache (computing)](cache-computing.md)
3. [Computer memory](computer-memory-split.md)
4. [Computer science](computer-science-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-computer-science-course-of-the-university-of-oxford/2015/computer-architecture/3/c/i/solution.md)
