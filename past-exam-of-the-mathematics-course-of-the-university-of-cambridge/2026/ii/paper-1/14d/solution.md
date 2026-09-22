<h1 id="14d/solution">Solution</h1>

↑ **Parent:** [14D](../14d.md)

Put $\Gamma(z)=I(z)$ for $\Re z>0$. Integration by parts gives $\Gamma(z+1)=z\Gamma(z)$, both proving $\Gamma(n)=(n-1)!$ and defining the meromorphic continuation. A keyhole-contour evaluation of $\int_0^\infty t^{z-1}/(1+t)\,dt$ gives

$$
\Gamma(z)\Gamma(1-z)=\frac{\pi}{\sin\pi z}.
$$

For

$$
\Gamma(z)\Gamma(z+\tfrac12)=e^{g(z)}\Gamma(2z),
$$

the reflection formula at $z$ and $z+\tfrac12$ gives $g(z+1)-g(z)=-2\log2$. Thus $h(z)=g(z)+2z\log2$ is entire and $1$-periodic; poles and zeros have cancelled in the quotient. Its Fourier expansion and the exponential growth bound make it a finite Laurent [polynomial](../../../../../polynomial-split.md) in $e^{2\pi iz}$; the same growth bound for $e^h$ excludes every nonconstant mode. Hence $h=b$. At $z=1/2$, $e^b=2\sqrt\pi$, yielding the duplication formula.

Set $z=1/6$ and use reflection at $1/3$:

$$
\Gamma(\tfrac16)\Gamma(\tfrac23)=2^{2/3}\sqrt\pi\,\Gamma(\tfrac13),\qquad
\Gamma(\tfrac13)\Gamma(\tfrac23)=\frac{2\pi}{\sqrt3}.
$$

Therefore

$$
\boxed{\Gamma(\tfrac16)=2^{-1/3}\sqrt{\frac3\pi}\,\Gamma(\tfrac13)^2.}
$$

## ↑ Ancestors (10)

1. [14D](../14d.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ii](../../split.md)
4. [2026](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
