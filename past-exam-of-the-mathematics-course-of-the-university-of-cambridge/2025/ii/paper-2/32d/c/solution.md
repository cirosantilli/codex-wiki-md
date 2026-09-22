<h1 id="32d/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Put $y=\lambda x$ and $t=y+s$. Factoring out the endpoint value gives

$$
\gamma(x,y)=y^{x-1}e^{-y}
\int_0^\infty
\exp\left((x-1)\log\left(1+\frac{s}{\lambda x}\right)-s\right)ds.
$$

For fixed $s$,

$$
(x-1)\log\left(1+\frac{s}{\lambda x}\right)-s
=-\frac{\lambda-1}{\lambda}s
-\frac1x\left(\frac{s}{\lambda}+\frac{s^2}{2\lambda^2}\right)
+O(x^{-2}).
$$

Watson's endpoint lemma justifies termwise integration, so with $\alpha=(\lambda-1)/\lambda$,

$$
\begin{aligned}
\frac{\gamma(x,y)}{y^{x-1}e^{-y}}
&\sim\int_0^\infty e^{-\alpha s}
\left[1-\frac1x\left(\frac{s}{\lambda}
+\frac{s^2}{2\lambda^2}\right)\right]ds\\
&=\frac1\alpha
-\frac1x\left(\frac1{\lambda\alpha^2}
+\frac1{\lambda^2\alpha^3}\right).
\end{aligned}
$$

Consequently

$$
\boxed{
f(\lambda)=\frac{\lambda}{\lambda-1},
\qquad
g(\lambda)=-\frac{\lambda^2}{(\lambda-1)^3}.}
$$

## ↑ Ancestors (11)

1. [C](../c.md)
2. [32D](../../32d.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
