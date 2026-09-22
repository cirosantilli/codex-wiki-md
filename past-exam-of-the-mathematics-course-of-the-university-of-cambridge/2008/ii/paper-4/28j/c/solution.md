<h1 id="28j/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Assume the riskless gross return $q=1+r>0$, as required by the positive-wealth model, and a finite moment $m_b=\mathbb EX_0^b$. Define

$$
C(\theta)=\mathbb E[\theta X_0+(1-\theta)q]^b,\qquad
C_* =\max_{\alpha\leq\theta\leq1}C(\theta).
$$

This maximum exists: the control interval is compact and dominated convergence gives continuity, using the integrable bound $(X_0+q)^b\leq X_0^b+q^b$ for $0<b\leq1$.

The terminal value is $V_N(w)=U(w)$. If $V_{n+1}(w)=a_{n+1}U(w)$, the [Bellman equation](../../../../../../bellman-equation.md) and [independence](../../../../../../independent-random-variables.md) of the next return give

$$
V_n(w)=\max_{\theta\in[\alpha,1]}\mathbb E V_{n+1}(w[\theta X_n+(1-\theta)q])
=a_{n+1}U(w)C_*.
$$

Backward induction therefore proves

$$
\boxed{V_n(w)=a_nU(w),\qquad a_n=C_*^{N-n}.}
$$

Any maximizing proportion can be used each day; allowing adapted choices cannot exceed the Bellman bound. For $\alpha=1$, $C_*=m_b$, exactly agreeing with part (b). If $m_b=\infty$ and at least one day remains, the allowed choice $\theta=1$ already gives infinite expected utility, so the value is infinite rather than a finite coefficient. This is the necessary moment qualification to the finite optimization formula.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [28J](../../28j.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
