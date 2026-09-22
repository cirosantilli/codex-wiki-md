# Memoization cache lifetime

↑ **Parent:** [Memoization cache contract](memoization-cache-contract.md)

A [memoization cache lifetime](memoization-cache-lifetime.md) is the interval over which retained entries are available and valid. One table per top-level request shares recursive subproblems within that request; keeping a table between requests also allows the warm $F_5$ and incremental $F_6$ examples. Clearing it loses those savings. Evicting a correct answer can preserve correctness for a terminating [pure function](pure-function.md), while forcing recomputation; changing an input without invalidating an obsolete answer can break correctness.

Specify who owns the table, when context changes invalidate it, and how long keys and results occupy [computer memory](computer-memory.md). In a concrete implementation, retained references can keep arguments and answers alive until removal or clearing.[Python documentation, functools.lru\_cache: cache\_clear and retention of argument and return-value references until eviction or clearing](python-3-14-documentation/functools-higher-order-functions-and-operations-on-callable-objects-python-3-14-documentation.md) The [memoization](memoization.md) promise is conditional reuse of valid completed answers, not an automatic guarantee of freshness, termination or bounded [computer memory](computer-memory.md).

// Target: computer-science.bigb

## ↑ Ancestors (5)

1. [Memoization cache contract](memoization-cache-contract.md)
2. [Memoization](memoization.md)
3. [Algorithm](algorithm-split.md)
4. [Computer science](computer-science-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (4)

- [Memoization](memoization.md)
- [Memoization cache contract](memoization-cache-contract.md)
- [Memoization cache lifetime](memoization-cache-lifetime.md)
- [Memoization key](memoization-key.md)
