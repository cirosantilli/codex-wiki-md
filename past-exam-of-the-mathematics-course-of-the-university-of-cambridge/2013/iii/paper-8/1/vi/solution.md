<h1 id="1/vi/solution">Solution</h1>

↑ **Parent:** [Vi](../vi.md)

For the [Hurwitz proof of the planar isoperimetric inequality](../../../../../../hurwitz-proof-of-the-planar-isoperimetric-inequality.md), take a positively oriented regular simple closed curve of length $L$ and enclosed area $A$. Write its complex position as $z(t)=x(t)+iy(t)$, with $0\leq t\leq2\pi$ proportional to [arc length](../../../../../../arc-length.md). Then $|z'(t)|=L/(2\pi)$. Translate the curve to make its mean position zero, and write its [Fourier coefficients](../../../../../../fourier-coefficient.md) as $c_n$, with $c_0=0$.

[Green's theorem](../../../../../../green-theorem.md) gives the signed area, and [Parseval's identity](../../../../../../parseval-identity.md) computes it:

$$
A=\frac12\int_0^{2\pi}(xy'-yx')\,dt
=\frac12\operatorname{Im}\int_0^{2\pi}\overline z\,z'\,dt
=\pi\sum_{n\in\mathbb Z}n|c_n|^2.
$$

Periodic [integration by parts](../../../../../../integration-by-parts.md) and [Parseval's identity](../../../../../../parseval-identity.md) applied to $z'$ give

$$
\sum_n n^2|c_n|^2=\frac1{2\pi}\int_0^{2\pi}|z'|^2\,dt
=\frac{L^2}{4\pi^2}.
$$

Since $n\leq n^2$ for every integer $n$,

$$
\boxed{A\leq\pi\sum_n n^2|c_n|^2
=\frac{L^2}{4\pi},\qquad L^2\geq4\pi A.}
$$

The sums converge absolutely: $\sum|n||c_n|^2\leq(\sum|c_n|^2)^{1/2}(\sum n^2|c_n|^2)^{1/2}$. Equality forces $c_n=0$ unless $n=0$ or $1$; after the mean translation, $z(t)=c_1e^{it}$ is a circle. Conversely a circle attains equality. Thus **circles uniquely attain equality, up to translation and orientation**.

The same proof applies to a rectifiable simple closed curve using its Lipschitz [arc length](../../../../../../arc-length.md) parametrization. Its derivative exists almost everywhere and belongs to $L^2$; periodic [mollification](../../../../../../mollification.md) converges to the curve in the function and derivative $L^2$ norms. This justifies the derivative coefficient identity, [Parseval's identity](../../../../../../parseval-identity.md) and area integral by approximation. Reversing orientation, if necessary, makes the enclosed area positive. The printed name “Hurewitz” is read as Hurwitz.

## ↑ Ancestors (11)

1. [Vi](../vi.md)
2. [1](../../1.md)
3. [Paper 8](../../../paper-8-split.md)
4. [Iii](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
