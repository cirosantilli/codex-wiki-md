<h1 id="5/2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

For unit-spaced knots, the [quadratic cardinal B-spline](../../../../../../quadratic-cardinal-b-spline.md) with support $[i,i+3]$ is $N_i(t)=B(t-i)$, where the [Cox-de Boor recurrence](../../../../../../cox-de-boor-recursion-formula.md) gives

$$
B(u)=\begin{cases}u^2/2,&0\le u\le1,\\-u^2+3u-3/2,&1\le u\le2,\\(3-u)^2/2,&2\le u\le3,\\0,&\text{otherwise}.\end{cases}
$$

In particular $B(1)=B(2)=1/2$ and $B(0)=B(3)=0$. At $x_i=i+2$, the only nonzero entries in row $i$ are $A_{ii}=1/2$ and, if $i<n$, $A_{i,i+1}=1/2$. Write $U$ for the upper shift matrix, with ones immediately above its diagonal. Then

$$
A_x=\tfrac12(I+U),\qquad A_x^{-1}=2\sum_{r=0}^{n-1}(-U)^r,
$$

since $U^n=0$. Thus $(A_x^{-1})_{ij}=2(-1)^{j-i}$ for $j\ge i$, and zero otherwise. The largest absolute row sum is the first, giving $\|A_x^{-1}\|_{\ell_\infty}=2n$.

Using (1) and the permitted $d_3=3$ proves the stronger [linear growth of shifted quadratic spline interpolation](../../../../../../linear-growth-of-shifted-quadratic-spline-interpolation.md) estimate

$$
\boxed{\frac{2n}{3}\le\|P_x\|\le2n.}
$$

Therefore **$\|P_x\|=\Theta(n)$ and is not uniformly bounded**. An $O(n)$ upper bound alone would not imply unboundedness; the lower bound is essential.

## ↑ Ancestors (11)

1. [2](../2.md)
2. [5](../../5.md)
3. [Paper 62](../../../paper-62-split.md)
4. [Iii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
