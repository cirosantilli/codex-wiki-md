<h1 id="27g/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

First assume the stated $\varepsilon$--$\delta$ condition. If $\nu(A)=0$, then $\nu(A)<\delta$ for the $\delta$ belonging to every $\varepsilon>0$, so $\mu(A)<\varepsilon$ for every $\varepsilon$ and $\mu(A)=0$. Hence $\mu\ll\nu$.

Conversely, suppose $\mu\ll\nu$ but the uniform condition fails. Then for some $\varepsilon>0$ there are sets $A_n$ with

$$
\nu(A_n)<2^{-n},\qquad \mu(A_n)\geq\varepsilon.
$$

Put $B_m=\bigcup_{n\geq m}A_n$. Then $\nu(B_m)\leq2^{1-m}$ and $B_m\downarrow B=\limsup A_n$, so $\nu(B)=0$. Absolute continuity gives $\mu(B)=0$. But $\mu(B_m)\geq\varepsilon$, and the finiteness of $\mu(\Omega)$ permits continuity from above:

$$
\mu(B)=\lim_m\mu(B_m)\geq\varepsilon,
$$

a contradiction. This proves [uniform absolute continuity for a finite measure](../../../../../../uniform-absolute-continuity-for-a-finite-measure.md).

## ↑ Ancestors (11)

1. [C](../c.md)
2. [27G](../../27g.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
