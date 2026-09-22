<h1 id="b/8/solution">Solution</h1>

↑ **Parent:** [8](../8.md)

There are two distinct inconsistencies in the printed formulas. First the initial [Cauchy integral](../../../../cauchy-transform.md) has coefficient $1/(2\pi)$, whereas the stated boundary limits require **$1/(2\pi i)$**. Second the final [integral](../../../../integral-split.md) is a solution of a difference jump problem, although the intervening equation for $W$ is a sum jump problem. We derive the valid identities, show precisely where that final deduction fails, and give the corrected construction. Take $c>0$ and, initially, a Hölder continuous density on the interior with integrable endpoints, so the boundary limits and [principal values](../../../../cauchy-principal-value.md) exist.

Define the [Cauchy principal value](../../../../cauchy-principal-value.md) by

$$
\operatorname{pv}\int_0^c\frac{f(t)}{t-x}dt
=\lim_{\delta\downarrow0}\left(\int_0^{x-\delta}\frac{f(t)}{t-x}dt+
\int_{x+\delta}^c\frac{f(t)}{t-x}dt\right).
$$

For the corrected normalization $C_f(z)=(2\pi i)^{-1}\int_0^cf(t)/(t-z)\,dt$, subtract $f(x)$ from the numerator near $x$. The subtracted [integral](../../../../integral-split.md) has the common principal-value limit, while integration of the remaining constant density produces boundary arguments differing by $2\pi$. This proves the [Sokhotski–Plemelj theorem](../../../../sokhotski-plemelj-theorem.md)

$$
(C_f)_\pm=\pm\frac12f+\frac1{2\pi i}\operatorname{pv}\int_0^c\frac{f(t)}{t-x}dt.
$$

In particular $f=(C_f)_+-(C_f)_-$ and $(C_f)_++(C_f)_-=(\pi i)^{-1}\operatorname{pv}\int f(t)/(t-x)dt$. With the literal printed [integral](../../../../integral-split.md) $w=iC_f$ instead, the limits are $\pm if/2+(2\pi)^{-1}\operatorname{pv}\int f/(t-x)$, and the next stated boundary equation would have right side $i\gamma$.

Use the corrected normalization from now on and write $w=C_f$, $a=\alpha+\beta$, $b=\alpha-\beta$. The original [singular integral equation](../../../../singular-integral-equation.md) then becomes

$$
\alpha(w_+-w_-)+\beta(w_++w_-)=\gamma,
\qquad\boxed{a w_+-b w_-=\gamma.}
$$

If $\tilde w$ satisfies the printed homogeneous relation $a\tilde w_++b\tilde w_-=0$, division of $w=\tilde w W$ gives, correctly,

$$
W_++W_-=\frac{\gamma}{a\tilde w_+}.
$$

A nonvanishing factor is needed as well as the printed nonvanishing of $a,b$; its zeros would require separate treatment.

The next printed step is invalid because a [Cauchy integral](../../../../cauchy-transform.md) of $g$ has boundary difference $g$, not boundary sum $g$. A particularly direct counterexample is $\alpha=1$, $\beta=0$, $\gamma=1$. The original equation is simply **$f=1$**. Choose $\tilde w=\rho(z)=\sqrt{z(z-c)}$, with $\rho(z)\sim z$ at infinity and cut $[0,c]$. Its [boundary values](../../../../boundary-value.md) are $\rho_\pm(x)=\pm i\sqrt{x(c-x)}$, so it satisfies precisely the printed homogeneous sum relation. But the printed proposed [integral](../../../../integral-split.md) yields

$$
I(z)=\int_0^c\frac{dt}{\rho_+(t)(t-z)}
=\frac{i\pi}{\rho(z)},\qquad
\frac{\tilde w(z)I(z)}{2\pi i}=\frac12.
$$

The [integral](../../../../integral-split.md) follows by $t=c(1+\cos\theta)/2$, or the usual elementary [integral](../../../../integral-split.md) $\int_0^\pi d\theta/(A+B\cos\theta)$. Its proposed $w$ is constant, has jump zero, and is not the Cauchy transform of $f=1$; it also fails the required decay at infinity. If the printed $I(x)$ is interpreted as [principal value](../../../../cauchy-principal-value.md) in its last formula, that value is zero, giving $f=0$ and the same contradiction.

To solve the sum jump correctly, introduce this sign-changing factor $\rho$. Set $V=W/\rho$, so

$$
V_+-V_-=\frac{\gamma}{a\tilde w_+\rho_+}.
$$

The corrected local Cauchy representation is consequently

$$
\boxed{w(z)=\tilde w(z)\rho(z)
\left[\frac1{2\pi i}\int_0^c
\frac{\gamma(t)\,dt}{a(t)\tilde w_+(t)\rho_+(t)(t-z)}+H(z)\right].}
$$

Here $H$ has no jump across the open interval; its possible endpoint singularities and [polynomial](../../../../polynomial-split.md) part are determined by endpoint admissibility, absence of unwanted poles, and $w(z)=O(1/z)$ at infinity. Some choices of factor require a weighted or regularized [integral](../../../../integral-split.md) at the endpoints. Thus nonvanishing of $a,b$ alone does not determine a unique global solution without a [function](../../../../function-split.md) class and growth conditions.

Equivalently put $X=\tilde w\rho$. It satisfies the homogeneous _difference_ relation $aX_+-bX_-=0$. If $g=\gamma/(aX_+)$, $J(z)=\int_0^c g(t)/(t-z)\,dt$, and the [integral](../../../../integral-split.md) is admissible, then

$$
w=X\left(\frac{J}{2\pi i}+H\right).
$$

Taking its jump gives the usable density formula

$$
\boxed{f(x)=\frac{X_+-X_-}{2\pi i}\operatorname{pv}J(x)
+\frac{X_++X_-}{2}\frac{\gamma(x)}{a(x)X_+(x)}
+(X_+-X_-)H(x).}
$$

This formula, together with the endpoint and infinity conditions, replaces the last printed equation. Alternatively, if the homogeneous relation in the question is changed from plus to minus, its unweighted Cauchy representation becomes a valid particular solution, but the density must still be obtained from this jump calculation and homogeneous terms still require normalization. The statements cannot all hold simultaneously as printed.

## ↑ Ancestors (12)

1. [8](../8.md)
2. [B](../../b.md)
3. [2007](../../../2007-split.md)
4. [Past exam of the perturbation methods and applied complex variables course of the University of Oxford](../../../split.md)
5. [Perturbation methods and applied complex variables course of the University of Oxford](../../../../perturbation-methods-and-applied-complex-variables-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematics course of the University of Oxford](../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
