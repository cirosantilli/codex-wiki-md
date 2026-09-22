<h1 id="2/c/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Let the [energy of a flow](../../../../../../../energy-of-a-flow.md) be $\mathcal E(\theta)=\sum_e\theta(e)^2$, with each unoriented edge counted once. Expanding as in part (i), dropping orientation signs, and summing over common edges gives

$$
\mathbb E\mathcal E(\theta_\omega)
\leq\mathbb E_{\mu\times\mu}[N p^{-N}]
\leq C\sum_{n\geq1}n\left(\frac\zeta p\right)^n<\infty,
$$

uniformly in $r$.

Part (i), $\mathbb EX_r=1$, and the [Paley-Zygmund inequality](../../../../../../../paley-zygmund-inequality.md) give a constant $a>0$ such that $\mathbb P(X_r>1/2)\geq a$ for every $r$. The preceding uniform expectation bound and [Markov inequality](../../../../../../../markov-inequality.md) allow a constant $L$ such that

$$
\mathbb P\bigl(X_r>1/2, \mathcal E(\theta_\omega)\leq L\bigr)\geq a/2.
$$

On this event, $\theta_\omega/X_r$ is a unit open flow from $o$ to $z_r$ with energy at most $4L$.

The events that there is such a bounded-energy unit flow from $o$ out of $B(o,r)$ are decreasing in $r$. Their intersection still has probability at least $a/2$. A diagonal compactness argument produces on this intersection a unit flow from $o$ to infinity, supported on its open cluster, with finite energy. The [finite-energy flow criterion for transience](../../../../../../../finite-energy-flow-criterion-for-transience.md) makes that open cluster transient.

Thus a transient open cluster exists with positive probability. This existence event is a [tail event](../../../../../../../tail-event.md): changing finitely many edges cannot destroy transience in every infinite component, because transience is invariant under finite graph modifications. The [Kolmogorov zero-one law](../../../../../../../kolmogorov-s-zero-one-law.md) upgrades its probability to one.

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [C](../../c.md)
3. [2](../../../2.md)
4. [Paper 212](../../../../paper-212-split.md)
5. [Iii](../../../../split.md)
6. [2026](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
