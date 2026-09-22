<h1 id="12a/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Apply the formula to

$$
R(z)=\frac{z}{1+z^4}.
$$

The upper-half-plane poles are

$$
z_1=e^{i\pi/4},\qquad z_2=e^{3i\pi/4},
$$

and their residues are $e^{iz_k}/(4z_k^2)$. Writing $c=1/\sqrt2$, their sum is

$$
\frac{i}{4}\left(e^{iz_2}-e^{iz_1}\right)
=\frac12e^{-c}\sin c.
$$

Since the cosine part of $x e^{ix}/(1+x^4)$ is [odd](../../../../../../odd-function.md), its integral vanishes, while the sine part is [even](../../../../../../even-function.md). Hence

$$
i\int_{-\infty}^{\infty}\frac{x\sin x}{1+x^4}\,dx
=2\pi i\left(\frac12e^{-c}\sin c\right),
$$

so

$$
\boxed{
\int_{-\infty}^{\infty}\frac{x\sin x}{1+x^4}\,dx
=\pi e^{-1/\sqrt2}\sin\!\left(\frac1{\sqrt2}\right)}.
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [12A](../../12a.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ib](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
