<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Tie the three scaled streams back to the same shared [lazy list](../../../../../lazy-list.md):

```
hamming :: [Integer]
hamming = 1 : merge (map (2*) hamming)
                    (merge (map (3*) hamming) (map (5*) hamming))
```

The resulting values are precisely the [Hamming numbers](../../../../../5-smooth-number.md) $2^i3^j5^k$ for nonnegative [integers](../../../../../integer-split.md) $i,j,k$. Every noninitial value has a smaller predecessor obtained by removing a factor, so the recursive demand can be supplied from earlier cells. This is the [productivity](../../../../../stream-productivity.md) argument for a [sorted multiplicative closure stream](../../../../../sorted-multiplicative-closure-stream.md). The [merge algorithm](../../../../../merge-algorithm.md) removes duplicate representations such as $2\cdot3=3\cdot2$, retaining strict order and every generated value.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [2](../../2.md)
3. [Functional programming, design and analysis of algorithms](../../../functional-programming-design-and-analysis-of-algorithms-split.md)
4. [2017](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
