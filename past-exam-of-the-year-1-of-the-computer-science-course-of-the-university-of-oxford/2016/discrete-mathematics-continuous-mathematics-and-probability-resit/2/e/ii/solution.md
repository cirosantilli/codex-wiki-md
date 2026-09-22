<h1 id="2/e/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Write $n=2r$ and $k=2s$. Partition an $n$-element [set](../../../../../../set-split.md) into $r$ distinguished pairs, and let $\tau$ interchange the two elements of every pair. It induces an [involution](../../../../../../involution.md) on the $k$-element subsets. Every nonfixed subset is paired with its distinct image, so nonfixed subsets contribute an even number to the [binomial coefficient](../../../../../../binomial-coefficient-split.md) $\binom{2r}{2s}$.

A fixed subset contains either both or neither of the elements of each distinguished pair. Since it contains $2s$ elements, it consists of exactly $s$ whole pairs. There are $\binom rs$ such fixed subsets. Counting modulo $2$ therefore gives

$$
\boxed{\binom nk\equiv\binom{n/2}{k/2}\pmod2}.
$$

The same [involution](../../../../../../involution.md) explains part (i): a fixed subset cannot have odd size.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [E](../../e.md)
3. [2](../../../2.md)
4. [Discrete mathematics, continuous mathematics and probability (resit)](../../../../discrete-mathematics-continuous-mathematics-and-probability-resit-split.md)
5. [2016](../../../../split.md)
6. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../../split.md)
7. [Year 1 of the computer science course of the University of Oxford](../../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
8. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../split.md)
