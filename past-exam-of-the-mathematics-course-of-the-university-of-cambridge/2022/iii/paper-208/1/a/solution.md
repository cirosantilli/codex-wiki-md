<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Let

$$
M(\lambda)=\mathbb Ee^{\lambda X},
\qquad
\psi(\lambda)=\log M(\lambda).
$$

The [entropy functional](../../../../../../entropy-functional.md) satisfies

$$
\frac{\operatorname{Ent}(e^{\lambda X})}{M(\lambda)}
=\lambda\psi'(\lambda)-\psi(\lambda).
$$

Hence the assumed inequality gives

$$
\left(\frac{\psi(\lambda)}{\lambda}\right)'
=\frac{\lambda\psi'(\lambda)-\psi(\lambda)}{\lambda^2}
\leq\frac\nu2.
$$

Because $\mathbb EX=0$, $\psi(\lambda)/\lambda\to0$ as $\lambda\to0$. Integrating from zero to $\lambda$ when $\lambda>0$, and from $\lambda$ to zero and then multiplying by the negative number $\lambda$ when $\lambda<0$, gives in both cases

$$
\psi(\lambda)\leq\frac{\nu\lambda^2}{2}.
$$

**Thus $\mathbb Ee^{\lambda X}\leq e^{\nu\lambda^2/2}$ for every real $\lambda$, which is precisely the [sub-Gaussian random variable](../../../../../../sub-gaussian-distribution.md) bound with variance parameter $\nu$. This integration is the [Herbst argument](../../../../../../herbst-argument.md).**

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 208](../../../paper-208-split.md)
4. [Iii](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
