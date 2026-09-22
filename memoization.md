# Memoization

↑ **Parent:** [Algorithm](algorithm-split.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Memoization)

[Memoization](memoization.md) retains a completed [function](function-split.md) result under a [memoization key](memoization-key.md) and returns that result when an equivalent request recurs. For a terminating [pure function](pure-function.md), repeated evaluation can therefore become lookup rather than repeated work. The benefit is especially striking with [recursion](recursion-computer-science.md) and [overlapping subproblems](overlapping-subproblems.md): a large [tree](tree-graph-theory-split.md) of calls can refer to a small [Directed acyclic graph](directed-acyclic-graph.md) of distinct answers. The [memoization cache contract](memoization-cache-contract.md) determines whether reuse is correct; the [memoization cache lifetime](memoization-cache-lifetime.md) determines whether an answer is still present when wanted.

[Memoization](memoization.md) records computed answers, whereas a [memory cache](cache-computing.md) retains data from [computer memory](computer-memory.md). A [CPU](central-processing-unit.md) [cache hit](cache-hit.md) does not by itself prevent a program from evaluating the same [function](function-split.md) again. [Spreadsheet dependency evaluation](spreadsheet-dependency-evaluation.md) adds an explicit mechanism for invalidating affected [cached cell values](cached-cell-value.md) after inputs change; a general [memoization](memoization.md) table does not discover such changes automatically.

A documented early motivation was to let programs improve their efficiency during execution through rote learning: the abstract of a 1968 paper explicitly proposes such a [programming language](programming-language-split.md) facility.[Donald Michie, “Memo” Functions and Machine Learning, Nature 218, pp. 19–22 (1968), abstract: programming-language rote learning motivated by efficiency during execution](%E2%80%9Cmemo%E2%80%9D-functions-and-machine-learning-by-donald-michie.md)

**Table of contents**

- [Overlapping subproblems](overlapping-subproblems.md)
- [Memoized Fibonacci evaluation](memoized-fibonacci-evaluation.md)
- [Memoization arithmetic and stack costs](memoization-arithmetic-and-stack-costs.md)
- [Memoization cache contract](memoization-cache-contract.md)
  - [Memoization key](memoization-key.md)
  - [Memoization cache lifetime](memoization-cache-lifetime.md)

## ↑ Ancestors (3)

1. [Algorithm](algorithm-split.md)
2. [Computer science](computer-science-split.md)
3. [Codex Wiki](split.md)

## ← Incoming links (15)

- [Cached cell value](cached-cell-value.md)
- [Collatz sequence](collatz-sequence.md)
- [Du Jiao sieve](du-jiao-sieve.md)
- [Dynamic programming](dynamic-programming.md)
- [Lazy list](lazy-list.md)
- [Matrix-chain dynamic programming](matrix-chain-dynamic-programming.md)
- [Memoization](memoization.md)
- [Memoization arithmetic and stack costs](memoization-arithmetic-and-stack-costs.md)
- [Memoization cache lifetime](memoization-cache-lifetime.md)
- [Memoized Fibonacci evaluation](memoized-fibonacci-evaluation.md)
- [Overlapping subproblems](overlapping-subproblems.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/ia/paper-5/5/a/iii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/ia/paper-5/6/a/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/ia/paper-5/9/b/ii/solution.md)
- [Spreadsheet dependency evaluation](spreadsheet-dependency-evaluation.md)
