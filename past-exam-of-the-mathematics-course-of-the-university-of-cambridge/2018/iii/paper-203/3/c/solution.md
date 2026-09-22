<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Set $F(w)=(\phi(w)-\phi(0))/w$ for $w\ne0$. The singularity is removable, with $F(0)=\phi'(0)$. Injectivity of the [conformal map](../../../../../../conformal-map.md) makes $F(w)\ne0$ away from zero, and conformality makes $F(0)\ne0$ as well. Since the disc is simply connected, $F$ has a [holomorphic logarithm](../../../../../../holomorphic-logarithm.md). Therefore $\psi=\log|F|$ is a [harmonic function](../../../../../../harmonic-function.md), including at zero, and $\psi(0)=\log|\phi'(0)|$.

The [mean value property for harmonic functions](../../../../../../mean-value-property-for-harmonic-functions.md) gives, for every $0<r<1$,

$$
\log|\phi'(0)|=\frac1{2\pi}\int_0^{2\pi}\log|\phi(re^{i\theta})-\phi(0)|\,d\theta-\log r.
$$

For general $D$, boundary values mean radial limits, rather than a continuous extension of $\phi$ to every point of the circle. The [boundary logarithmic mean of a univalent function](../../../../../../boundary-logarithmic-mean-of-a-univalent-function.md) justifies taking $r\uparrow1$: the [Koebe distortion theorem](../../../../../../koebe-distortion-theorem.md) bounds $|F|$ below by $|\phi'(0)|/4$, while the standard integral-mean bound for a [univalent function](../../../../../../univalent-function.md), $\sup_{r<1}\int|\phi(re^{i\theta})|^p d\theta<\infty$ for $0<p<1/2$, gives [uniform integrability](../../../../../../uniform-integrability.md) of its positive logarithm. Radial limits exist almost everywhere, and passage to the integral follows. Thus, writing $dw=d\theta$ for arc length on the unit circle,

$$
\boxed{\log|\phi'(0)|=\frac1{2\pi}\int_{\partial\mathbb D}\log|\phi(w)-\phi(0)|\,dw.}
$$

The expression on the left is the logarithm of the [conformal radius](../../../../../../conformal-radius.md) of $D$ at $z=\phi(0)$.

## ↑ Ancestors (11)

1. [C](../c.md)
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
