<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Put $\xi_t=\ker\alpha_t$, the [contact distribution](../../../../../contact-distribution.md). If $\dim M=2r+1$, the [contact form](../../../../../contact-form.md) condition is $\alpha_t\wedge(d\alpha_t)^r\ne0$. It implies that $d\alpha_t|_{\xi_t}$ is a [symplectic form](../../../../../symplectic-form.md) on each contact hyperplane: inserting a vector transverse to $\xi_t$ in that volume form leaves the nonzero top exterior power $(d\alpha_t|_{\xi_t})^r$. Hence there is a unique smooth [time-dependent vector field](../../../../../time-dependent-vector-field.md) $Y_t\in\xi_t$ satisfying

$$
(\iota_{Y_t}d\alpha_t)|_{\xi_t}=-\dot\alpha_t|_{\xi_t}.
$$

Its smoothness follows by inverting the smoothly varying [nondegenerate](../../../../../nondegenerate-bilinear-form.md) matrix of this [contact distribution symplectic form](../../../../../contact-distribution-symplectic-form.md). This is the [horizontal generator of contact stability](../../../../../horizontal-generator-of-contact-stability.md).

Let $R_t$ be the [Reeb vector field](../../../../../reeb-vector-field.md) of $\alpha_t$. The one-form $\dot\alpha_t+\iota_{Y_t}d\alpha_t$ vanishes on $\xi_t$, so it is $h_t\alpha_t$. Evaluating on $R_t$, using $\alpha_t(R_t)=1$ and $\iota_{R_t}d\alpha_t=0$, identifies the coefficient:

$$
h_t=\dot\alpha_t(R_t),\qquad
\dot\alpha_t+\iota_{Y_t}d\alpha_t=h_t\alpha_t.
$$

By [Cartan's magic formula](../../../../../cartan-s-magic-formula.md), the [Lie derivative of a differential form](../../../../../lie-derivative-of-a-differential-form.md) is

$$
\mathcal L_{Y_t}\alpha_t=\iota_{Y_t}d\alpha_t+d(\alpha_t(Y_t))
=\iota_{Y_t}d\alpha_t,
$$

because $Y_t$ lies in the contact hyperplane.

Let $\rho_t$ solve $\partial_t\rho_t=Y_t\circ\rho_t$, with $\rho_0=\operatorname{id}_M$. Since $M$ is compact without boundary and $Y_t$ is smooth on the closed time interval, its solutions cannot escape and exist for the entire interval. Reversing the time-dependent equation supplies a smooth inverse for each $\rho_t$. Thus these [flow maps](../../../../../flow-map.md) give a [smooth isotopy](../../../../../smooth-isotopy.md). Differentiating the [pullback of a differential form](../../../../../pullback-of-a-differential-form.md) along this isotopy yields

$$
\frac d{dt}(\rho_t^*\alpha_t)
=\rho_t^*(\dot\alpha_t+\mathcal L_{Y_t}\alpha_t)
=(h_t\circ\rho_t)\rho_t^*\alpha_t.
$$

For each base point this is a scalar linear equation for a covector, initially $\alpha_0$. Its solution is

$$
\boxed{\rho_t^*\alpha_t=u_t\alpha_0,\qquad
u_t(x)=\exp\left(\int_0^t h_s(\rho_s(x))\,ds\right)>0.}
$$

By [finite-time flow completeness on a compact manifold](../../../../../finite-time-flow-completeness-on-a-compact-manifold.md), this construction gives the whole time interval. The [contact conformal factor along an isotopy](../../../../../contact-conformal-factor-along-an-isotopy.md) is smooth in $(t,x)$ and nowhere zero, proving [Gray stability theorem](../../../../../gray-stability-theorem.md). The precise domains here are $\rho_t:M\to M$ and $\rho:M\times[0,1]\to M$; the extra time factor attached to the already indexed $\rho_t$ in the source is a notational slip. The proof produces the required family on its whole specified interval. If a parameter domain of all $\mathbb R$ is intended, extend the smooth field slightly beyond $[0,1]$, multiply it by a time cutoff, and use compactness to obtain the extended isotopy $\rho:M\times\mathbb R\to M$. Its restriction to $[0,1]$ is unchanged.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 15](../../paper-15-split.md)
3. [Iii](../../split.md)
4. [2012](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
