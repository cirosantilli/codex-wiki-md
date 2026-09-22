<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The expression is a [Test-function pairing with a Gaussian free field](../../../../../../test-function-pairing-with-a-gaussian-free-field.md), rather than the pointwise integral of an ordinary random function. For a real [test function](../../../../../../test-function.md) $\phi$, take the Dirichlet solution

$$
f_\phi=-2\pi\Delta^{-1}\phi,
\qquad f_\phi(x)=\int_DG(x,y)\phi(y)\,dy,
$$

using the Green-kernel identity allowed in the original PDF. In particular, $-\Delta f_\phi=2\pi\phi$. [Integration by parts](../../../../../../integration-by-parts.md) gives, initially for smooth compactly supported $u$ and then by [continuity](../../../../../../continuous-function.md) in the [Dirichlet energy space](../../../../../../dirichlet-energy-space.md),

$$
(u,f_\phi)_\nabla=\frac1{2\pi}\int_D\nabla u\cdot\nabla f_\phi
=\int_Du(x)\phi(x)\,dx.
$$

The integral functional is continuous in the energy norm: pull back to the [unit disc](../../../../../../unit-disc.md), where the transformed test function has compact support, and use the [Poincaré inequality](../../../../../../poincare-inequality.md). Hence $f_\phi$ is its energy-space representer. Define

$$
\boxed{(h,\phi):=(h,f_\phi)_\nabla.}
$$

By the [isonormal Gaussian process](../../../../../../isonormal-gaussian-process.md) definition, it has mean zero and [variance](../../../../../../variance-split.md)

$$
\begin{aligned}
\mathbb E[(h,\phi)^2]
&=\|f_\phi\|_\nabla^2
=\int_D f_\phi(x)\phi(x)\,dx\\
&=\iint_{D\times D}\phi(x)G(x,y)\phi(y)\,dx\,dy.
\end{aligned}
$$

The logarithmic singularity is locally integrable, so this [variance](../../../../../../variance-split.md) is finite for smooth compactly supported test functions. Thus

$$
\boxed{(h,\phi)\sim N\!\left(0,\iint\phi(x)G(x,y)\phi(y)\,dx\,dy\right).}
$$

The local TeX corrupted the double integral and the bracketed Green-kernel identity; the PDF supplies the identity above and does not assert an infinite [variance](../../../../../../variance-split.md).

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 203](../../../paper-203-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
