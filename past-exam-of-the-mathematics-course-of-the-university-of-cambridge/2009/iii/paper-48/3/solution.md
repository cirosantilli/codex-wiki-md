<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Let $\phi_B=Z_\phi^{1/2}\phi$ define the renormalized field in [Phi-fourth theory](../../../../../quartic-interaction.md). For an $n$-point [correlation function](../../../../../correlation-function.md), with no composite operator insertions, this implies

$$
G_{n,B}=Z_\phi^{n/2}G_n.
$$

The bare [correlation function](../../../../../correlation-function.md) is independent of the arbitrary [renormalization scale](../../../../../renormalization-scale.md) $\mu$ when the bare parameters and external momenta are fixed. Define

$$
\widehat\beta_\lambda=\left.\mu\frac{d\lambda}{d\mu}\right|_B,\qquad \gamma_{m^2}=\left.\mu\frac{d\log m^2}{d\mu}\right|_B,\qquad \gamma_\phi=\left.\frac12\mu\frac{d\log Z_\phi}{d\mu}\right|_B.
$$

The definitions of the [running mass](../../../../../running-mass.md) and [wave-function renormalization](../../../../../wave-function-renormalization.md) functions specify their signs and the factor of two. Differentiating $Z_\phi^{n/2}G_n$ using the [chain rule](../../../../../chain-rule.md) yields the **Callan–Symanzik equation**

$$
\boxed{\left[\mu\partial_\mu+\widehat\beta_\lambda\partial_\lambda+m^2\gamma_{m^2}\partial_{m^2}+n\gamma_\phi\right]G_n=0.}
$$

Here $\widehat\beta_\lambda$ denotes the [renormalization-group beta function](../../../../../beta-function-physics.md) itself, not the function multiplied by an additional $\lambda$. The [Callan-Symanzik equation](../../../../../callan-symanzik-equation.md) concerns dependence on the arbitrary reference scale, with the displayed external momenta kept fixed.

For the [minimal subtraction scheme](../../../../../minimal-subtraction-scheme.md) in [dimensional regularization](../../../../../dimensional-regularization.md), write

$$
F(\lambda,\epsilon)=\lambda+\sum_{k\geq1}\frac{f_k(\lambda)}{\epsilon^k},\qquad H(\lambda,\epsilon)=1+\sum_{k\geq1}\frac{b_k(\lambda)}{\epsilon^k},
$$

so $\lambda_B=\mu^\epsilon F$ and $m_B^2=m^2H$. The $\mu^\epsilon$ factor gives the engineering contribution $-\epsilon\lambda$ to the [renormalization-group beta function](../../../../../beta-function-physics.md). Put $\widehat\beta_\lambda=-\epsilon\lambda+\beta_\lambda$. Scale independence of the bare coupling then gives

$$
0=\epsilon F+\widehat\beta_\lambda\partial_\lambda F
=\epsilon(F-\lambda F')+\beta_\lambda F'.
$$

The coefficient of $\epsilon^0$ is $f_1-\lambda f_1'+\beta_\lambda$. Its vanishing proves the first of the [simple-pole formulas for minimal-subtraction renormalization group functions](../../../../../simple-pole-formulas-for-minimal-subtraction-renormalization-group-functions.md):

$$
\boxed{\beta_\lambda=\widehat\beta_\lambda+\epsilon\lambda=(\lambda\partial_\lambda-1)f_1(\lambda).}
$$

The coefficients of $\epsilon^{-k}$, $k\geq1$, also vanish and impose $(\lambda\partial_\lambda-1)f_{k+1}=\beta_\lambda f_k'$. These relations explain how the higher poles are consistent with a finite [renormalization-group beta function](../../../../../beta-function-physics.md).

For the mass, differentiate the second bare-parameter relation:

$$
0=\gamma_{m^2}H+\widehat\beta_\lambda H'.
$$

Its finite coefficient is $\gamma_{m^2}-\lambda b_1'$. Therefore

$$
\boxed{\gamma_{m^2}=\lambda\partial_\lambda b_1(\lambda).}
$$

The higher poles impose $\lambda b_{k+1}'=\gamma_{m^2}b_k+\beta_\lambda b_k'$. The formulas for the [running mass](../../../../../running-mass.md) and [renormalization-group beta function](../../../../../beta-function-physics.md) thus follow directly from bare-parameter independence rather than from an identification with diagram coefficients by name.

At the specified [loop order](../../../../../loop-order.md), $f_1=3\lambda^2/(16\pi^2)$ and $b_1=\lambda/(16\pi^2)$. There is no [wave-function renormalization](../../../../../wave-function-renormalization.md) at this order. Hence

$$
\boxed{\beta_\lambda=\frac{3\lambda^2}{16\pi^2}+O(\lambda^3),\qquad \gamma_{m^2}=\frac{\lambda}{16\pi^2}+O(\lambda^2),\qquad \gamma_\phi=0+O(\lambda^2).}
$$

The regulated [renormalization-group beta function](../../../../../beta-function-physics.md) is $\widehat\beta_\lambda=-\epsilon\lambda+3\lambda^2/(16\pi^2)+O(\lambda^3)$; after removing the regulator, $\widehat\beta_\lambda=\beta_\lambda$.

Now take $m^2=0$ and the four-dimensional limit. This massless surface is preserved since $\mu\,dm^2/d\mu=m^2\gamma_{m^2}$. Set $b=3/(16\pi^2)$, choose a reference scale $\mu_0$, and define the [running coupling](../../../../../running-coupling.md) by

$$
\frac{d\lambda(\mu)}{d\log\mu}=b\lambda(\mu)^2,\qquad \lambda(\mu_0)=\lambda_0.
$$

Differentiating $1/\lambda$ gives $d(1/\lambda)/d\log\mu=-b$, so

$$
\boxed{\lambda(\mu)=\frac{\lambda_0}{1-b\lambda_0\log(\mu/\mu_0)}.}
$$

The zero-coupling solution is obtained by continuity. At one-loop accuracy $\gamma_\phi=0$, and the [chain rule](../../../../../chain-rule.md) turns the massless [Callan-Symanzik equation](../../../../../callan-symanzik-equation.md) into

$$
\frac{d}{d\log\mu}G_n(p_1,\ldots,p_n;0,\lambda(\mu),\mu)=0.
$$

Thus the **one-loop solution along a running-coupling trajectory** is

$$
\boxed{G_n(p_1,\ldots,p_n;0,\lambda(\mu),\mu)=G_n(p_1,\ldots,p_n;0,\lambda_0,\mu_0).}
$$

For a prescribed endpoint coupling $\lambda$, substitute $\lambda_0=\lambda/[1+b\lambda\log(\mu/\mu_0)]$ on the right. The reference [correlation function](../../../../../correlation-function.md) supplies arbitrary boundary data; the [Callan-Symanzik equation](../../../../../callan-symanzik-equation.md) determines their scale evolution, not their full momentum dependence. The [running coupling](../../../../../running-coupling.md) formula is used on a branch on which its denominator is nonzero and the retained perturbative approximation is appropriate.

If one keeps $\epsilon\ne0$, the same characteristic calculation uses $d\lambda/d\log\mu=-\epsilon\lambda+b\lambda^2$. Writing $r=\mu/\mu_0$ gives $\lambda(\mu)=\lambda_0r^{-\epsilon}/[1-(b\lambda_0/\epsilon)(1-r^{-\epsilon})]$, which tends to the displayed four-dimensional result as $\epsilon\to0$.

With a nonzero [anomalous dimension](../../../../../anomalous-dimension.md), the characteristic equation instead reads $dG_n/d\log\mu=-n\gamma_\phi(\lambda(\mu))G_n$. Integration proves the [characteristic solution of the massless Callan-Symanzik equation](../../../../../characteristic-solution-of-the-massless-callan-symanzik-equation.md):

$$
G_n(\boldsymbol p;0,\lambda(\mu),\mu)=\exp\left[-n\int_{\mu_0}^{\mu}\gamma_\phi(\lambda(\nu))\frac{d\nu}{\nu}\right]G_n(\boldsymbol p;0,\lambda_0,\mu_0).
$$

For the stipulated $\gamma_\phi=c\lambda^2$ and the same one-loop [renormalization-group beta function](../../../../../beta-function-physics.md), change variables using $d\log\nu=d\lambda/(b\lambda^2)$. The exponent's integral becomes $(c/b)(\lambda(\mu)-\lambda_0)$. Therefore the **modified explicit solution** is

$$
\boxed{G_n(\boldsymbol p;0,\lambda(\mu),\mu)=\exp\left[-\frac{nc}{b}\big(\lambda(\mu)-\lambda_0\big)\right]G_n(\boldsymbol p;0,\lambda_0,\mu_0).}
$$

Equivalently its multiplicative factor is $\exp[-nc\lambda_0^2\log r/(1-b\lambda_0\log r)]$. This solves the equation with the stated truncated [renormalization-group beta function](../../../../../beta-function-physics.md) and [anomalous dimension](../../../../../anomalous-dimension.md); it does not introduce additional higher-order coefficients that were not specified.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 48](../../paper-48-split.md)
3. [Iii](../../split.md)
4. [2009](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
