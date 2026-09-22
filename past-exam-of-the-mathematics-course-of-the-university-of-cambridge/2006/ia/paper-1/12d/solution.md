<h1 id="12d/solution">Solution</h1>

↑ **Parent:** [12D](../12d.md)

For a bounded function on an interval $I$, write $\omega_I(f)=\sup_I f-\inf_I f$ for its [oscillation of a function on an interval](../../../../../oscillation-of-a-function-on-an-interval.md). For a partition $P$, the difference between its [upper Darboux sum](../../../../../upper-darboux-sum.md) and [lower Darboux sum](../../../../../lower-darboux-sum.md) is $\sum_{I\in P}|I|\omega_I(f)$. The [Riemann integrability criterion](../../../../../riemann-integrability-criterion.md) says that this can be made arbitrarily small.

Since $\omega_I(f_1+f_2)\le\omega_I(f_1)+\omega_I(f_2)$, choose good partitions for the two functions and take their common refinement. [Darboux sum refinement monotonicity](../../../../../darboux-sum-refinement-monotonicity.md) makes both oscillation sums small on this refinement, so their sum is [Riemann integrable](../../../../../riemann-integrable-function.md). The same argument handles differences and scalar multiples.

Both $t\mapsto\max(t,0)$ and $t\mapsto|t|$ are [Lipschitz continuous](../../../../../lipschitz-continuity.md) with constant one. Thus $\omega_I(f^+)\le\omega_I(f)$ and $\omega_I(|f|)\le\omega_I(f)$. This calculation shows that [Lipschitz composition preserves Riemann integrability](../../../../../lipschitz-composition-preserves-riemann-integrability.md), so the [positive part](../../../../../positive-part-of-a-real-valued-function.md) and the [absolute value](../../../../../absolute-value.md) are integrable.

The converse for the absolute value is false. Define $f=1$ on [rational numbers](../../../../../rational-number.md) and $f=-1$ on [irrational numbers](../../../../../irrational-number.md). Then $|f|=1$ is integrable, but every interval has supremum one and infimum minus one, so every Darboux difference for $f$ is $2(b-a)$. Hence $f$ is not [Riemann integrable](../../../../../riemann-integrable-function.md).

Finally,

$$
\boxed{\max(f_1,f_2)=\frac{f_1+f_2+|f_1-f_2|}{2}}
$$

is integrable by the closure properties just proved. This establishes that [Riemann integrability is closed under addition and maximum](../../../../../riemann-integrability-is-closed-under-addition-and-maximum.md).

A countable supremum can fail, even for a uniformly bounded family. Enumerate the rational points of $[a,b]$ as $q_1,q_2,\ldots$ and set $f_n=1_{\{q_n\}}$. Each singleton [indicator function](../../../../../indicator-function.md) is [Riemann integrable](../../../../../riemann-integrable-function.md) with integral zero: isolate its single nonzero point in intervals of arbitrarily small total length. But

$$
\boxed{\sup_n f_n=1_{\mathbb Q\cap[a,b]}}
$$

is the nonintegrable [Dirichlet function](../../../../../dirichlet-function.md). This proves that a [pointwise supremum need not preserve Riemann integrability](../../../../../pointwise-supremum-need-not-preserve-riemann-integrability.md).

## ↑ Ancestors (10)

1. [12D](../12d.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ia](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
