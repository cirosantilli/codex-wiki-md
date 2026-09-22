<h1 id="b/4/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

The [generating function](../../../../../generating-function.md) gives $P_n(-t)=(-1)^nP_n(t)$, so the odd function $f$ is orthogonal to every even-degree [Legendre polynomial](../../../../../legendre-polynomial.md). For $n\geq1$, integrate the self-adjoint form of the [Legendre differential equation](../../../../../legendre-differential-equation.md) from zero to one:

$$
[(1-t^2)P_n'(t)]_0^1+n(n+1)\int_0^1P_n(t)dt=0.
$$

Thus $\int_0^1P_n=P_n'(0)/(n(n+1))$. Differentiating the [generating function](../../../../../generating-function.md) in $t$ and then setting $t=0$ gives

$$
\sum_nP_n'(0)z^n=z(1+z^2)^{-3/2},\qquad P_{2m+1}'(0)=(-1)^m\frac{(2m+1)!}{2^{2m}(m!)^2}.
$$

Combining these identities with the normalization of $p_n$ yields

$$
\boxed{\langle f,p_{2m}\rangle=0,\qquad\langle f,p_{2m+1}\rangle=(-1)^m\sqrt{\frac{4m+3}{2}}\frac{(2m)!}{2^{2m}m!(m+1)!}.}
$$

For the [Legendre expansion of the sign function](../../../../../legendre-expansion-of-the-sign-function.md), $\|f\|_2^2=2$, so the [Parseval identity](../../../../../parseval-identity.md) gives

$$
2=\sum_{m\geq0}\frac{4m+3}{2}\frac{((2m)!)^2}{2^{4m}(m!(m+1)!)^2}.
$$

Therefore the requested sum equals

$$
\boxed{4.}
$$

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [4](../../4.md)
3. [B](../../../b.md)
4. [2009](../../../../2009-split.md)
5. [Past exam of the analysis course of the University of Oxford](../../../../split.md)
6. [Analysis course of the University of Oxford](../../../../../analysis-course-of-the-university-of-oxford.md)
7. [Year 3 of the mathematics course of the University of Oxford](../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
