<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Write the Bernstein basis as $p_{n,j}(x)=\binom njx^j(1-x)^{n-j}$, with $p_{n,j}=0$ for out-of-range indices. The [Bernstein polynomial](../../../../../bernstein-polynomial.md) is

$$
\boxed{B_n(f,x)=\sum_{j=0}^nf(j/n)p_{n,j}(x).}
$$

Differentiation and the identities $j\binom nj=n\binom{n-1}{j-1}$ and $(n-j)\binom nj=n\binom{n-1}j$ give $p_{n,j}'=n(p_{n-1,j-1}-p_{n-1,j})$. Shifting the first sum's index therefore yields

$$
\boxed{B_n'(f,x)=n\sum_{j=0}^{n-1}\bigl[f((j+1)/n)-f(j/n)\bigr]p_{n-1,j}(x).}
$$

Repeating this calculation takes another forward [finite difference](../../../../../finite-difference-split.md) of the coefficients and lowers the degree by one. Induction proves the [derivatives of Bernstein polynomials](../../../../../derivatives-of-bernstein-polynomials.md) formula

$$
\boxed{B_n^{(r)}(f,x)=(n)_r\sum_{j=0}^{n-r}\Delta_{1/n}^rf(j/n)p_{n-r,j}(x),\qquad (n)_r=\frac{n!}{(n-r)!}.}
$$

For $n>r$, define a continuous function on $[0,1]$ by

$$
\boxed{g_{n,r}(t)=(n)_r\Delta_{1/n}^rf\left(\frac{n-r}{n}t\right).}
$$

All sampled arguments lie in $[0,1]$, since the largest is $(n-r)t/n+r/n\le1$. At the degree-$(n-r)$ sampling point $t=j/(n-r)$, this gives exactly the coefficient $(n)_r\Delta_{1/n}^rf(j/n)$, and hence $\boxed{B_n^{(r)}f=B_{n-r}g_{n,r}}$. The rescaling is essential: the sampling meshes are $1/n$ and $1/(n-r)$, and the function $g_{n,r}$ depends on $n$. For $n=r$, the derivative is the constant $n!\Delta_{1/n}^nf(0)$, interpreted as a degree-zero [Bernstein polynomial](../../../../../bernstein-polynomial.md).

Now fix $r$ and assume $f\in C^r[0,1]$. The supplied uniform limit of normalized [finite differences](../../../../../finite-difference-split.md), together with $(n)_r/n^r\to1$ and [uniform continuity](../../../../../uniform-continuity.md) of $f^{(r)}$, shows that

$$
\|g_{n,r}-f^{(r)}\|_\infty\longrightarrow0:
\quad \frac{n-r}{n}t\longrightarrow t\quad\text{uniformly in }t.
$$

Positivity and $\sum_jp_{m,j}=1$ imply $\|B_mh\|_\infty\le\|h\|_\infty$. For completeness, if $X\sim\operatorname{Bin}(m,x)$ then $B_m(h,x)=\mathbb E[h(X/m)]$, and $\operatorname{Var}(X/m)=x(1-x)/m\le1/(4m)$. Splitting according to whether $|X/m-x|\le\delta$ and using [Chebyshev's inequality](../../../../../chebyshev-inequality.md) gives

$$
\|B_mh-h\|_\infty\le\omega(h,\delta)+\frac{\|h\|_\infty}{2m\delta^2}.
$$

First let $m\to\infty$ and then $\delta\to0$; this proves [uniform convergence](../../../../../uniform-convergence.md) for each continuous $h$. Finally,

$$
\|B_n^{(r)}f-f^{(r)}\|_\infty
\le\|B_{n-r}(g_{n,r}-f^{(r)})\|_\infty
+\|B_{n-r}f^{(r)}-f^{(r)}\|_\infty
\longrightarrow0.
$$

**Thus Bernstein polynomial derivatives converge uniformly to the corresponding derivatives of $f$, for each fixed $r$ with $f\in C^r[0,1]$.** Continuity of $f$ alone is sufficient for the definition of $B_n$, but not for this derivative conclusion.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 69](../../paper-69-split.md)
3. [Iii](../../split.md)
4. [2009](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
