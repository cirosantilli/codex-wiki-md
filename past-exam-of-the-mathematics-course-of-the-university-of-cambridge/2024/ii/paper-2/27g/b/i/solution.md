<h1 id="27g/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Fix $\varepsilon>0$. Since a rate-one exponential variable has  
$\mathbb P(X_n>x)=e^{-x}$,

$$
\sum_n\mathbb P\{X_n>(1+\varepsilon)\log n\}
=\sum_n n^{-(1+\varepsilon)}<\infty.
$$

The first Borel--Cantelli lemma gives the upper bound  
$\limsup X_n/\log n\leq1$. Conversely,

$$
\sum_n\mathbb P\{X_n>(1-\varepsilon)\log n\}
=\sum_n n^{-(1-\varepsilon)}=\infty.
$$

These events are independent, so the second lemma makes them occur infinitely often. Hence the lower bound is $1-\varepsilon$. Letting rational $\varepsilon\downarrow0$ proves

$$
\boxed{\limsup_{n\to\infty}\frac{X_n}{\log n}=1}
\quad\hbox{almost surely}.
$$

## ↑ Ancestors (12)

1. [I](../i.md)
2. [B](../../b.md)
3. [27G](../../../27g.md)
4. [Paper 2](../../../../paper-2-split.md)
5. [Ii](../../../../split.md)
6. [2024](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
