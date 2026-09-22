# Polynomial kernel

↑ **Parent:** [Positive-semidefinite kernel](positive-semidefinite-kernel-split.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Polynomial_kernel)

For $x,z\in\mathbb R^d$, a polynomial kernel is the [positive-semidefinite kernel](positive-semidefinite-kernel-split.md) $k(x,z)=(x^Tz+c)^r$, where $r$ is a positive integer and $c\geq0$. The case $c=0$ uses [monomials](monomial.md) of total degree $r$; $c>0$ also includes lower degrees. The [feature map](feature-map.md) weights matter: listing each distinct [monomial](monomial.md) once with coefficient one generally gives a different [inner product](inner-product-split.md).[Section 4.2.2, pp. 89–90, equations (4.23)–(4.24): polynomial kernels and weighted monomial features](gaussian-processes-for-machine-learning-by-carl-edward-rasmussen-and-christopher-k-i-williams.md)

For the homogeneous quadratic case in two dimensions, take the scaled [quadratic feature map](quadratic-feature-map.md)

$$
\phi(x_1,x_2)=\begin{pmatrix}x_1^2\\\sqrt2 x_1x_2\\x_2^2\end{pmatrix},\qquad k(x,z)=(x^Tz)^2.
$$

The [inner product](inner-product-split.md) identity is explicit:

$$
\phi(x)^T\phi(z)=x_1^2z_1^2+2x_1x_2z_1z_2+x_2^2z_2^2=(x_1z_1+x_2z_2)^2=k(x,z).
$$

The factor $\sqrt2$ accounts for the two equal cross terms in the square. Thus an [inner product](inner-product-split.md) of three derived coordinates can be obtained from an [inner product](inner-product-split.md) of the two input coordinates followed by squaring. The [kernel trick](kernel-trick.md) uses this equality inside an algorithm; the [feature map](feature-map.md) explains which nonlinear [functions](function-split.md) the algorithm can represent.

## ↑ Ancestors (5)

1. [Positive-semidefinite kernel](positive-semidefinite-kernel-split.md)
2. [Probability and statistics](probability-and-statistics-split.md)
3. [Area of mathematics](area-of-mathematics.md)
4. [Mathematics](mathematics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (4)

- [Computational tradeoffs of the kernel trick](computational-tradeoffs-of-the-kernel-trick.md)
- [Dual prediction with a kernel](dual-prediction-with-a-kernel.md)
- [Kernel trick](kernel-trick.md)
- [XOR separation by a product feature](xor-separation-by-a-product-feature.md)
