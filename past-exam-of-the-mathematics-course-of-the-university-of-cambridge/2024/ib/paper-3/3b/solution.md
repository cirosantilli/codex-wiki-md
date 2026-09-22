<h1 id="3b/solution">Solution</h1>

↑ **Parent:** [3B](../3b.md)

The [Cauchy integral theorem](../../../../../cauchy-s-integral-theorem.md) states that if $f$ is holomorphic on a simply connected domain, then its [integral](../../../../../integral.md) around every closed piecewise smooth contour in that domain is zero.

Put $q=b-k$. Completing the square gives

$$
-ax^2+iqx
=-a\left(x-\frac{iq}{2a}\right)^2-
\frac{q^2}{4a}.
$$

After the change of variable $z=x-iq/(2a)$, the [integral](../../../../../integral.md) runs along the horizontal line $\operatorname{Im}z=-q/(2a)$. The integrand $e^{-az^2}$ is entire. Apply Cauchy's theorem to a rectangle joining this line to the real axis; the two vertical [integrals](../../../../../integral.md) tend to zero as their real parts tend to $\pm\infty$, because $a>0$. The contour may therefore be shifted to the real line. Hence the [Fourier transform of a Gaussian](../../../../../fourier-transform-of-a-gaussian.md) gives

$$
\begin{aligned}
\widehat f_{a,b}(k)
&=e^{-q^2/(4a)}\int_{-\infty}^{\infty}e^{-az^2}\,dz\\
&=\boxed{\sqrt{\frac\pi a}
\exp\left[-\frac{(k-b)^2}{4a}\right]}.
\end{aligned}
$$

## ↑ Ancestors (10)

1. [3B](../3b.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ib](../../split.md)
4. [2024](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
