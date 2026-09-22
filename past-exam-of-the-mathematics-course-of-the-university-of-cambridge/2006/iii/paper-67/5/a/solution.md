<h1 id="5/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Let $C_k(u)$ be the order-$k$ [Cardinal B-spline](../../../../../../cardinal-b-spline.md) supported on $[0,k]$. The [Cox-de Boor recurrence](../../../../../../cox-de-boor-recursion-formula.md) on unit-spaced knots reads

$$
C_k(u)=\frac{u}{k-1}C_{k-1}(u)+\frac{k-u}{k-1}C_{k-1}(u-1),\qquad k\geq2.
$$

Start with $C_1=\mathbf1_{[0,1)}$. The order-two hat satisfies $C_2(1)=1$ and vanishes at its [support](../../../../../../support.md) endpoints. Substituting these values into the recurrence gives $C_3(1)=C_3(2)=1/2$ and then

$$
C_4(1)=\frac16,\qquad C_4(2)=\frac23,\qquad C_4(3)=\frac16.
$$

The continuous cubic [spline](../../../../../../spline-mathematics.md) is zero at $0,4$ and outside its [support](../../../../../../support.md). Since $N_j(t)=C_4(t-j)$ and $x_i=i+2$, this yields the [midpoint cubic spline collocation](../../../../../../midpoint-cubic-spline-collocation.md) values

$$
\boxed{N_j(x_i)=\begin{cases}
2/3,&j=i,\\
1/6,&j=i-1\text{ or }j=i+1,\\
0,&|i-j|\geq2.
\end{cases}}
$$

Only indices $1\leq j\leq n$ are retained. In particular no nonexistent [spline](../../../../../../spline-mathematics.md) is added to an endpoint row.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [5](../../5.md)
3. [Paper 67](../../../paper-67-split.md)
4. [Iii](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
