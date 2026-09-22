# Memoization key

↑ **Parent:** [Memoization cache contract](memoization-cache-contract.md)

A [memoization key](memoization-key.md) identifies all information that determines a reusable answer. Write $x$ for explicit arguments and $c$ for relevant context. For a [function](function-split.md) $f$ and key [function](function-split.md) $K$, the necessary value condition is

$$
K(x,c)=K(y,d)\ \Longrightarrow\ f(x,c)=f(y,d).
$$

This implication need hold only for contexts in which the entry can be reused. The condition concerns [key equality](key-equality.md), not merely equality of [hash function](hash-function.md) outputs: a [hash table](hash-table.md) must resolve [hash collisions](hash-collision.md) by comparing complete keys. Include the identity or version of the procedure if one table stores results for several procedures or changing implementations.

For an original toy example, let $g(n,a)=an$. Caching only by $n$ after $g(3,2)=6$ incorrectly returns $6$ for $g(3,4)$, whose answer is $12$. The pair $(n,a)$ is complete for this [function](function-split.md). If $a$ is hidden in mutable configuration, either freeze that configuration for the [memoization cache lifetime](memoization-cache-lifetime.md), include a reliable version in the key, or invalidate affected entries before reuse. A version is sufficient only if every relevant change updates it. Object identity alone is likewise insufficient for a [mutable list](mutable-list.md) whose contents determine the answer.

## ↑ Ancestors (5)

1. [Memoization cache contract](memoization-cache-contract.md)
2. [Memoization](memoization.md)
3. [Algorithm](algorithm.md)
4. [Computer science](computer-science-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (4)

- [Memoization](memoization.md)
- [Memoization cache contract](memoization-cache-contract.md)
- [Memoization key](memoization-key.md)
- [Overlapping subproblems](overlapping-subproblems.md)
