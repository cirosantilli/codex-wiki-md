<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Since $5^k\equiv1\pmod4$,

$$
g\left(\frac\pi2+\frac1n\right)-g\left(\frac\pi2\right)
=-\sum_{k=0}^\infty5^{-k}\sin(5^k/n).
$$

Choose $5^m\leq n<5^{m+1}$. For $k\leq m$, $\sin(5^k/n)\geq c5^k/n$, so each of these $m+1$ same-sign terms has magnitude at least $c/n$. The remaining tail is $O(5^{-m})=O(n^{-1})$. Hence

$$
\boxed{\left|g\left(\frac\pi2+\frac1n\right)-g\left(\frac\pi2\right)\right|
\geq c\frac{\log n}{n}},\qquad
\boxed{\omega(g,n^{-1})\geq c\frac{\log n}{n}}.
$$

**Thus $E_n(f)=O(n^{-1})$ does not imply $\omega(f,n^{-1})=O(n^{-1})$; the logarithmic gap prevents a characterization of that approximation class by this first modulus alone.**

## ↑ Ancestors (11)

1. [C](../c.md)
2. [1](../../1.md)
3. [Paper 318](../../../paper-318-split.md)
4. [Iii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
