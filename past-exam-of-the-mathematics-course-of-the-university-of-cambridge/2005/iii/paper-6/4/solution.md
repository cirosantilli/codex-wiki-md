<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

We construct the finite evaluation representation explicitly by [Lagrange interpolation](../../../../../lagrange-polynomial.md). This supplies all the [polynomial](../../../../../polynomial-split.md) facts needed for the bound.

Define the [Chebyshev polynomial](../../../../../chebyshev-polynomial.md) by $T_0=1,T_1=x$ and

$$
T_{m+1}(x)=2xT_m(x)-T_{m-1}(x).
$$

Induction shows that $T_m$ has degree $m$; the [cosine](../../../../../cosine.md) addition identity also proves $T_m(\cos\theta)=\cos(m\theta)$. Therefore $\|T_n\|_{[-1,1]}=1$, and $T_n(-x)=(-1)^nT_n(x)$ follows from the recurrence. The case $n=0$ is immediate, since both $P$ and $T_0$ are constant.

For $n\geq1$, choose the descending extremal nodes

$$
x_j=\cos(j\pi/n),\qquad 0\leq j\leq n,
$$

so $T_n(x_j)=(-1)^j$. Define the fundamental interpolation polynomials

$$
\ell_j(t)=\prod_{k\ne j}\frac{t-x_k}{x_j-x_k}.
$$

They satisfy $\ell_j(x_k)=\delta_{jk}$. Consequently

$$
\boxed{P(t)=\sum_{j=0}^nP(x_j)\ell_j(t)}
$$

for every [polynomial](../../../../../polynomial-split.md) of degree at most $n$: the difference has degree at most $n$ and vanishes at the $n+1$ distinct nodes, so it is zero. The root count used here follows by successively factoring $(t-x_j)$ from a [polynomial](../../../../../polynomial-split.md) having such a root; a nonzero degree-$n$ [polynomial](../../../../../polynomial-split.md) cannot have more than $n$ distinct roots. Thus the interpolation identity has been proved.

If $u>1$, every numerator factor in $\ell_j(u)$ is positive, while exactly $j$ denominator factors are negative. Hence $\operatorname{sgn}\ell_j(u)=(-1)^j$. Applying interpolation to $T_n$ itself gives

$$
\sum_{j=0}^n|\ell_j(u)|=\sum_{j=0}^n(-1)^j\ell_j(u)=T_n(u)>0.
$$

Putting $M=\sup_{[-1,1]}|P|$ in the interpolation formula yields

$$
|P(u)|\leq\sum_{j=0}^n|P(x_j)||\ell_j(u)|\leq M T_n(u).
$$

For $u<-1$, apply the proved positive-side inequality to $Q(t)=P(-t)$ at $-u>1$, and use the parity identity. The result is

$$
\boxed{|P(u)|\leq\|P\|_{[-1,1]}|T_n(u)|,\qquad u\notin[-1,1].}
$$

This is sharp, with equality for $P=T_n$ or its scalar multiples.

In functional terms, the evaluation map $E_u:P\mapsto P(u)$ on the normed [polynomial](../../../../../polynomial-split.md) space has $\|E_u\|=|T_n(u)|$: the inequality gives the upper bound and $T_n$ attains it. For $u>1$, its normalized version has the exact representation

$$
\frac{E_u(P)}{T_n(u)}=\sum_{j=0}^n\lambda_jP(x_j),
\qquad\lambda_j=\frac{\ell_j(u)}{T_n(u)},\quad
\sum_{j=0}^n|\lambda_j|=1.
$$

Thus [Chebyshev interpolation represents external evaluation](../../../../../chebyshev-interpolation-represents-external-evaluation.md) using $n+1$ nodes. The necessary finite representation and its [norm](../../../../../norm.md) are derived directly, so no convex-hull theorem is being invoked without proof.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 6](../../paper-6-split.md)
3. [Iii](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
