<h1 id="9h/solution">Solution</h1>

↑ **Parent:** [9H](../9h.md)

Write $u_k$ for the quantity denoted $\xi_k$ in the question, to distinguish it from the random-walk increments. Absorption at zero at time zero gives $u_0=1$, and starting at $N$ gives $u_N=0$. For $1\leq k\leq N-1$, condition on the first step and use independence of the remaining increments. That step contributes one factor of $s$, so the [discounted gambler's ruin hitting probability](../../../../../discounted-gambler-s-ruin-hitting-probability.md) satisfies

$$
\boxed{u_k=s(pu_{k+1}+qu_{k-1}),\qquad u_0=1,\quad u_N=0.}
$$

The absorption time is finite almost surely: in each block of $N$ steps there is a probability bounded below by a positive constant of reaching a boundary by successive steps in one direction.

Trying $u_k=r^k$ gives $psr^2-r+qs=0$, with roots

$$
r_\pm=\frac{1\pm\sqrt{1-4pqs^2}}{2ps}.
$$

They are positive and distinct because $4pq\leq1$ and $0<s<1$. Hence the general solution is $Ar_+^k+Br_-^k$. Enforcing both boundary values gives

$$
\boxed{\xi_k=u_k=\frac{r_+^Nr_-^k-r_-^Nr_+^k}{r_+^N-r_-^N},\qquad0\leq k\leq N.}
$$

This includes the unbiased walk without a special limiting case, since the discount keeps the roots distinct. For uniqueness, a difference of two solutions has zero boundary values and its largest absolute value $M$ satisfies $M\leq sM$ if attained in the interior. Since $s<1$, $M=0$.

## ↑ Ancestors (10)

1. [9H](../9h.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ib](../../split.md)
4. [2009](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
