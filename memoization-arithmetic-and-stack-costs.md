# Memoization arithmetic and stack costs

↑ **Parent:** [Memoization](memoization.md)

Under constant-cost lookup and [integer](integer-split.md) [addition](addition.md), [Memoized Fibonacci evaluation](memoized-fibonacci-evaluation.md) has [time complexity](time-complexity.md) $O(n)$ in [Big O notation](big-o-notation.md), retaining $O(n)$ values. A [hash table](hash-table.md) needs its own lookup-cost assumptions; an [array](array-data-structure.md) indexed by $0,\ldots,n$ avoids [hash collisions](hash-collision.md) in this example. [Memoization](memoization.md) removes repeated bodies, but also pays for keys, lookups and retained answers. A workload without reuse can pay those costs without saving evaluations.

The [call stack](call-stack.md) remains. Left-first [recursion](recursion-computer-science.md) descends through arguments $n,n-1,\ldots,1$ before returning, giving $n$ simultaneously active frames for $n\geq2$. Therefore the auxiliary [space complexity](space-complexity.md) includes $O(n)$ frames as well as $O(n)$ table entries in the constant-size-value model. An iterative bottom-up [dynamic programming](dynamic-programming.md) calculation removes these recursive frames; retaining only the two previous [Fibonacci numbers](fibonacci-number.md) suffices when only the final value is wanted, but discards the table useful for later requests.

Exact [Fibonacci numbers](fibonacci-number.md) do not remain constant-size values. For $k\geq2$, the [recurrence relation](recurrence-relation.md) gives $2^{(k-2)/2}\leq F_k\leq2^{k-1}$, so the representation of $F_k$ as a [binary number](binary-number.md) has order $k$ [bits](bit.md). With ordinary [addition](addition.md) costing order $k$ [bit](bit.md) operations on such operands, the $n-1$ [additions](addition.md) cost order $n^2$ [bit](bit.md) operations in total. Retaining all values also requires order $n^2$ [bits](bit.md) of value storage, before keys and frame overhead. The linear bound counts [additions](addition.md) under its stated cost model; it is not a linear bound on exact [integer arithmetic](integer-arithmetic.md) in [bits](bit.md).[MIT 6.006 Spring 2020, Lecture 15: Recursive Algorithms, printed p. 3, final three bullets: growing Fibonacci bit lengths and addition cost](lecture-15-recursive-algorithms-6-006-spring-2020-by-massachusetts-institute-of-technology-6-006-course-staff.md)

## ↑ Ancestors (4)

1. [Memoization](memoization.md)
2. [Algorithm](algorithm-split.md)
3. [Computer science](computer-science-split.md)
4. [Codex Wiki](split.md)
