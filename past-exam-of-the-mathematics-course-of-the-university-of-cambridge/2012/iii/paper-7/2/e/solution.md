<h1 id="2/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

For $0<r<1$, $r\log r<0$. The printed upper bound is negative whenever $\Omega\ne0$, so it cannot bound a nonnegative difference. **The correct small-distance modulus is $r\log(1/r)$**, and the radius in the hint must also be positive.

Write $h=|x_1-x_2|\leq e^{-1}$, $x_3=(x_1+x_2)/2$, and $M=h\log(1/h)$. Then $h\leq M\leq e^{-1}$. Denote the [planar vorticity velocity kernel](../../../../../../planar-vorticity-velocity-kernel.md) by $K$. It satisfies $|K(z)|\leq C/|z|$ and $|DK(z)|\leq C/|z|^2$. Split the [integral](../../../../../../integral.md) at radii $M$ and $1$ about $x_3$.

On $|y-x_3|\geq1$, every point of the segment joining $x_1$ and $x_2$ remains at least $|y-x_3|-h/2\geq(1-h/2)|y-x_3|$ from $y$. The [mean value theorem](../../../../../../mean-value-theorem.md) bounds the kernel difference by $Ch/|y-x_3|^2$, giving a contribution at most $Ch\|\Omega\|_1$.

On $M\leq|y-x_3|\leq1$, the same estimate holds because $h/2\leq M/2$. [Polar integration](../../../../../../polar-coordinates.md) gives

$$
\int_{M\leq|y-x_3|\leq1}
|K(x_1-y)-K(x_2-y)|\,|\Omega(y)|\,dy
\leq Ch\|\Omega\|_\infty\int_M^1\frac{dr}{r}
\leq Ch\log(1/h)\|\Omega\|_\infty.
$$

Here $\log(1/M)\leq\log(1/h)$ because $M\geq h$.

On $|y-x_3|<M$, use the sum of the two kernel magnitudes instead of their derivatives. This disk lies inside a disk of radius $M+h/2\leq3M/2$ about either $x_i$. Hence its contribution is bounded by $CM\|\Omega\|_\infty$. Combining the three regions yields

$$
\boxed{|U[\Omega](x_1)-U[\Omega](x_2)|
\leq C(\|\Omega\|_1+\|\Omega\|_\infty)
h\log(1/h),\quad 0<h\leq e^{-1}.}
$$

At coincident points the difference is zero. At larger distances use the boundedness from part (d). A convenient global [log-Lipschitz modulus](../../../../../../log-lipschitz-modulus.md) is

$$
\mu(r)=
\begin{cases}r(1-\log r),&0<r\leq1,\\1,&r\geq1,\end{cases}
\qquad \mu(0)=0,
$$

giving $|U[\Omega](x)-U[\Omega](y)|\leq C(\|\Omega\|_1+\|\Omega\|_\infty)\mu(|x-y|)$. This is positive, continuous and nondecreasing. It also proves [continuity](../../../../../../continuous-function.md) of $U[\Omega]$.

## ↑ Ancestors (11)

1. [E](../e.md)
2. [2](../../2.md)
3. [Paper 7](../../../paper-7-split.md)
4. [Iii](../../../split.md)
5. [2012](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
