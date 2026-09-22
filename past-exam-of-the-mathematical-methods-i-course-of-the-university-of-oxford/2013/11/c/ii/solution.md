<h1 id="11/c/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Setting $\mathbf b=\mathbf a$ in [i](../i.md) removes the [cross product](../../../../../cross-product.md) term and gives $\sigma(\mathbf a)^2=(\mathbf a\cdot\mathbf a)I$. Repeated multiplication therefore yields, for nonnegative integers $m$,

$$
\boxed{\sigma(\mathbf a)^{2m}=(\mathbf a\cdot\mathbf a)^mI,\qquad
\sigma(\mathbf a)^{2m+1}=(\mathbf a\cdot\mathbf a)^m\sigma(\mathbf a).}
$$

The zeroth power is $I$. If negative powers are intended, they require $\mathbf a\cdot\mathbf a\ne0$, and the same parity formulas then follow from $\sigma(\mathbf a)^{-1}=\sigma(\mathbf a)/(\mathbf a\cdot\mathbf a)$. Every nonzero real vector meets that condition; a nonzero complex null vector need not. For example, $\mathbf a=(1,i,0)$ has $\sigma(\mathbf a)^2=0$ and no inverse.

For a real [unit vector](../../../../../unit-vector.md) $\hat{\mathbf n}$, let $S=\sigma(\hat{\mathbf n})$. Then $S^2=I$, so even powers are $I$ and odd powers are $S$. Split the absolutely convergent [matrix exponential](../../../../../matrix-exponential.md) into its even and odd series:

$$
\begin{aligned}
e^{i\theta S}
&=I\sum_{m=0}^\infty\frac{(-1)^m\theta^{2m}}{(2m)!}
+iS\sum_{m=0}^\infty\frac{(-1)^m\theta^{2m+1}}{(2m+1)!}\\
&=\boxed{\cos\theta\,I+i\sin\theta\,\sigma(\hat{\mathbf n})}.
\end{aligned}
$$

The result holds for every real $\theta$, not merely small angles. Its two scalar series are the ordinary cosine and sine series.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [C](../../c.md)
3. [11](../../../11.md)
4. [2013](../../../../2013-split.md)
5. [Past exam of the mathematical methods I course of the University of Oxford](../../../../split.md)
6. [Mathematical methods I course of the University of Oxford](../../../../../mathematical-methods-i-course-of-the-university-of-oxford.md)
7. [Year 1 of the physics course of the University of Oxford](../../../../../year-1-of-the-physics-course-of-the-university-of-oxford.md)
8. [Physics course of the University of Oxford](../../../../../physics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
