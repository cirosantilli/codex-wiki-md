<h1 id="1/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

**No: the Lebesgue measure can decrease when separate components of the Minkowski sum merge.** A one-dimensional example is enough to disprove the assertion in general. Take

$$
A=(0,1/10)\cup(10,101/10),\qquad B=(0,1/10)\cup(2,21/10).
$$

The [Minkowski sum](../../../../../../minkowski-addition.md) $A+tB$ consists of four [open intervals](../../../../../../open-interval.md), with left endpoints $0,10,2t,10+2t$ and common length $(1+t)/10$. At $t=4$ the four [open intervals](../../../../../../open-interval.md) are disjoint, so

$$
\lambda_1(A+4B)=4\cdot\frac12=2.
$$

At $t=5$ the middle two [open intervals](../../../../../../open-interval.md) coincide and the remaining three are disjoint, so

$$
\boxed{\lambda_1(A+5B)=3\cdot\frac35=\frac95<2=\lambda_1(A+4B).}
$$

For a counterexample in any prescribed dimension $n>1$, take [Cartesian products](../../../../../../cartesian-product.md) of these [open sets](../../../../../../open-set.md) with $(0,1)$ in the remaining coordinates. Compare $t_2=5$ with $t_1=5-\delta$, where $\delta=\delta_n>0$ is sufficiently small, and choose the interval width $\varepsilon>0$ so small that $6\varepsilon<2\delta$. The four intervals remain disjoint at $t_1$, giving

$$
\lambda_n(A_n+t_1B_n)=4\varepsilon(6-\delta)^n,\qquad\lambda_n(A_n+5B_n)=3\varepsilon6^n.
$$

Choosing $(1-\delta/6)^n>3/4$ makes the latter smaller. Here $A_n=((0,\varepsilon)\cup(10,10+\varepsilon))\times(0,1)^{n-1}$ and $B_n=((0,\varepsilon)\cup(2,2+\varepsilon))\times(0,1)^{n-1}$. The [Brunn–Minkowski inequality](../../../../../../brunn-minkowski-theorem.md) gives a lower bound at each value of $t$; it does not give the claimed monotonicity for arbitrary [open sets](../../../../../../open-set.md).

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [1](../../1.md)
3. [Paper 112](../../../paper-112-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
