<h1 id="5a/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Let $D=d/dx$ and write the constant-coefficient [linear ordinary differential equation](../../../../../../linear-ordinary-differential-equation.md) as $p(D)y=0$. Since $D^ke^{\lambda x}=\lambda^ke^{\lambda x}$,

$$
p(D)e^{\lambda x}=p(\lambda)e^{\lambda x}.
$$

The exponential never vanishes, so **$\boxed{e^{\lambda x}\text{ solves the equation }\Longleftrightarrow p(\lambda)=0}$**.

For the second claim, the [product rule](../../../../../../product-rule.md) gives

$$
D^k(xe^{\mu x})=e^{\mu x}(x\mu^k+k\mu^{k-1})
$$

for $k\geq1$, with the $k=0$ term treated separately. Summing the coefficients yields

$$
p(D)(xe^{\mu x})=e^{\mu x}\bigl(xp(\mu)+p'(\mu)\bigr).
$$

A root of multiplicity at least two has $p(\mu)=p'(\mu)=0$, proving **$xe^{\mu x}$ is also a solution**. This directly establishes the repeated-root contribution without assuming a solution formula. If the displayed coefficient list has leading zeros, the exponential calculation still applies to its actual [polynomial](../../../../../../polynomial-split.md) degree.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [5A](../../5a.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ia](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
