<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Fix $a<b<c<1$ and choose

$$
\lambda=\operatorname{arctanh}b.
$$

Under $\mathbb P_\lambda$, the increments remain independent and identically distributed, with mean $\psi'(\lambda)=b$. The [strong law of large numbers](../../../../../../strong-law-of-large-numbers.md) therefore gives

$$
\mathbb P_\lambda(an\leq S_n\leq cn)\longrightarrow1.
$$

Part (b) implies

$$
\liminf_{n\to\infty}\frac1n\log\mathbb P(S_n\geq an)
\geq-\lambda c+\psi(\lambda).
$$

Let $c\downarrow b$ and then $b\downarrow a$. Since $\lambda b-\psi(\lambda)=\psi^*(b)$ and $\psi^*$ is continuous on $[0,1)$,

$$
\boxed{\liminf_{n\to\infty}\frac1n
\log\mathbb P(S_n\geq an)\geq-\psi^*(a).}
$$

The same argument includes $a=0$ by taking $b\downarrow0$.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [3](../../3.md)
3. [Paper 201](../../../paper-201-split.md)
4. [Iii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
