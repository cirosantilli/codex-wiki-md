<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

One precise relation is to [radial SLE](../../../../../../radial-schramm-loewner-evolution.md) with parameter $2$. Its orientation is from the boundary point $1$ to the interior target $0$. With conformal-radius time it is defined by

$$
\partial_tg_t(z)=g_t(z)\frac{e^{i\theta_t}+g_t(z)}{e^{i\theta_t}-g_t(z)},
\qquad\theta_t=\sqrt2\,\beta_t,\qquad g_t'(0)=e^t.
$$

There is a coupling of the conditioned Brownian path $B$ with this simple radial curve $\eta$ such that, for each initial curve segment, the first point at which $B$ encounters it is its tip. More precisely, if $s_t=\inf\{s:B_s\in\eta[0,t]\}$, then $B_{s_t}=\eta(t)$. Reversing the Brownian path turns these first-hit times into the last-visit times that characterize [loop-erasure of planar Brownian motion](../../../../../../loop-erasure-of-planar-brownian-motion.md). Thus

$$
\boxed{\eta\text{ is a loop-erasure of the time reversal of }B,
\qquad\eta\sim\operatorname{radial\ SLE}_2(D;1\to0).}
$$

This is an existence statement for a coupling, not a pointwise equality of the two processes or a claim that a naive finite-loop deletion algorithm applies to [Brownian motion](../../../../../../brownian-motion-split.md).

Here is the [martingale](../../../../../../martingale-split.md) mechanism behind the coupling. Put $a_t=e^{i\theta_t}$ and

$$
Q_t(z)=\operatorname{Re}\frac{a_t+g_t(z)}{a_t-g_t(z)}.
$$

This is the positive slit-domain [Poisson kernel](../../../../../../poisson-kernel-for-the-upper-half-plane.md) at the tip, normalized by $Q_t(0)=1$. Writing $q_t=g_t(z)/a_t$, the radial equation gives

$$
dq_t=-i\sqrt\kappa\,q_t\,d\beta_t+
\left[q_t\frac{1+q_t}{1-q_t}-\frac\kappa2q_t\right]dt.
$$

The drift of $(1+q_t)/(1-q_t)$ is $(2-\kappa)q_t(1+q_t)/(1-q_t)^3$, so $Q_t(z)$ is a [local martingale](../../../../../../local-martingale.md) at $\kappa=2$.

Start independent stopped $B$ and [radial SLE2](../../../../../../radial-sle2.md), and weight their joint laws, before meeting, by

$$
L(s,t)=\frac{Q_t(B_s)}{h(B_s)}.
$$

For fixed $s$ this is an [SLE](../../../../../../schramm-loewner-evolution.md) [local martingale](../../../../../../local-martingale.md). For fixed $t$ it is a Brownian-transform [local martingale](../../../../../../local-martingale.md), because $\mathcal L^h(Q_t/h)=(2h)^{-1}\Delta Q_t=0$. Since $L(0,t)=L(s,0)=1$, localized two-parameter weighting preserves both original marginals. For a fixed slit, the changed Brownian law is the transform by $Q_t$, so it hits that slit at the pole, its tip. Compatible stopped couplings, followed by exhaustion, give the first-hit-at-tip property. This completion is the substantive continuum coupling step. Discrete [loop-erased random walks](../../../../../../loop-erased-random-walk.md) and their radial-SLE2 limit give a parallel approximation picture.

For example, in this coupling avoidance by $B$ implies avoidance by $\eta$, since the radial curve is contained in the Brownian trace. The probability from part (b) therefore supplies a lower bound $|\phi'(1)|\leq\mathbb P(\eta\subset U)$. The two avoidance laws are not identical: unweighted simple radial $\operatorname{SLE}_2$ does not have the Brownian radial-restriction property. This is a way to transfer path-containment information while retaining the distinct geometry and orientation of the two random curves.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [3](../../3.md)
3. [Paper 35](../../../paper-35-split.md)
4. [Iii](../../../split.md)
5. [2012](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
