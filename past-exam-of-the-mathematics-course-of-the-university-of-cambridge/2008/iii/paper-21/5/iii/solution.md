<h1 id="5/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Let $g$ be the [geometric genus](../../../../../../geometric-genus.md) of $X$. Choose an integer $N\ge2g+1$. For each prescribed point $x_i$, both $Nx_i$ and $(N-1)x_i$ have degree greater than $2g-2$, so their complementary [canonical divisors](../../../../../../canonical-divisor.md) have negative degree and their complementary [Riemann-Roch spaces](../../../../../../riemann-roch-space.md) vanish. The [Riemann-Roch theorem](../../../../../../riemann-roch-theorem.md) therefore gives

$$
\ell(Nx_i)=N+1-g,\qquad\ell((N-1)x_i)=N-g.
$$

Choose $f_i\in L(Nx_i)\setminus L((N-1)x_i)$. This is possible because the two dimensions differ by one. Such a [rational function](../../../../../../rational-function.md) has its only pole at $x_i$, and its pole order there is exactly $N$. Set $f=\sum_{i=1}^m f_i$.

At $x_i$ all terms except $f_i$ are regular. In a local parameter, the term of order $-N$ in $f_i$ has a nonzero coefficient, and none of the other terms has a negative-power term. Hence that coefficient cannot cancel. Away from the prescribed points every summand is regular. We obtain the stronger conclusion

$$
\boxed{(f)_\infty=N\sum_{i=1}^m x_i.}
$$

Thus **$f$ is regular on $U$ and has a pole at every $x_i$**. This [rational functions with prescribed poles](../../../../../../rational-functions-with-prescribed-poles.md) construction works in every characteristic and does not require a generic-coefficient choice. If the prescribed list is empty, a constant function meets the vacuous requirements.

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [5](../../5.md)
3. [Paper 21](../../../paper-21-split.md)
4. [Iii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
