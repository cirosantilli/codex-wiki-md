<h1 id="10e/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Here

$$
d_1(f,g)=\int_0^1|f(x)-g(x)|\,dx,
\qquad
d_\infty(f,g)=\max_{x\in[0,1]}|f(x)-g(x)|.
$$

The [L1 norm](../../../../../../l1-norm.md) and [uniform norm](../../../../../../supremum-norm.md) satisfy

$$
d_1(f,g)\le d_\infty(f,g),
$$

so the identity from the $d_\infty$ metric to the $d_1$ metric is one-Lipschitz and therefore continuous. The two metrics do not induce the same topology on all of $C[0,1]$. For

$$
f_n(x)=\max(1-nx,0),
$$

one has $d_1(f_n,0)=1/(2n)\to0$ but $d_\infty(f_n,0)=1$. Thus $d_1$ convergence need not imply uniform convergence.

A map $F:(X,d_X)\to(Y,d_Y)$ is [Lipschitz continuous](../../../../../../lipschitz-continuity.md) if there is $L<\infty$ such that

$$
d_Y(F(x),F(x'))\le Ld_X(x,x')
$$

for all $x,x'\in X$. Evaluation at $a\in[0,1]$ is one-Lipschitz because

$$
|f(a)-g(a)|\le d_\infty(f,g).
$$

Choose distinct $a_0,\ldots,a_n\in[0,1]$ and define

$$
T:\mathcal P_n\longrightarrow\mathbb R^{n+1},
\qquad
T(p)=(p(a_0),\ldots,p(a_n)).
$$

The [Vandermonde determinant](../../../../../../vandermonde-determinant.md) is nonzero, so $T$ is a bijection. It is one-Lipschitz for the two uniform metrics. If $\ell_i$ are the associated [Lagrange cardinal polynomials](../../../../../../lagrange-polynomial.md), then

$$
p(x)=\sum_{i=0}^np(a_i)\ell_i(x),
$$

and hence

$$
\|p-q\|_\infty
\le\left(\sum_{i=0}^n\|\ell_i\|_\infty\right)
\|T(p)-T(q)\|_\infty.
$$

Thus $T^{-1}$ is also Lipschitz.

Let $\widehat{\mathcal P}_n$ be the polynomials whose values lie in $[-1,1]$. Its image under $T$ lies in the bounded cube $[-1,1]^{n+1}$. It is closed: if $T(p_j)\to v$, then the Lipschitz inverse gives uniform convergence $p_j\to p=T^{-1}(v)$, and passing to the limit pointwise preserves $|p(x)|\le1$. By the [Heine-Borel theorem](../../../../../../heine-borel-theorem.md), $T(\widehat{\mathcal P}_n)$ is compact, and the continuous inverse carries compactness back to $\widehat{\mathcal P}_n$. Therefore

$$
\boxed{(\widehat{\mathcal P}_n,d_\infty)\text{ is compact}}.
$$

## ↑ Ancestors (11)

1. [I](../i.md)
2. [10E](../../10e.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ib](../../../split.md)
5. [2020](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
