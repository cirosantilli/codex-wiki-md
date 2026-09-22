<h1 id="8g/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The [eigenvalue](../../../../../../eigenvalue.md) equation $D_rf=\lambda f$ is

$$
f(x+r)=(1+\lambda)f(x).
$$

If $\lambda=-1$, this forces $f(x+r)=0$ for every $x$, hence $f=0$, so $-1$ is not an [eigenvalue](../../../../../../eigenvalue.md). If $c=1+\lambda\ne0$, choose arbitrary values on representatives of the cosets of $r\mathbb Z$ and extend by

$$
f(t+kr)=c^kf(t),
\qquad k\in\mathbb Z.
$$

This produces nonzero eigenfunctions. Choosing [functions](../../../../../../function-split.md) supported on distinct cosets gives infinitely many linearly independent eigenfunctions. Therefore

$$
\boxed{\operatorname{spec}_{\rm point}(D_r)=\mathbb R\setminus\{-1\}},
$$

and every eigenspace is infinite-dimensional.

Direct expansion gives

$$
D_rD_sf(x)=f(x+r+s)-f(x+r)-f(x+s)+f(x),
$$

which is symmetric in $r,s$. Hence

$$
\boxed{D_rD_s=D_sD_r}.
$$

Suppose a degree-$n$ [polynomial](../../../../../../polynomial-split.md) $p$ were a sum of $n$ periodic [functions](../../../../../../function-split.md),

$$
p=f_1+\cdots+f_n,
\qquad D_{r_i}f_i=0,
\quad r_i\ne0.
$$

Apply the commuting product $D_{r_1}\cdots D_{r_n}$. Every term on the right is killed by its corresponding factor, whereas for leading coefficient $a_n$ the [mixed finite difference of a polynomial](../../../../../../mixed-finite-difference-of-a-polynomial.md) gives

$$
D_{r_1}\cdots D_{r_n}p
=n!a_n\prod_{i=1}^nr_i\ne0.
$$

This contradiction proves

$$
\boxed{p\text{ cannot be a sum of }n\text{ periodic functions}}.
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [8G](../../8g.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ib](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
