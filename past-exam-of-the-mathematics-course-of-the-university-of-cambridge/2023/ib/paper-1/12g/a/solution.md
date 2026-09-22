<h1 id="12g/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Termwise [differentiation](../../../../../../differentiation.md) inside the disc gives

$$
f'(z)=\sum_{n=1}^{\infty}(1-z)^{n-1}=\frac1z.
$$

Consequently

$$
\frac d{dz}\bigl(ze^{-f(z)})
=e^{-f(z)}(1-zf'(z))=0.
$$

Since $f(1)=0$, the constant is one, so $e^{f(z)}=z$. Thus $f$ is an analytic branch of the logarithm on $D(1,1)$ with the required value.

Given $a\in D$, write $a=|a|e^{i\theta_a}$ with $0<\theta_a<2\pi$. On $|z/a-1|<1$, define

$$
\ell_a(z)=f(z/a)+\log|a|+i\theta_a.
$$

Then $e^{\ell_a(z)}=z$ and $\operatorname{Im}\ell_a(a)=\theta_a$. After shrinking the neighbourhood of $a$, continuity keeps its imaginary part in $(0,2\pi)$.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [12G](../../12g.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ib](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
