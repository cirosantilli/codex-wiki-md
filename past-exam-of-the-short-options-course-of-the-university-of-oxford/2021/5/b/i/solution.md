<h1 id="5/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Write $F_j(p)=\mathcal Lf_j(p)$, using the square-root branch positive on real $p>0$. Integrating the differential equation and using boundedness at zero gives

$$
xf_1(x)=\int_0^x tf_0(t)\,dt.
$$

The integration constant is zero since $xf_1(x)\to0$. Continuity of $f_0$ then shows $f_1(x)=O(x)$, so $f_1$ extends continuously with $f_1(0)=0$.

The [Laplace transform of a derivative](../../../../../laplace-transform-of-a-derivative.md) and [differentiation under the integral sign](../../../../../differentiation-under-the-integral-sign.md) give

$$
-pF_1'(p)=-F_0'(p),\qquad F_1'(p)=\frac{F_0'(p)}p=-\frac1{(p^2+1)^{3/2}}.
$$

Integrating and using $F_1(p)\to0$ as real $p\to\infty$ fixes the constant:

$$
\boxed{F_1(p)=1-\frac p{\sqrt{p^2+1}}.}
$$

The [initial value theorem for Laplace transforms](../../../../../initial-value-theorem-for-laplace-transforms.md) gives $f_0(0)=\lim_{p\to\infty}pF_0(p)=1$. It is tempting to apply the derivative rule immediately to $f_0$, but its stated regularity is only continuity. To justify that step, define $h(x)=1-\int_0^x f_1(t)\,dt$. Then

$$
\mathcal Lh(p)=\frac{1-F_1(p)}p=\frac1{\sqrt{p^2+1}}=F_0(p).
$$

Uniqueness of the [Laplace transform](../../../../../laplace-transform.md) gives $h=f_0$, and hence $f_0$ is continuously differentiable and

$$
\boxed{f_1=-f_0'.}
$$

## ↑ Ancestors (13)

1. [I](../i.md)
2. [B](../../b.md)
3. [5](../../../5.md)
4. [2021](../../../../2021-split.md)
5. [Past exam of the short options course of the University of Oxford](../../../../split.md)
6. [Short options course of the University of Oxford](../../../../../short-options-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
