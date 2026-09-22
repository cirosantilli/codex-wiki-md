<h1 id="2/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

For the base case $n=2$, $1+1/\sqrt2>\sqrt2$, since multiplying by $\sqrt2$ reduces this to $\sqrt2+1>2$. Suppose the claimed inequality holds for some $n\geq2$. The identity

$$
\sqrt{n+1}-\sqrt n=\frac1{\sqrt{n+1}+\sqrt n}<\frac1{\sqrt{n+1}}
$$

then gives

$$
\sum_{k=1}^{n+1}\frac1{\sqrt k}
>\sqrt n+\frac1{\sqrt{n+1}}
>\sqrt{n+1}.
$$

Thus [mathematical induction](../../../../../../mathematical-induction.md) proves

$$
\boxed{\sqrt n<\sum_{k=1}^{n}\frac1{\sqrt k}\quad(n\geq2).}
$$

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [2](../../../2.md)
4. [Discrete mathematics, continuous mathematics, and probability (resit)](../../../../discrete-mathematics-continuous-mathematics-and-probability-resit-split.md)
5. [2015](../../../../split.md)
6. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../../split.md)
7. [Year 1 of the computer science course of the University of Oxford](../../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
8. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../split.md)
