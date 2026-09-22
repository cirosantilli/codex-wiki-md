<h1 id="25j/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Split the overlapping products into two nonoverlapping families:

$$
U_n=\sum_{j=1}^nX_{2j-1}X_{2j}+\sum_{j=1}^nX_{2j}X_{2j+1}.
$$

Within each sum the summands depend on disjoint independent pairs and are independent identically distributed Bernoulli variables of mean $1/4$. The two families need not be independent of each other. The [strong law of large numbers](../../../../../../strong-law-of-large-numbers.md) says that averages of independent identically distributed integrable random variables converge [almost surely](../../../../../../almost-sure-convergence.md) to their [expectation](../../../../../../expected-value.md). Applying it separately to each family and intersecting the two probability-one events gives

$$
\boxed{\frac{U_n}{n}\longrightarrow\frac14+\frac14=\frac12\quad\text{almost surely}.}
$$

## ↑ Ancestors (11)

1. [D](../d.md)
2. [25J](../../25j.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
