<h1 id="6h/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For $\sigma>0$, the density is

$$
p_\sigma(x)=\frac1{\sqrt{2\pi}\sigma}
\exp\left(-\frac{x^2}{2\sigma^2}\right)
=g_\sigma(|x|),
$$

so the [Fisher-Neyman factorization theorem](../../../../../../fisher-neyman-factorization-theorem.md) proves that $|X|$ is sufficient.

Moreover,

$$
\frac{p_\sigma(x)}{p_\sigma(y)}
=\exp\left(-\frac{x^2-y^2}{2\sigma^2}\right)
$$

is independent of $\sigma$ exactly when $x^2=y^2$, equivalently $|x|=|y|$. The [likelihood-ratio criterion for minimal sufficiency](../../../../../../likelihood-ratio-criterion-for-minimal-sufficiency.md) therefore proves that

$$
\boxed{|X|\text{ is minimal sufficient}.}
$$

## ↑ Ancestors (11)

1. [C](../c.md)
2. [6H](../../6h.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ib](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
