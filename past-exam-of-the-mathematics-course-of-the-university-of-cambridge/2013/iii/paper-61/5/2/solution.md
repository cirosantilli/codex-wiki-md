<h1 id="5/2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

For the uniform [spline knots](../../../../../../spline-knot.md), translation reduces every degree-two basis function to a [quadratic cardinal B-spline](../../../../../../quadratic-cardinal-b-spline.md). From the [Cox-de Boor recurrence](../../../../../../cox-de-boor-recursion-formula.md), an order-three function takes the values

$$
N_{j,3}(j)=0,\quad N_{j,3}(j+1)=\frac12,\quad
N_{j,3}(j+2)=\frac12,\quad N_{j,3}(j+3)=0.
$$

At the prescribed site $x_i=i+2$, only $N_i$ and, when $i<n$, $N_{i+1}$ have nonzero values. Hence the [B-spline collocation matrix](../../../../../../b-spline-collocation-matrix.md) is

$$
A=\frac12(I+S),\qquad
S_{ij}=\begin{cases}1,&j=i+1,\\0,&\text{otherwise}.\end{cases}
$$

The shift satisfies $S^n=0$. A finite geometric expansion gives the exact inverse

$$
\boxed{A^{-1}=2\sum_{r=0}^{n-1}(-S)^r,\qquad
(A^{-1})_{ij}=
\begin{cases}
2(-1)^{j-i},&j\ge i,\\
0,&j<i.
\end{cases}}
$$

Its $i$th absolute row sum is $2(n-i+1)$, so $\|A^{-1}\|_{\ell^\infty}=2n$. Use the preceding bounds and the supplied stability constant $d_3=3$:

$$
\boxed{\frac{2n}{3}\le\|P_{\mathbf x}\|_{L^\infty}\le2n}.
$$

Thus the [linear growth of shifted quadratic spline interpolation](../../../../../../linear-growth-of-shifted-quadratic-spline-interpolation.md) is **$\Theta(n)$**, which in particular is $O(n)$. The lower bound, rather than the $O(n)$ upper bound alone, proves that these [spline interpolation operators](../../../../../../spline-interpolation-operator.md) are not uniformly bounded.

## ↑ Ancestors (11)

1. [2](../2.md)
2. [5](../../5.md)
3. [Paper 61](../../../paper-61-split.md)
4. [Iii](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
