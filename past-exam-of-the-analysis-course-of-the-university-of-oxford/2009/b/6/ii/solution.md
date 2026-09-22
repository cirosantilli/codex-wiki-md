<h1 id="b/6/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

For the [adjoint of an integration operator anchored at zero](../../../../../adjoint-of-an-integration-operator-anchored-at-zero.md), use the [inner product](../../../../../inner-product-split.md) $\langle f,g\rangle=\int f\bar g$. On the positive half-interval, reversing the triangular integration order gives

$$
\int_0^\pi\left(\int_0^tf(s)ds\right)\overline{g(t)}dt=\int_0^\pi f(s)\overline{\left(\int_s^\pi g(t)dt\right)}ds.
$$

On the negative half-interval the corresponding calculation gives

$$
\int_{-\pi}^0\left(-\int_t^0f(s)ds\right)\overline{g(t)}dt=\int_{-\pi}^0f(s)\overline{\left(-\int_{-\pi}^sg(t)dt\right)}ds.
$$

These exchanges are justified by the [Fubini theorem](../../../../../fubini-s-theorem.md), since on a finite interval $L^2$ functions belong to $L^1$ and the absolute double integral is at most $\|f\|_1\|g\|_1$. Therefore

$$
(T^*g)(s)=\begin{cases}\displaystyle\int_s^\pi g(t)dt,&s>0,\\\displaystyle-\int_{-\pi}^sg(t)dt,&s<0.\end{cases}
$$

Adding $Tg$ gives $\int_0^\pi g$ on the positive half and $-\int_{-\pi}^0g$ on the negative half, exactly the prescribed $Ug$. Values at zero do not matter in $L^2$. Consequently

$$
\boxed{T+T^*=U.}
$$

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [6](../../6.md)
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
