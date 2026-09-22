<h1 id="1/a/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Multiply the supplied [Feynman gauge](../../../../../feynman-gauge.md) propagators before reducing the numerator. Their two factors $-i$ and the source's [Clifford algebra](../../../../../clifford-algebra.md) imply

$$
\gamma^\nu\widetilde S(p+l)\gamma^\mu\widetilde\Delta_{\mu\nu}(l)
=\frac{(d-2)(\not p+\not l)+dm}
{(l^2-i0)[(p+l)^2+m^2-i0]}.
$$

For example, contracting the numerator before the propagator factors gives $\gamma^\nu[-(\not p+\not l)+m]\gamma_\nu=-(d-2)(\not p+\not l)-dm$; the extra minus from $(-i)^2$ reverses both signs.

Use a [Feynman parameter](../../../../../feynman-parameter.md) $x$ on the massive denominator and shift $q=l+xp$. The combined denominator is

$$
x[(p+l)^2+m^2]+(1-x)l^2=q^2+D(x),\qquad
D(x)=xm^2+x(1-x)p^2.
$$

The term odd in $q$ integrates to zero in [dimensional regularization](../../../../../dimensional-regularization.md). The pole can be evaluated away from on-shell infrared singularities; its local ultraviolet coefficient is independent of $D$. With the source's master integral,

$$
\begin{aligned}
\mathcal I_{\rm UV}(p)
&=-\frac{ie^2}{8\pi^2\epsilon}\int_0^1dx\,[2(1-x)\not p+4m]\\
&=-\frac{ie^2}{8\pi^2\epsilon}(\not p+4m),\qquad
\Sigma_{\rm UV}(p)=\frac{e^2}{8\pi^2\epsilon}(\not p+4m).
\end{aligned}
$$

Terms proportional to $d-4$ multiply the pole into a finite term, so they do not change this result. The [counterterm](../../../../../counterterm.md) [kernel](../../../../../kernel-of-a-linear-map-split.md) from 1ai is $K_{\rm ct}=-\delta Z_2\not p-\delta m_L$. Cancelling $-\Sigma_{\rm UV}+K_{\rm ct}$ therefore gives

$$
\boxed{\delta Z_2=-\frac{e^2}{8\pi^2\epsilon},\qquad
\delta m_L=-\frac{e^2m}{2\pi^2\epsilon}.}
$$

The distinction between [mass](../../../../../mass.md) definitions matters. Since $Z_2m_0=m+\delta m_L$,

$$
\boxed{m_0-m=\delta m_L-m\delta Z_2=-\frac{3e^2m}{8\pi^2\epsilon},\qquad
Z_m-1=-\frac{3e^2}{8\pi^2\epsilon}\quad(m_0=Z_mm).}
$$

Equivalently the mass-dependent part of the [counterterm](../../../../../counterterm.md) density is $+e^2m\bar\psi\psi/(2\pi^2\epsilon)$, because its definition includes the explicit minus sign in $-\delta m_L\bar\psi\psi$. In the alternative convention $d=4-2\varepsilon$, replace every $1/\epsilon$ here by $1/(2\varepsilon)$. These are ultraviolet minimal-subtraction poles, not the finite on-shell [mass](../../../../../mass.md) correction. The [Ward identity](../../../../../ward-identity.md) also fixes $\delta Z_1=\delta Z_2$; the [photon](../../../../../photon.md) coefficient $\delta Z_3$ requires its own two-point function and is not obtained from this graph.

## ↑ Ancestors (13)

1. [Iii](../iii.md)
2. [A](../../a.md)
3. [1](../../../1.md)
4. [2016](../../../../2016-split.md)
5. [Past exam of the advanced quantum field theory for particle physics course of the University of Oxford](../../../../split.md)
6. [Advanced quantum field theory for particle physics course of the University of Oxford](../../../../../advanced-quantum-field-theory-for-particle-physics-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematical and theoretical physics course of the University of Oxford](../../../../../year-4-of-the-mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
8. [Mathematical and theoretical physics course of the University of Oxford](../../../../../mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
