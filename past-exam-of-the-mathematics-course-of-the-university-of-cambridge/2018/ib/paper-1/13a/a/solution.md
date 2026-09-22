<h1 id="13a/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The integrand

$$
F(z)=\frac{e^{iz^2/(4\pi)}}{e^{z/2}-e^{-z/2}}
$$

has one pole inside the rectangle, at $z=0$, with residue $1$. The [residue theorem](../../../../../../residue-theorem.md) therefore gives $\int_CF(z)\,dz=2\pi i$. The vertical-side integrals tend to zero as $R\to\infty$.

On the horizontal sides, direct substitution $z=x\pm\pi i$, with the upper side oppositely oriented, shows that their sum is

$$
i e^{-i\pi/4}\int_{-R}^{R}e^{ix^2/(4\pi)}
\left(\frac1{1+e^x}+\frac{e^x}{1+e^x}\right)dx.
$$

Taking the limit and comparing with $2\pi i$ gives

$$
\boxed{\lim_{R\to\infty}\int_{-R}^{R}e^{ix^2/(4\pi)}\,dx
=2\pi e^{i\pi/4}.}
$$

## ↑ Ancestors (11)

1. [A](../a.md)
2. [13A](../../13a.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ib](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
