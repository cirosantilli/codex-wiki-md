<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For $q\geq1$, choose an ordered list of $q$ distinct elements: there are $n(n-1)\cdots(n-q+1)$ such lists. Every $q$-element [subset](../../../../../subset.md) occurs in exactly $q!$ orders, the number of [permutations](../../../../../permutation.md) of its elements. Thus the count is the [binomial coefficient](../../../../../binomial-coefficient-split.md)

$$
\boxed{\binom nq=\frac{n(n-1)\cdots(n-q+1)}{q!}.}
$$

For fixed $q$ and $n\geq2q$, every numerator factor lies between $n/2$ and $n$. Consequently

$$
\frac{n^q}{2^q q!}\leq\binom nq\leq\frac{n^q}{q!}.
$$

The constants depend on the fixed $q$, not on $n$. These inequalities prove $\binom nq=\Theta(n^q)$ in [big theta notation](../../../../../big-theta-notation.md). More precisely, dividing the product by $n^q$ gives the [fixed-cardinality binomial coefficient asymptotic](../../../../../fixed-cardinality-binomial-coefficient-asymptotic.md) $\binom nq\sim n^q/q!$. For $q=0$, there is exactly one empty [subset](../../../../../subset.md), and the assertion is $1=\Theta(1)$.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [3](../../3.md)
3. [Discrete mathematics, continuous mathematics, and probability](../../../discrete-mathematics-continuous-mathematics-and-probability-split.md)
4. [2021](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
