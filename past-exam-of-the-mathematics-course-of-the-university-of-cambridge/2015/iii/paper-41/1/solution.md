<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Normalize the [constant relative risk aversion utility](../../../../../constant-relative-risk-aversion-utility.md) as $U(c)=c^{1-R}/(1-R)$. The printed specification of $U'$ alone also permits an additive constant $K$; that would add $K/\rho$ to the value, so the stated [homogeneity](../../../../../homogeneity.md) holds for the normalized value. Set

$$
\kappa=\frac{\mu-r}{\sigma},\qquad x=\frac w{\bar w},\qquad 0<x\leq1.
$$

Multiplying initial wealth, the historical maximum, dollar investments, and consumption by $a>0$ multiplies every term of the wealth equation by $a$, including the tax term. It maps admissible policies bijectively and multiplies the normalized reward by $a^{1-R}$. Therefore **the value scales as**

$$
\boxed{V(w,\bar w)=\bar w^{1-R}v(w/\bar w).}
$$

The historical maximum means $\bar w_t=\max(\bar w_0,\sup_{0\leq s\leq t}w_s)$ when initially $w<\bar w$.

Inside the state region $w<\bar w$, the maximum is locally constant. The [Hamilton-Jacobi-Bellman equation](../../../../../hamilton-jacobi-bellman-equation.md) is

$$
0=-\rho V+rwV_w+
\sup_{\theta\in\mathbb R,\ c\geq0}
\left\{\tfrac12\sigma^2\theta^2V_{ww}
+(\mu-r)\theta V_w+U(c)-cV_w\right\}.
$$

At $w=\bar w$, the finite-variation contribution in the [Itô formula](../../../../../ito-s-lemma.md) is $(V_{\bar w}-\tau V_w)\,d\bar w$. The [high-water mark tax boundary condition](../../../../../high-water-mark-tax-boundary-condition.md) is consequently

$$
\boxed{V_{\bar w}(w,w)=\tau V_w(w,w).}
$$

For an increasing, strictly [concave function](../../../../../concave-function.md) of wealth, optimizing the two controls gives

$$
c^*=V_w^{-1/R},\qquad
\theta^*=-\frac{\mu-r}{\sigma^2}\frac{V_w}{V_{ww}}.
$$

The consumption [convex conjugate](../../../../../convex-conjugate.md) is

$$
\widetilde U(z)=\sup_{c>0}\{U(c)-zc\}
=\frac{R}{1-R}z^{1-1/R}.
$$

Substitution of the [homogeneity](../../../../../homogeneity.md) derivatives gives **the reduced equation and boundary condition**

$$
\boxed{\widetilde U(v')+rxv'-\rho v
-\frac{\kappa^2}{2}\frac{(v')^2}{v''}=0,\qquad
(1-R)v(1)=(1+\tau)v'(1).}
$$

The controls in scaled variables are $c^*/\bar w=(v')^{-1/R}$ and $\theta^*/\bar w=-(\mu-r)v'/(\sigma^2v'')$.

Use the [wealth-variable Legendre dual](../../../../../wealth-variable-legendre-dual.md)

$$
z=v'(x),\qquad J(z)=v(x)-xz.
$$

Since $v''<0$, the inverse map satisfies $J'=-x$ and $J''=-1/v''>0$. Inserting $v=J-zJ'$ into the reduced [Hamilton-Jacobi-Bellman equation](../../../../../hamilton-jacobi-bellman-equation.md) gives **a linear Euler equation**

$$
\boxed{\tfrac12\kappa^2z^2J''+(\rho-r)zJ'-\rho J
+\widetilde U(z)=0.}
$$

For the [Euler differential equation](../../../../../cauchy-euler-equation.md) operator on the left, its action on $z^t$ is $Q(t)z^t$. Write $b=1-1/R$. Under $\gamma_M=-Q(b)>0$, the particular solution is $-\widetilde U(z)/Q(b)$. For the nondegenerate case $\kappa\ne0$, the two characteristic roots are $-\alpha<0<t_+$, with $t_+>1$ because $Q(0)=-\rho$ and $Q(1)=-r$. Thus the general solution also contains $A(z/z_*)^{-\alpha}+Bz^{t_+}$.

Here $z_*=v'(1)$ and the relevant dual domain is $z\geq z_*$. The inverse wealth ratio must have $x=-J'(z)\to0$ as $z\to\infty$. The particular solution and the negative-root term have derivatives tending to zero, whereas $Bz^{t_+}$ has an unbounded derivative unless $B=0$. Hence **the admissible dual solution has the claimed form**

$$
\boxed{J(z)=\frac{\widetilde U(z)}{\gamma_M}
+A\left(\frac z{z_*}\right)^{-\alpha}.}
$$

The quadratic-root formulation presupposes a nonzero [market price of risk](../../../../../market-price-of-risk.md). If $\kappa=0$, the dual equation becomes first order; it is treated directly or by an appropriate nondegenerate limit rather than by assuming two quadratic roots.

The inverse map and the tax boundary provide two equations at $z_*$:

$$
J'(z_*)=-1,\qquad
(1-R)J(z_*)=(R+\tau)z_*.
$$

Because $\widetilde U'(z)=-z^{-1/R}$, these become

$$
\frac{z_*^{-1/R}}{\gamma_M}+\frac{\alpha A}{z_*}=1,
\qquad
\frac R{\gamma_M}z_*^{1-1/R}+(1-R)A=(R+\tau)z_*.
$$

Let $D=\alpha R+R-1$. Eliminating $z_*^{1-1/R}/\gamma_M$ gives $-DA=\tau z_*$. Also $D=R(\alpha+b)>0$, since $Q(b)<0$ puts $b$ strictly between the two roots. The derivative boundary then gives $z_*^{-1/R}/\gamma_M=(D+\alpha\tau)/D$. Therefore **the constants are**

$$
\boxed{z_*=\left[\frac{\alpha R+R-1}
{\gamma_M(\alpha R+R-1+\alpha\tau)}\right]^R,\qquad
A=-\frac{\tau z_*}{\alpha R+R-1}.}
$$

There is an important admissibility qualification in the printed conclusion. With $x(z)=-J'(z)$,

$$
x(z)=\frac{z^{-1/R}}{\gamma_M}
+\frac{\alpha A}{z_*}\left(\frac z{z_*}\right)^{-\alpha-1}.
$$

The second term is negative, but decays faster than the first because $\alpha+1>1/R$. Direct differentiation at the boundary gives

$$
\boxed{z_*J''(z_*)=\frac{1-\alpha\tau}{R}.}
$$

A [wealth-variable Legendre dual](../../../../../wealth-variable-legendre-dual.md) of a [concave](../../../../../concave-function.md) value must be a [convex function](../../../../../convex-function.md). Thus **the printed smooth tax-paying solution requires $\alpha\tau<1$**, with the limiting case $\alpha\tau=1$ allowed as a degenerate boundary. The assumptions $\gamma_M>0$ and $0<\tau<1$ do not imply this: for example $R=2$, $r=0.03$, $\rho=0.1$, $\kappa=0.2$, and $\tau=0.5$ give $\alpha=(5+\sqrt{105})/4>2$ and $\gamma_M=0.07$, hence negative boundary dual curvature.

For higher tax the investor can avoid raising the historical maximum. The [wealth-cap investment boundary](../../../../../wealth-cap-investment-boundary.md) replaces the tax-paying equality by $J''(z_*)=0$, alongside $J'(z_*)=-1$. Solving these equations gives

$$
z_*=\left[\frac{D}{\gamma_M R(\alpha+1)}\right]^R,\qquad
A=-\frac{z_*}{\alpha D}.
$$

These are the same constants with $\tau$ replaced by $\tau_{\rm eff}=1/\alpha$. More generally the admissible two-regime expression uses

$$
\boxed{\tau_{\rm eff}=\min(\tau,1/\alpha)}
$$

in the constants, while the claimed formulas themselves describe the tax-paying regime. In the cap regime the portfolio volatility vanishes at $x=1$ and the consumption rate there is $r+\kappa^2(\alpha+1)/(2R)>r$, so the wealth drift points inward and no new maximum is required. The remaining boundary inequality is $(V_{\bar w}-\tau V_w)/V_w=1/\alpha-\tau\leq0$, consistent with avoiding costly maximum increases. For $z>z_*$, dual curvature is positive because the negative term in $J''$ decays faster than the positive term. Thus this qualification repairs an actual missing parameter restriction rather than a TeX transcription error.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 41](../../paper-41-split.md)
3. [Iii](../../split.md)
4. [2015](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
