<h1 id="5/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

Take complex-valued functions. Pointwise multiplication is associative and commutative, with identity the constant function $1$, whose norm is one. The [product rule](../../../../../../product-rule.md) gives

$$
\|fg\|_\infty+\|(fg)'\|_\infty
\leq\|f\|_\infty\|g\|_\infty+\|f'\|_\infty\|g\|_\infty+\|f\|_\infty\|g'\|_\infty
\leq\|f\|\|g\|.
$$

To prove completeness, let $(f_n)$ be a [Cauchy sequence](../../../../../../cauchy-sequence.md) in this norm. The functions and their derivatives converge uniformly to [continuous functions](../../../../../../continuous-function.md) $f,g$. Passing to the limit in $f_n(t)-f_n(0)=\int_0^tf_n'(s)\,ds$ gives $f(t)-f(0)=\int_0^tg(s)\,ds$. The [fundamental theorem of calculus](../../../../../../fundamental-theorem-of-calculus.md) yields $f'=g$, including the one-sided endpoint derivatives. Thus $f\in C^1[0,1]$ and $f_n\to f$ in the stated norm. Consequently **$A$ is a unital commutative [Banach algebra](../../../../../../banach-algebra-split.md)**.

Let $u(t)=t$. If $\lambda\notin[0,1]$, then $(u-\lambda1)^{-1}(t)=1/(t-\lambda)$ belongs to $C^1[0,1]$. If $\lambda\in[0,1]$, the function $u-\lambda1$ vanishes somewhere and cannot have a pointwise inverse. Thus $\sigma_A(u)=[0,1]$. Every [character of an algebra](../../../../../../character-of-an-algebra.md) satisfies $\phi(u)=t_0$ for some $t_0\in[0,1]$, by part (d), and therefore $\phi(p(u))=p(t_0)$ for every [polynomial](../../../../../../polynomial-split.md) $p$.

[Polynomials](../../../../../../polynomial-split.md) are dense in this stronger norm, not just the [supremum norm](../../../../../../supremum-norm.md). By the [Weierstrass approximation theorem](../../../../../../weierstrass-approximation-theorem.md), approximate the real and imaginary parts of $f'$ uniformly by [polynomials](../../../../../../polynomial-split.md), combining them into $q_n\to f'$. Put $p_n(t)=f(0)+\int_0^tq_n(s)\,ds$. Then $p_n$ is a [polynomial](../../../../../../polynomial-split.md) and

$$
\|p_n'-f'\|_\infty\to0,\qquad\|p_n-f\|_\infty\leq\|q_n-f'\|_\infty\to0.
$$

[Continuity](../../../../../../continuous-function.md) of the [algebra character](../../../../../../character-of-an-algebra.md) now gives $\phi(f)=\lim p_n(t_0)=f(t_0)$. Conversely each point evaluation is a continuous [algebra character](../../../../../../character-of-an-algebra.md). Hence the [character space of C1 on a compact interval](../../../../../../character-space-of-c1-on-a-compact-interval.md) consists exactly of the evaluation functionals, and part (c) gives

$$
\boxed{\mathcal M_A=\{M_t:t\in[0,1]\},\qquad M_t=\{f\in C^1[0,1]:f(t)=0\}.}
$$

Distinct points give distinct [maximal ideals](../../../../../../maximal-ideal.md), since the coordinate function separates them.

## ↑ Ancestors (11)

1. [E](../e.md)
2. [5](../../5.md)
3. [Paper 10](../../../paper-10-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
