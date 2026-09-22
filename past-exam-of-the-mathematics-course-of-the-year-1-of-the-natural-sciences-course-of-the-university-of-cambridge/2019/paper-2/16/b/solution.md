<h1 id="16/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Write $q(x)=1/[x(1+(\ln x)^2)]$. The [vector field](../../../../../vector-field.md) is undefined at $x=0$ because $q$ diverges there, but this component is tangential to that face. The face fluxes have finite [improper integral](../../../../../improper-integral.md) limits. In particular, the substitution $s=\ln x$ gives

$$
J=\int_0^1q(x)\,dx=\int_{-\infty}^0\frac{ds}{1+s^2}=\frac\pi2.
$$

Using the outward [unit normal](../../../../../unit-normal.md) on each face, the [flux](../../../../../flux.md) contributions are

$$
\boxed{\begin{array}{c|c|c}
\text{face}&\mathbf F\cdot\hat{\mathbf n}&\text{outward flux}\\\hline
x=0&-1\text{ (normal trace)}&-1\\
x=1&e^{-1}&e^{-1}\\
y=0&-q(x)&-\pi/2\\
y=1&q(x)&\pi/2\\
z=0&0&0\\
z=1&1&1
\end{array}}
$$

Hence

$$
\boxed{\text{total outward flux}=e^{-1}}.
$$

For a precise justification at the singular face, first use the truncated cube $\varepsilon\leq x\leq1$. Its opposite $y$-face integrals cancel, the $x$-faces contribute $e^{-1}-e^{-\varepsilon}$, and the upper $z$-face contributes $1-\varepsilon$. The limit as $\varepsilon\downarrow0$ is $e^{-1}$. On each truncated cube the [divergence theorem](../../../../../divergence-theorem.md) gives the same answer, since $\nabla\cdot\mathbf F=1-e^{-x}$. Thus the result is a [flux of a vector field with an integrable tangential singularity](../../../../../flux-of-a-vector-field-with-an-integrable-tangential-singularity.md), rather than an application of the classical smooth-field theorem directly at $x=0$.

## ↑ Ancestors (13)

1. [B](../b.md)
2. [16](../../16.md)
3. [Paper 2](../../../paper-2-split.md)
4. [2019](../../../split.md)
5. [Past exam of the mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 1 of the natural sciences course of the University of Cambridge](../../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
