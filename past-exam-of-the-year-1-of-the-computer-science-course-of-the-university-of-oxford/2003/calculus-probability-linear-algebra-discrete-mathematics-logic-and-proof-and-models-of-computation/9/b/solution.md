<h1 id="9/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The assertion is **false**. Use the [pumping lemma for regular languages](../../../../../pumping-lemma-for-regular-languages.md): if $L$ is a [regular language](../../../../../regular-language.md), there is $p\ge1$ such that every $w\in L$ with $|w|\ge p$ admits a factorization $w=xyz$ with $|xy|\le p$, $|y|\ge1$, and $xy^kz\in L$ for every integer $k\ge0$.

Suppose the stated [formal language](../../../../../formal-language.md) were a [regular language](../../../../../regular-language.md), and take $w=0^{2p}1^p$. This [string](../../../../../string.md) has twice as many zeros as ones, so it belongs to $L$. In every allowed factorization, the first $p$ positions are all zeros, forcing $y=0^d$ with $1\le d\le p$. Pumping down with $k=0$ produces

$$
xz=0^{2p-d}1^p.
$$

It still has $p$ ones but fewer than $2p$ zeros, contradicting the [pumping lemma for regular languages](../../../../../pumping-lemma-for-regular-languages.md). Thus

$$
\boxed{\{w:|w|_0=2|w|_1\}\text{ is not regular}.}
$$

## ↑ Ancestors (12)

1. [B](../b.md)
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
