<h1 id="2/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

The solution and its first [derivative](../../../../../../derivative.md) are [continuous](../../../../../../continuous-function.md) at $x=1$: a jump would create a [Dirac delta distribution](../../../../../../dirac-delta-function.md) or its derivative, absent from the forcing. Put $r=x-1$, $A=a+1$ and $B=b$. The [outer expansions](../../../../../../outer-expansion.md), fixed by the respective endpoint [boundary conditions](../../../../../../boundary-condition.md), are

$$
y_L=A+r+\varepsilon\bigl[r+1+A\log|r|\bigr]+\cdots\quad(r<0),
\qquad y_R=B+\varepsilon B\log r+\cdots\quad(r>0).
$$

Balancing diffusion and advection near $r=0$ gives the [interior layer at a simple zero of advection](../../../../../../interior-layer-at-a-simple-zero-of-advection.md) with [inner variable](../../../../../../inner-variable.md) $z=r/\varepsilon$. The leading [inner expansion](../../../../../../inner-expansion.md) solves $Y_0''+2zY_0'=0$, so matching to $A$ and $B$ gives

$$
Y_0=c+d\operatorname{erf}z,\qquad c=\frac{A+B}{2},\qquad d=\frac{B-A}{2}.
$$

For the next term define the [Gaussian drift primitives](../../../../../../gaussian-drift-primitives.md)

$$
E_0(z)=\int_0^z e^{-t^2}\int_0^t e^{u^2}\,du\,dt,
\qquad E_1(z)=\int_0^z e^{-t^2}\int_0^t e^{u^2}\operatorname{erf}u\,du\,dt.
$$

Writing $H$ for the [Heaviside step function](../../../../../../heaviside-step-function.md), let $F(z)=zH(-z)+(\sqrt\pi/4)\operatorname{erf}|z|$. Its value and first derivative match at zero and $(D^2+2zD)F=2zH(-z)$. Thus

$$
Y_1=F+2cE_0+2dE_1+\alpha+\beta\operatorname{erf}z,
$$

where the logarithmic overlaps fix

$$
\alpha=\frac12-\frac{\sqrt\pi}{4}+c\log\varepsilon-2cC_1,
\qquad\beta=-\frac12+d\log\varepsilon-2dC_2.
$$

Here $C_1,C_2$ are the constants in the supplied large-positive-$z$ limits of $E_0,E_1$. The terms $\varepsilon\log\varepsilon$ are essential [switchback terms](../../../../../../switchback-term.md); discarding them would not give accuracy through $O(\varepsilon)$.

Subtracting the common overlap from the [inner expansion](../../../../../../inner-expansion.md) and [outer expansions](../../../../../../outer-expansion.md) gives the [additive composite expansion](../../../../../../additive-composite-expansion.md)

$$
\boxed{y_{\rm comp}(x)=Y_0(z)+\varepsilon Y_1(z)+\frac{\varepsilon r}{2}(1-\operatorname{erf}z),\qquad z=\frac{x-1}{\varepsilon}.}
$$

The standard overlap subtraction leaves $\varepsilon rH(-r)$. Replacing $H(-r)$ by $(1-\operatorname{erf}z)/2$ changes the value only by $O(\varepsilon^2)$ uniformly and gives a composite with continuous first derivative. The last term restores the endpoint values through the retained order. When $b=a+1$, $d=0$ and the order-one error-function jump disappears. An $O(\varepsilon)$ interior adjustment remains to accommodate the leading outer derivative mismatch, together with logarithmic matching when $A\ne0$.

Reversing the diffusion sign changes the leading inner equation to $-Y_0''+2zY_0'=0$. Its nonconstant solution grows like the integral of $e^{z^2}$, so bounded matching forces the same leading value $C$ on both sides. The bulk is $C+r$ on the left and $C$ on the right; both endpoint conditions are instead supplied by decaying [endpoint layers for reversed diffusion](../../../../../../endpoint-layers-for-reversed-diffusion.md), of width $\varepsilon^2$. A weaker width-$\varepsilon$ interior adjustment matches derivatives and selects $C$. Indeed, its first-order equation has a non-growing solution only if

$$
\int_{-\infty}^{\infty}e^{-z^2}\bigl(2C+2zH(-z)\bigr)\,dz=0,
\qquad C=\frac1{2\sqrt\pi}.
$$

The leading structure is consequently

$$
y\sim C+rH(-r)+(a-C+1)e^{-2x/\varepsilon^2}+(b-C)e^{-2(2-x)/\varepsilon^2},
$$

with the smaller interior correction understood. Unlike the positive-diffusion case, the endpoint values are not transported into two distinct order-one inner limits.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [2](../../2.md)
3. [Paper 336](../../../paper-336-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
