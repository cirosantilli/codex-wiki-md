# Memoization cache contract

↑ **Parent:** [Memoization](memoization.md)

For a terminating [pure function](pure-function.md), a reusable entry must record its correct completed result, and equal [memoization keys](memoization-key.md) must imply equal results throughout the entry's [memoization cache lifetime](memoization-cache-lifetime.md). Reusing that result must also preserve the behavior callers require. These conditions separate correctness from speed: a complete key can be correct even if it rarely repeats.

A procedure using [deterministic computation](deterministic-computation.md) can still have a required [side effect](side-effect-computer-science.md). If a procedure returns $n^2$ and appends an audit record on every call, serving the second call from a table preserves the numerical answer but skips the second record. Likewise, if each call promises a fresh [mutable list](mutable-list.md), returning the same stored [mutable list](mutable-list.md) changes observable sharing and allows a caller to damage later answers. Plain result reuse is unsuitable for those contracts.[Python documentation, functools.lru\_cache: paragraph warning against functions with side effects, distinct mutable results, or impure time/random results](python-3-14-documentation/functools-higher-order-functions-and-operations-on-callable-objects-python-3-14-documentation.md)

Completion matters for [recursion](recursion-computer-science.md). Suppose computing key $A$ needs key $B$, and computing $B$ needs $A$. A table containing only completed answers has no answer to return for the second $A$; remembering completed values does not make this [directed cycle](directed-cycle.md) terminate. Marking a key `ACTIVE` before descending detects re-entry, as in [spreadsheet dependency evaluation](spreadsheet-dependency-evaluation.md), but detection is not a solution of the circular equations. If computation fails, clear its active mark and do not publish an unfinished value. The example using [Fibonacci numbers](fibonacci-number.md) avoids this issue through a strictly decreasing argument.

The call counts above assume sequential execution and no eviction. Concurrent requests for an absent key can both begin evaluation before either publishes its result; keeping a table coherent alone does not ensure one body execution per key.[Python documentation, functools.cache and functools.lru\_cache: thread-safe cache updates can still allow repeated evaluation before completion](python-3-14-documentation/functools-higher-order-functions-and-operations-on-callable-objects-python-3-14-documentation.md)

**Table of contents**

- [Memoization key](memoization-key.md)
- [Memoization cache lifetime](memoization-cache-lifetime.md)

## ↑ Ancestors (4)

1. [Memoization](memoization.md)
2. [Algorithm](algorithm.md)
3. [Computer science](computer-science-split.md)
4. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Memoization](memoization.md)
- [Pure function](pure-function.md)
