<h1 id="5/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Denote the density process by $L_t=\exp(M_t-[M]_t/2)$. The given identities for all $A\in\mathcal F_s$ imply

$$
\mathbb E_{\mathbb P}(L_t\mid\mathcal F_s)=L_s,\qquad \mathbb E_{\mathbb P}L_t=1.
$$

Thus $L$ is a strictly positive true [martingale](../../../../../../martingale-split.md), not merely a [local martingale](../../../../../../local-martingale.md). The [Itô formula](../../../../../../ito-s-lemma.md) gives $dL=L\,dM$, and hence

$$
d[L,X]_t=L_t\,d[M,X]_t.
$$

First work with the zero-starting corrected increments $U=X-X_0-[X,M]$. Integration by parts gives

$$
\begin{aligned}
d(LU)&=U\,dL+L\,dU+d[L,U]\\
&=LU\,dM+L\,dX-L\,d[X,M]+L\,d[M,X]\\
&=LU\,dM+L\,dX.
\end{aligned}
$$

The finite-variation bracket has zero [quadratic covariation](../../../../../../quadratic-covariation.md) with $L$, so no other term appears. Thus $LU$ is a P-local [martingale](../../../../../../martingale-split.md).

To justify the change of measure, stop $U$ at $\tau_n=\inf\{t:|U_t|\ge n\}$, with optional further localization if needed. The product $L_tU_{t\wedge\tau_n}$ remains a P-local [martingale](../../../../../../martingale-split.md): before the [stopping time](../../../../../../stopping-time.md) the cancellation above applies, and afterwards only its bounded constant factor multiplies $dL$. Its absolute value is bounded by $nL_t$. On a finite horizon the stopped values of $L$ are [uniformly integrable](../../../../../../uniform-integrability.md), so Q1(c) upgrades this product to a true [martingale](../../../../../../martingale-split.md). The [Bayes formula for conditional expectation](../../../../../../bayes-formula-for-conditional-expectation.md) now gives

$$
\mathbb E_{\mathbb Q}(U_{t\wedge\tau_n}\mid\mathcal F_s)
=\frac{\mathbb E_{\mathbb P}(L_tU_{t\wedge\tau_n}\mid\mathcal F_s)}{L_s}
=U_{s\wedge\tau_n}.
$$

Finite-horizon equivalence of the measures transfers the [localizing sequence](../../../../../../localizing-sequence.md) to Q. Therefore $U$ is a continuous Q-local [martingale](../../../../../../martingale-split.md). If $X_0\in L^1(\mathbb Q)$, adding its constant-in-time process proves

$$
\boxed{\widetilde X=X-[X,M]\text{ is a continuous Q-local martingale}.}
$$

This proves the [Girsanov theorem](../../../../../../girsanov-theorem.md) assertion under the usual zero or deterministic initial-value convention. More generally the normalization $M_0=0$ makes $L_0=1$, so P and Q agree on $\mathcal F_0$ and the required initial integrability is automatic.

There is a literal initial-integrability qualification if neither convention is imposed. On positive integers let $P(n)=2^{-n}$, $Q(n)=c/n^2$, with $c=(\sum_{n\ge1}n^{-2})^{-1}$, and let every [filtration](../../../../../../filtration-probability-theory.md) equal the full [sigma-algebra](../../../../../../sigma-algebra.md). Constant processes $M_t=\log(c2^n/n^2)$ and $X_t=n$ are P-martingales, and $e^{M_t}$ is precisely the prescribed density. But $\mathbb E_Q|X_0|=\infty$ and $[X,M]=0$, so the asserted Q-local [martingale](../../../../../../martingale-split.md) cannot have an integrable initial value. This is why [initial integrability under a density change](../../../../../../initial-integrability-under-a-density-change.md) is part of the precise formulation.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [5](../../5.md)
3. [Paper 30](../../../paper-30-split.md)
4. [Iii](../../../split.md)
5. [2004](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
