<h1 id="a/3/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

The [double-angle formula](../../../../../double-angle-formula.md) gives

$$
3\pm4\cos\theta+\cos2\theta=2(1\pm\cos\theta)^2\ge0.
$$

For $\sigma>1$, the [logarithm](../../../../../logarithm.md) of the absolutely convergent [Euler product](../../../../../euler-product.md) gives

$$
\begin{aligned}
&3\log\zeta(\sigma)+4\log|\zeta(\sigma+it)|+\log|\zeta(\sigma+2it)|\\
&=\sum_p\sum_{m\ge1}\frac{3+4\cos(mt\log p)+\cos(2mt\log p)}{mp^{m\sigma}}\ge0.
\end{aligned}
$$

Exponentiation proves

$$
\boxed{\zeta(\sigma)^3|\zeta(\sigma+it)|^4|\zeta(\sigma+2it)|\ge1.}
$$

Suppose $\zeta(1+it)=0$ for $t\ne0$, of order $r\ge1$. As $\sigma\downarrow1$, its middle factor is $O((\sigma-1)^{4r})$, the first is $O((\sigma-1)^{-3})$ because the [pole](../../../../../pole.md) at one is simple, and the final factor is bounded because $1+2it\ne1$. The product is $O((\sigma-1)^{4r-3})\to0$, contradicting the lower bound one. Therefore

$$
\boxed{\zeta(1+it)\ne0\qquad(t\ne0).}
$$

This is the [three-four-one zero-free-region argument](../../../../../three-four-one-zero-free-region-argument.md) specialized to the line with real part one.

## ↑ Ancestors (13)

1. [I](../i.md)
2. [3](../../3.md)
3. [A](../../../a.md)
4. [2007](../../../../2007-split.md)
5. [Past exam of the analytic number theory and elliptic curves course of the University of Oxford](../../../../split.md)
6. [Analytic number theory and elliptic curves course of the University of Oxford](../../../../../analytic-number-theory-and-elliptic-curves-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
