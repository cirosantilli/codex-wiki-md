<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Set $q=\log\psi$ and use the sign-appropriate [Cole-Hopf transformation](../../../../../../cole-hopf-transformation.md) $f=2\varepsilon q_\theta$. Direct differentiation gives

$$
f_z-ff_\theta-\varepsilon f_{\theta\theta}
=2\varepsilon\partial_\theta\left(q_z-\varepsilon q_{\theta\theta}-\varepsilon q_\theta^2\right)
=2\varepsilon\partial_\theta\left(\frac{\psi_z-\varepsilon\psi_{\theta\theta}}\psi\right).
$$

Thus the [heat equation](../../../../../../heat-equation.md) $\psi_z=\varepsilon\psi_{\theta\theta}$ implies the [viscous Burgers equation](../../../../../../viscous-burgers-equation.md) with the required negative nonlinear sign. Conversely, vanishing of the Burgers residual makes the final quotient depend only on $z$, and a multiplicative time-dependent factor in $\psi$ removes it. The algebraic substitution works for any nonzero $\varepsilon$ where $\psi\ne0$.

For a forward dissipative initial-value solution, take **$\varepsilon>0$ and $z>0$**. This is essential for the supplied [heat kernel](../../../../../../heat-kernel.md): at $\varepsilon<0$, $z>0$, its real [Gaussian integral](../../../../../../gaussian-integral.md) diverges even for $\psi(0,\phi)=1$. More generally that kernel requires $\varepsilon z>0$. The physical viscosity convention selects the positive case; the mere condition $\varepsilon\ne0$ does not justify a forward [Gaussian function](../../../../../../gaussian-function.md) formula.

Integrating $\partial_\theta\log\psi(0,\theta)=f_0(\theta)/(2\varepsilon)$ gives a positive continuous initial factor, normalized as

$$
\psi(0,\phi)=\begin{cases}1,&\phi\leq0,\\ e^{U\phi/(2\varepsilon)},&\phi\geq0.\end{cases}
$$

Its [heat kernel](../../../../../../heat-kernel.md) [convolution](../../../../../../convolution.md) converges for both signs of $U$, since a [Gaussian function](../../../../../../gaussian-function.md) dominates the one-sided exponential. Define

$$
J(b)=\int_b^\infty e^{-y^2/(4\varepsilon z)}dy,\qquad
S=\frac{U(2\theta+Uz)}{4\varepsilon}.
$$

The left half-line contributes $J(\theta)$; completing the square on the right half-line gives $e^S J(-\theta-Uz)$. Thus

$$
\psi(z,\theta)=\frac{J(\theta)+e^S J(-\theta-Uz)}{\sqrt{4\pi\varepsilon z}}.
$$

When differentiating, the two moving-endpoint [Gaussian function](../../../../../../gaussian-function.md) terms cancel, because

$$
e^S e^{-(\theta+Uz)^2/(4\varepsilon z)}=e^{-\theta^2/(4\varepsilon z)}.
$$

Only $\partial_\theta e^S=(U/(2\varepsilon))e^S$ remains in the logarithmic [derivative](../../../../../../derivative.md). The [viscous Burgers step solution with negative flux](../../../../../../viscous-burgers-step-solution-with-negative-flux.md) is therefore

$$
\boxed{f(z,\theta)=\frac{U}{1+\alpha e^{-S}},\qquad
\alpha=\frac{J(\theta)}{J(-\theta-Uz)}.}
$$

The denominator is strictly positive, so $f$ lies between $0$ and $U$, irrespective of the sign of $U$. Its initial limits away from $\theta=0$ are the required step.

For the spatial limits, the [Gaussian function](../../../../../../gaussian-function.md) tails must be compared with $e^S$; inspecting that exponential alone gives the wrong inference when $U<0$. As $b\to+\infty$, the [complementary error function](../../../../../../complementary-error-function.md) asymptotic gives

$$
J(b)\sim\frac{2\varepsilon z}{b}e^{-b^2/(4\varepsilon z)},\qquad
J(b)\to\sqrt{4\pi\varepsilon z}\quad(b\to-\infty).
$$

At $\theta\to+\infty$, $J(\theta)e^{-S}$ tends to zero even for $U<0$, because its quadratic decay dominates any exponential linear in $\theta$. Hence $\alpha e^{-S}\to0$. At $\theta\to-\infty$, use the identity above to obtain

$$
e^S J(-\theta-Uz)\sim\frac{2\varepsilon z}{-\theta-Uz}e^{-\theta^2/(4\varepsilon z)}\to0,
$$

while $J(\theta)$ approaches its full [Gaussian integral](../../../../../../gaussian-integral.md). Thus

$$
\boxed{f(z,\theta)\to U\ (\theta\to+\infty),\qquad f(z,\theta)\to0\ (\theta\to-\infty),}
$$

for both signs of $U$.

Since $J$ is strictly decreasing, $\alpha=1$ holds exactly when $\theta=-\theta-Uz$. At this point $S=0$, so the [midpoint symmetry of a viscous Burgers step](../../../../../../midpoint-symmetry-of-a-viscous-burgers-step.md) gives

$$
\boxed{\alpha=1\quad\Longleftrightarrow\quad\theta=-Uz/2,\qquad f=U/2.}
$$

More generally the exact symmetry is $f(z,-Uz-\theta)=U-f(z,\theta)$. For $U>0$, the midpoint follows the inviscid [shock](../../../../../../shock-wave.md) trajectory. For $U<0$, it is instead the center of an expanding fan, not a [shock](../../../../../../shock-wave.md).

The [vanishing viscosity approximation](../../../../../../vanishing-viscosity-approximation.md) makes the comparison precise. For fixed $z>0$ and $U>0$, near $\theta=-Uz/2$ both tail integrals tend to the full [Gaussian integral](../../../../../../gaussian-integral.md), so $\alpha\to1$ and

$$
f\sim\frac{U}{1+\exp\{-U(\theta+Uz/2)/(2\varepsilon)\}}.
$$

The layer has width $O(\varepsilon/U)$ and tends to the entropy [shock](../../../../../../shock-wave.md), with value $U/2$ at its center. Outside it the limits are $0$ and $U$.

For $U<0$, inside $0<\theta<-Uz$ both [Gaussian function](../../../../../../gaussian-function.md) tails have large positive lower limits. Their asymptotics give

$$
\alpha e^{-S}\sim\frac{-\theta-Uz}{\theta},\qquad
f\longrightarrow-\frac{\theta}{z}.
$$

Outside this interval the limits are $0$ on the left and $U$ on the right. Thus positive viscosity selects the [rarefaction wave](../../../../../../rarefaction-wave.md), including the same midpoint value as the inviscid fan. The two sign cases agree with the preceding [entropy solution](../../../../../../entropy-solution.md) construction, while a negative diffusivity would not furnish this dissipative selection.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 70](../../../paper-70-split.md)
4. [Iii](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
