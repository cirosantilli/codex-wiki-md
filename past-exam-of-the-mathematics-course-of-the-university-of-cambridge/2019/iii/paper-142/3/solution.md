<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

For a complex vector bundle $E\to X$, the [K-theory Euler class](../../../../../k-theory-euler-class.md) is the zero-section pullback of its [K-theory Thom class](../../../../../k-theory-thom-class.md):

$$
e^K(E)=\lambda_{-1}(\overline E)
=\sum_{j=0}^{\operatorname{rank}E}(-1)^j[\Lambda^j\overline E].
$$

The cofibration of the disk and sphere bundles gives the [K-theory Gysin sequence of a sphere bundle](../../../../../k-theory-gysin-sequence-of-a-sphere-bundle.md)

$$
\cdots\to K^i(X)\xrightarrow{\cdot e^K(E)}K^i(X)
\longrightarrow K^i(S(E))\longrightarrow K^{i+1}(X)\to\cdots.
$$

Let $\gamma=\gamma_{\mathbb C}^{1,n+1}$ be the [tautological bundle](../../../../../tautological-bundle.md). The [Euler sequence on complex projective space](../../../../../euler-sequence-on-complex-projective-space.md) gives the bundle isomorphism

$$
T\mathbb{CP}^n\oplus\mathbb C\cong(n+1)\overline\gamma.
$$

Put $t=1-[\gamma]$, so $K^0(\mathbb{CP}^n)=\mathbb Z[t]/(t^{n+1})$. From

$$
\lambda_s(\overline{T\mathbb{CP}^n})
=\frac{(1+s\gamma)^{n+1}}{1+s}
$$

and evaluation at $s=-1$, or polynomial division followed by differentiation at the removable root, we obtain

$$
e^K(T\mathbb{CP}^n)
=(n+1)[\gamma](1-[\gamma])^n
=\boxed{(n+1)t^n}.
$$

Because $K^{-1}(\mathbb{CP}^n)=0$, the Gysin sequence identifies even K-theory with the cokernel and odd K-theory with the kernel of multiplication by $(n+1)t^n$. Therefore

$$
\boxed{K^0(S(T\mathbb{CP}^n))
\cong\mathbb Z[t]/(t^{n+1},(n+1)t^n)
\cong\mathbb Z^n\oplus\mathbb Z/(n+1),}
$$

and, since multiplication only detects the constant coefficient,

$$
\boxed{K^{-1}(S(T\mathbb{CP}^n))\cong(t)\cong\mathbb Z^n.}
$$

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 142](../../paper-142-split.md)
3. [Iii](../../split.md)
4. [2019](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
