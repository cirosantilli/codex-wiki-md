<h1 id="6/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Set $u_0=\alpha/\beta$ and use the accelerated grid time $j/n$. At population $k=nu_0+\sqrt n\,x$, the fluctuation increment is $h_n=n^{-1/2}$, $-h_n$, or zero. Its first and second conditional moments, multiplied by $n$, are

$$
b_n(x)=n\mathbb E(\Delta X^n\mid x)
=\sqrt n\,(p_k-q_k)=-\alpha x-\frac\beta{\sqrt n}x^2,
$$



$$
a_n(x)=n\mathbb E((\Delta X^n)^2\mid x)
=p_k+q_k=\frac{2\alpha^2}{\beta}
+\frac{3\alpha}{\sqrt n}x+\frac\beta n x^2.
$$

Thus $b_n\to b(x)=-\alpha x$ and $a_n\to a=2\alpha^2/\beta$, uniformly on every compact set. The centered conditional variance has the same limit, since the squared conditional mean contributes only $b_n(x)^2/n$.

Here is the [diffusion approximation theorem](../../../../../../diffusion-approximation-theorem.md) being applied. For Markov chains sampled with time step $1/n$, suppose the first and second conditional increment moments multiplied by $n$ converge uniformly on compact sets to continuous coefficients $b,a$; the large-jump conditional second moments satisfy the local Lindeberg condition; the initial laws converge; compact containment holds on finite time intervals; and the limiting [martingale problem](../../../../../../martingale-problem.md) is well-posed and nonexplosive. Then the interpolated chains converge weakly, uniformly on finite time intervals, to that problem's continuous solution. The step versions converge in the [Skorokhod J1 topology](../../../../../../skorokhod-j1-topology.md). Local moment bounds supply the stopped-process tightness, and the limiting test-function identities identify every subsequential limit by the [martingale problem](../../../../../../martingale-problem.md).

We verify the global condition rather than assume it. Before the stopping rule is triggered, $p_k+q_k\le1$, and $k\ge0$ implies $x\ge-u_0\sqrt n$. Therefore

$$
xb_n(x)=-x^2\left(\alpha+\frac\beta{\sqrt n}x\right)\le0.
$$

For the [Lyapunov function](../../../../../../lyapunov-function.md) $V(x)=x^2$, the exact one-step generator is consequently

$$
G_nV(x)=2xb_n(x)+a_n(x)\le1.
$$

After stopping, the process is constant. Applying the elementary stopped [supermartingale](../../../../../../supermartingale.md) inequality for $V(X_{j/n}^n)-j/n$, and stopping also on first reaching $|X^n|\ge L$, gives

$$
\boxed{\mathbb P\left(\sup_{t\le1}|X^n_{t\wedge\tau_n}|\ge L\right)
\le\frac{(X_0^n)^2+1}{L^2}.}
$$

This is [compact containment](../../../../../../compact-containment.md). At zero population we use the natural absorbing convention $p_0=q_0=0$; the same calculation is valid there.

The invalid-probability threshold is at the positive root

$$
u_* =\frac{\sqrt{\alpha^2+4\beta}-\alpha}{2\beta}
\quad\text{of}\quad\alpha u+\beta u^2=1.
$$

Because $2\alpha^2<\beta$, we have $u_*>u_0$. The corresponding fluctuation level $\sqrt n(u_*-u_0)$ tends to infinity, so the stopping rule changes none of the compact-set moment limits. The initial fluctuation satisfies $|X_0^n|\le n^{-1/2}$ and hence tends to zero. All jumps have magnitude at most $n^{-1/2}$, so the Lindeberg condition is immediate. The limiting equation has globally Lipschitz coefficients and is well-posed and nonexplosive. The theorem therefore gives

$$
\boxed{dX_t=-\alpha X_tdt+\alpha\sqrt{\frac2\beta}\,dB_t,
\qquad X_0=0.}
$$

This is the [Ornstein-Uhlenbeck fluctuation limit at a stable population equilibrium](../../../../../../ornstein-uhlenbeck-fluctuation-limit-at-a-stable-population-equilibrium.md). The limiting [Ornstein-Uhlenbeck process](../../../../../../ornstein-uhlenbeck-process.md) has explicit solution

$$
X_t=\alpha\sqrt{\frac2\beta}\int_0^te^{-\alpha(t-s)}dB_s,
\qquad \operatorname{Var}(X_t)=\frac\alpha\beta(1-e^{-2\alpha t}).
$$

The PDF samples the linearly interpolated population at $\lfloor nt\rfloor$, so its displayed process is actually the step version. Using $nt$ instead gives the continuous interpolation; their uniform distance is at most $n^{-1/2}$. Both therefore have the asserted continuous diffusion limit, with the step version interpreted in [Skorokhod J1 topology](../../../../../../skorokhod-j1-topology.md).

Finally, if $\tau_n\le1$, the stopped fluctuation reaches a value greater than $\sqrt n(u_*-u_0)$. The preceding [Lyapunov function](../../../../../../lyapunov-function.md) bound gives directly

$$
\boxed{\mathbb P(\tau_n\le1)
\le\frac{(X_0^n)^2+1}{n(u_*-u_0)^2}\longrightarrow0.}
$$

This also shows explicitly why the artificial stopping rule is asymptotically irrelevant.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [6](../../6.md)
3. [Paper 29](../../../paper-29-split.md)
4. [Iii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
