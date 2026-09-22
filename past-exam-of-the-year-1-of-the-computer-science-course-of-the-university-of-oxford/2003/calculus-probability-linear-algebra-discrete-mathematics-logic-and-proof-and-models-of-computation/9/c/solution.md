<h1 id="9/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The assertion is **false**. Suppose the [formal language](../../../../../formal-language.md) $L=\{ww:w\in\{0,1\}^*\}$ were a [regular language](../../../../../regular-language.md), and let $p$ be its constant from the [pumping lemma for regular languages](../../../../../pumping-lemma-for-regular-languages.md). Consider

$$
t=0^p1\,0^p1\in L.
$$

In every decomposition $t=xyz$ with $|xy|\le p$ and $|y|\ge1$, the pumped factor is $y=0^d$ with $1\le d\le p$. Pumping down gives

$$
xz=0^{p-d}1\,0^p1.
$$

This [string](../../../../../string.md) has exactly two ones and ends in a one. If it were $vv$, each copy of $v$ would contain exactly one one, and each copy would end in a one. The first copy would consequently be $0^{p-d}1$, while the second would be $0^p1$. They have different lengths because $d>0$, so they cannot be equal. This contradiction to the [pumping lemma for regular languages](../../../../../pumping-lemma-for-regular-languages.md) proves

$$
\boxed{\{ww:w\in\{0,1\}^*\}\text{ is not regular}.}
$$

## ↑ Ancestors (12)

1. [C](../c.md)
2. [9](../../9.md)
3. [Calculus, probability, linear algebra, discrete mathematics, logic and proof, and models of computation](../../../calculus-probability-linear-algebra-discrete-mathematics-logic-and-proof-and-models-of-computation-split.md)
4. [2003](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
