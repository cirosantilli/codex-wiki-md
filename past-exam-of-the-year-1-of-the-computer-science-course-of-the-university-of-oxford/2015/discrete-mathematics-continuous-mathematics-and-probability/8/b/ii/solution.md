<h1 id="8/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Group the elements of a colouring by equality of colour. This creates a unique [partition of a set](../../../../../../partition-of-a-set.md) into nonempty unlabelled blocks, each of one colour, with distinct blocks assigned distinct colours.

For a [partition of a set](../../../../../../partition-of-a-set.md) with $k$ blocks, assigning distinct colours to the blocks gives the [falling factorial](../../../../../../falling-factorial.md) $x(x-1)\cdots(x-k+1)$ possibilities. To see that no extra factor $k!$ is needed, order the blocks canonically by their smallest elements, then assign colours in that order. There are $A(n,k)$ possible [set partitions](../../../../../../set-partition.md) with $k$ blocks; these numbers are the [Stirling numbers of the second kind](../../../../../../stirling-numbers-of-the-second-kind.md).

Every colouring is counted exactly once in exactly one value of $k$, so

$$
\boxed{x^n=\sum_{k=1}^n A(n,k)x(x-1)\cdots(x-k+1).}
$$

For $k>x$, no colouring of the blocks is possible and the displayed [falling factorial](../../../../../../falling-factorial.md) is zero, because one factor is $x-x$.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [8](../../../8.md)
4. [Discrete mathematics, continuous mathematics, and probability](../../../../discrete-mathematics-continuous-mathematics-and-probability-split.md)
5. [2015](../../../../split.md)
6. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../../split.md)
7. [Year 1 of the computer science course of the University of Oxford](../../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
8. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../split.md)
