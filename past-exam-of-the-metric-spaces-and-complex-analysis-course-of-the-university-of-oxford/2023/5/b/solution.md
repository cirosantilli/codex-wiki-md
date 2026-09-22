<h1 id="5/b/solution">Solution</h1>

↑ **Parent:** [b](../b.md)

The [improper integral](../../../../improper-integral.md) converges: its integrand is bounded near zero and at most $x^{-n}$ for $x\geq1$, which is integrable because $n\geq2$.

Set $\theta=\pi/n$, $\omega=e^{2i\theta}$ and $\zeta=e^{i\theta}$. Apply the [residue theorem](../../../../residue-theorem.md) to $F(z)=1/(1+z^n)$ on the positively oriented sector contour consisting of the segment $0\to R$, the arc $Re^{it}$ for $0\leq t\leq2\theta$, and the segment $R\omega\to0$, with $R>1$. No [pole](../../../../pole.md) lies on the boundary. Exactly one root of $z^n=-1$ is inside this sector, namely $\zeta$; it is a [simple pole](../../../../simple-pole.md). Part (a) gives

$$
\operatorname{Res}_{\zeta}F=\frac1{n\zeta^{n-1}}=-\frac\zeta n.
$$

On the returning ray, put $z=\omega x$ with $x$ decreasing from $R$ to zero. Since $\omega^n=1$, the two ray contributions are

$$
\int_0^R\frac{dx}{1+x^n}+\int_R^0\frac{\omega\,dx}{1+x^n}=(1-\omega)I_R,
\qquad I_R=\int_0^R\frac{dx}{1+x^n}.
$$

On the arc, $|1+z^n|\geq R^n-1$, so the [estimation lemma](../../../../estimation-lemma.md) bounds its [contour integral](../../../../contour-integral.md) by

$$
\frac{2\pi R}{n(R^n-1)}\longrightarrow0.
$$

The [residue theorem](../../../../residue-theorem.md) and the convergence already established now give

$$
(1-e^{2i\theta})I=-\frac{2\pi i}{n}e^{i\theta}.
$$

Using $1-e^{2i\theta}=-2ie^{i\theta}\sin\theta$, we conclude

$$
\boxed{\int_0^\infty\frac{dx}{1+x^n}=\frac\pi{n\sin(\pi/n)}\qquad(n\geq2)}.
$$

The sector also works for $n=2$, when it is the upper semicircle. Its angle is chosen so that $z^n$ has the same value on the two rays.

## ↑ Ancestors (12)

1. [b](../b.md)
2. [5](../../5.md)
3. [2023](../../../2023-split.md)
4. [Past exam of the metric spaces and complex analysis course of the University of Oxford](../../../split.md)
5. [Metric spaces and complex analysis course of the University of Oxford](../../../../metric-spaces-and-complex-analysis-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
