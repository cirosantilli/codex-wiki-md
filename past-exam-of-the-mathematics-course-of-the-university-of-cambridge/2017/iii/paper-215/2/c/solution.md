<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Let $m\geq2$ be the number of states and put

$$
r=\max_{2\leq j\leq m}|\lambda_j|,\qquad
\boxed{\gamma_*=1-r,\qquad t_{\mathrm{rel}}=\gamma_*^{-1}.}
$$

The [absolute L2 spectral gap of a reversible Markov chain](../../../../../../absolute-l2-spectral-gap-of-a-reversible-markov-chain.md) is $\gamma_*$; in this question the [relaxation time](../../../../../../relaxation-time.md) means the [absolute relaxation time](../../../../../../absolute-relaxation-time.md). For a nonlazy [reversible Markov chain](../../../../../../reversible-markov-chain.md), it may differ from the reciprocal of the ordinary [spectral gap](../../../../../../spectral-gap.md) $1-\lambda_2$. For a finite [irreducible Markov chain](../../../../../../irreducible-markov-chain.md) that is an [aperiodic Markov chain](../../../../../../aperiodic-markov-chain.md), $r<1$.

For $r>0$, choose a real [eigenfunction](../../../../../../eigenfunction.md) $f$ whose [eigenvalue](../../../../../../eigenvalue.md) has modulus $r$, and an initial state $x$ maximizing $|f(x)|=\|f\|_\infty$. It has $\pi(f)=0$, and the definition of [total variation distance](../../../../../../total-variation-distance.md) implies

$$
r^t\|f\|_\infty=|P^tf(x)-\pi(f)|\leq2\|f\|_\infty\|P^t(x,\cdot)-\pi\|_{\mathrm{TV}}.
$$

This is the [eigenvalue lower bound for total variation mixing](../../../../../../eigenvalue-lower-bound-for-total-variation-mixing.md), $d(t)\geq r^t/2$. At $t=t_{\mathrm{mix}}(\varepsilon)$, for $0<\varepsilon<1/2$,

$$
t\geq\frac{\log(1/(2\varepsilon))}{-\log r}\geq\frac{r}{1-r}\log\frac1{2\varepsilon}.
$$

The second inequality follows from $-r\log r\leq1-r$, the supplied inequality with $x=1-r$. Since $r/(1-r)=t_{\mathrm{rel}}-1$,

$$
\boxed{(t_{\mathrm{rel}}-1)\log\frac1{2\varepsilon}\leq t_{\mathrm{mix}}(\varepsilon).}
$$

When $r=0$ the left side is zero, so no logarithm of zero is needed. For $\varepsilon\geq1/2$ the left side is nonpositive and the conclusion is automatic. A one-state chain has [mixing time](../../../../../../mixing-time-of-a-markov-chain.md) zero; with the convention $\gamma_*=1$ the bound is again trivial.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [2](../../2.md)
3. [Paper 215](../../../paper-215-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
