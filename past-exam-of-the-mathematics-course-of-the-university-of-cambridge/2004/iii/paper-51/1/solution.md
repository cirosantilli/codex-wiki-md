<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

The [canonical momentum](../../../../../canonical-momentum.md) is $\pi=\phi_t$, so the [Hamiltonian density](../../../../../hamiltonian-density.md) and total [energy](../../../../../energy.md) are

$$
\mathcal H=\pi\phi_t-\mathcal L=\frac12\phi_t^2+\frac12\phi_x^2+U(\phi),\qquad
\boxed{E=\int_{\mathbb R}\left(\frac12\phi_t^2+\frac12\phi_x^2+U\right)dx.}
$$

The [Euler-Lagrange field equation](../../../../../euler-lagrange-field-equation.md) is $\phi_{tt}-\phi_{xx}+U'(\phi)=0$. Multiplication by $\phi_t$ gives the local [conservation of energy](../../../../../conservation-of-energy.md) identity

$$
\partial_t\mathcal H=\partial_x(\phi_t\phi_x).
$$

Thus $E$ is conserved when the [energy](../../../../../energy.md) flux vanishes at spatial infinity. For finite [energy](../../../../../energy.md) with asymptotically constant fields, the endpoints $\phi_\pm$ must be [scalar-field vacua](../../../../../scalar-field-vacuum.md), where $U=0$.

Choose an [antiderivative](../../../../../antiderivative.md) $G'(\phi)=\sqrt{2U(\phi)}$. For either sign $s=\pm1$, [completing the square](../../../../../completing-the-square.md) gives

$$
E=\frac12\int\phi_t^2dx+\frac12\int(\phi_x-s\sqrt{2U})^2dx+s[G(\phi_+)-G(\phi_-)].
$$

Choosing $s$ to make the boundary term nonnegative proves the [Bogomolny bound](../../../../../bogomolny-bound.md)

$$
\boxed{E\geq\left|\int_{\phi_-}^{\phi_+}\sqrt{2U(a)}\,da\right|,\qquad
\phi_t=0,\quad\phi_x=s\sqrt{2U(\phi)}\ \text{at saturation}.}
$$

These [Bogomolny equations](../../../../../bogomolny-equations.md) obtained by [square completion for a one-dimensional kink](../../../../../square-completion-for-a-one-dimensional-kink.md) describe minima within a fixed endpoint sector when a saturating configuration exists. Differentiating the spatial equation gives $\phi_{xx}=U'(\phi)$ wherever $U>0$, with smooth extension to its limiting [scalar-field vacua](../../../../../scalar-field-vacuum.md). The absolute minimum across all sectors is a constant zero-potential [scalar-field vacuum](../../../../../scalar-field-vacuum.md) when one exists; the nontrivial minima are sector-specific [kinks](../../../../../scalar-field-kink.md).

For $\beta\ne0$, write $b=|\beta|$. The [scalar-field vacua](../../../../../scalar-field-vacuum.md) are $-b,0,b$. A static finite-energy solution has the first integral

$$
\frac12\phi_x^2-U(\phi)=0,
$$

because differentiating its left side gives $\phi_x(\phi_{xx}-U')=0$, and its value is zero at infinity. In either adjacent interval, $\sqrt{2U}=|\phi|(b^2-\phi^2)$. Set $y=\phi^2/b^2$. The first-order equation becomes $y_x=\eta\,2b^2y(1-y)$, with $\eta=\pm1$, and separation gives $\log[y/(1-y)]=2\eta b^2(x-x_0)$. Hence

$$
\boxed{\phi_{\sigma,\eta}(x)=\frac{\sigma b}{\sqrt{1+e^{-2\eta b^2(x-x_0)}}},\qquad \sigma,\eta\in\{1,-1\}.}
$$

For $\eta=1$ the endpoints are $0\to\sigma b$; for $\eta=-1$ they are $\sigma b\to0$. Thus there are **four oriented static [kink](../../../../../scalar-field-kink.md) families, up to translation**, namely two increasing [kinks](../../../../../scalar-field-kink.md) and two decreasing [antikinks](../../../../../antikink.md). Each has rest [energy](../../../../../energy.md)

$$
\int_0^b a(b^2-a^2)\,da=\frac{b^4}{4}.
$$

A static field joining $-b$ directly to $b$ would have to pass through $\phi=0$ at finite $x$. The first integral then gives $\phi_x=0$, and the [Picard-Lindelöf theorem](../../../../../picard-lindelof-theorem.md) applied to the smooth second-order equation with those [initial conditions](../../../../../initial-condition.md) forces $\phi\equiv0$. Therefore there is no such additional [kink](../../../../../scalar-field-kink.md); this is the [intermediate-vacuum obstruction to a kink](../../../../../intermediate-vacuum-obstruction-to-a-kink.md). The [Bogomolny classification of a rescaled phi-six kink](../../../../../bogomolny-classification-of-a-rescaled-phi-six-kink.md) also shows that if $\beta=0$, only the [scalar-field vacuum](../../../../../scalar-field-vacuum.md) $0$ remains and there is **no nontrivial finite-energy static [kink](../../../../../scalar-field-kink.md)**. Indeed the first integral gives a monotone field wherever it is nonzero, precluding a return to the same [scalar-field vacuum](../../../../../scalar-field-vacuum.md).

<a id="1/image-four-oriented-elementary-phi-six-kink-profiles-connecting-adjacent-vacua-with-equal-rest-energy"></a>
![](../../../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-51-kinks.png)

**[Figure 1](#1/image-four-oriented-elementary-phi-six-kink-profiles-connecting-adjacent-vacua-with-equal-rest-energy). Four oriented elementary phi-six kink profiles connecting adjacent vacua, with equal rest energy**.

A [Lorentz boost](../../../../../lorentz-boost.md) of the $0\to b$ profile gives a moving solution with arbitrary $|v|<1$:

$$
\boxed{\phi(x,t)=\frac{b}{\sqrt{1+\exp[-2b^2\gamma(x-vt-x_0)]}},\qquad\gamma=(1-v^2)^{-1/2}.}
$$

If $K$ denotes the static profile and $\xi=\gamma(x-vt-x_0)$, then $\phi_{tt}-\phi_{xx}=\gamma^2(v^2-1)K''=-K''$, proving the [Euler-Lagrange field equation](../../../../../euler-lagrange-field-equation.md) directly. Its [energy](../../../../../energy.md) is $\gamma b^4/4$: since $K'^2=2U(K)$, changing variable to $\xi$ in the [energy](../../../../../energy.md) integral gives the factor $\gamma$. Reversing $\sigma$ or $\eta$ yields the other moving elementary profiles.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 51](../../paper-51-split.md)
3. [Iii](../../split.md)
4. [2004](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
