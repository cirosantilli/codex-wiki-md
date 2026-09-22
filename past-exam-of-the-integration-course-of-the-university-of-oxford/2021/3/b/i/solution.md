<h1 id="3/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

The points belonging to infinitely many $E_n$ form their [limit superior of sets](../../../../../limit-superior-of-sets.md):

$$
G=\bigcap_{N\geq1}\bigcup_{n\geq N}E_n.
$$

For every $N$, [countable subadditivity](../../../../../countable-subadditivity-of-a-measure.md) gives

$$
0\leq m(G)\leq\sum_{n\geq N}m(E_n)\leq\sum_{n\geq N}2^{-n}=2^{1-N}\longrightarrow0.
$$

Thus $\boxed{m(G)=0}$. Outside this [null set](../../../../../null-set.md), each point belongs to only finitely many $E_n$, so its [indicator functions](../../../../../indicator-function.md) are eventually zero. Therefore $\boxed{\chi_{E_n}(x)\to0\text{ almost everywhere}}$. This is the summable-measure argument behind the first [Borel-Cantelli lemma](../../../../../borel-cantelli-lemmas.md); no [independence](../../../../../independent-random-variables.md) assumption is needed.

## ↑ Ancestors (13)

1. [I](../i.md)
2. [B](../../b.md)
3. [3](../../../3.md)
4. [2021](../../../../2021-split.md)
5. [Past exam of the integration course of the University of Oxford](../../../../split.md)
6. [Integration course of the University of Oxford](../../../../../integration-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
