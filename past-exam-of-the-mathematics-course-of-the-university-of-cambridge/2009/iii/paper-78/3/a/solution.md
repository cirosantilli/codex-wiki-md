<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For zero viscosity the [Inviscid Burgers equation](../../../../../../inviscid-burgers-equation.md) is $q_X-q q_\theta=0$. Along a [characteristic curve](../../../../../../characteristic-curve.md), $dq/dX=0$ and $d\theta/dX=-q$. Labelling a characteristic by its initial position $\eta$ gives

$$
\boxed{q=f(\eta),\qquad\theta=\eta-Xf(\eta),\qquad q(\theta,X)=f(\theta+Xq).}
$$

Where $f$ is differentiable, $q_\theta=f'(\eta)/(1-Xf'(\eta))$. The first characteristic crossing occurs at $X=1/\max f'$ if the maximum positive slope exists. A multivalued continuation is not a physical wave: rewrite the equation as the [conservation law](../../../../../../conservation-law.md) $q_X+\partial_\theta(-q^2/2)=0$ and replace the overturning part by an entropy-admissible [shock wave](../../../../../../shock-wave.md). The [Rankine-Hugoniot conditions](../../../../../../rankine-hugoniot-conditions.md) give its trajectory

$$
\frac{d\theta_s}{dX}=\frac{-q_R^2/2+q_L^2/2}{q_R-q_L}=-\frac{q_L+q_R}{2}.
$$

The states on either side are supplied by the characteristics meeting the shock. Conservation supplies the equal-area construction, and the entropy condition requires characteristics to enter the shock. Since the flux is concave, a jump with $q_L<q_R$ is compressive.

For the rising step, $q_L=0$ and $q_R=U>0$, the left characteristics have slope zero and the right ones slope $-U$. They overlap immediately. The [Burgers Riemann problem with negative flux](../../../../../../burgers-riemann-problem-with-negative-flux.md) is solved by

$$
\boxed{q(\theta,X)=\begin{cases}0,&\theta<-UX/2,\\U,&\theta>-UX/2,\end{cases}\qquad\theta_s(X)=-UX/2.}
$$

It is a shock, not a [rarefaction wave](../../../../../../rarefaction-wave.md); the minus sign in the nonlinear flux is decisive.

For positive viscosity, substitute $q=2\epsilon\partial_\theta\log\psi$ into the [viscous Burgers equation](../../../../../../viscous-burgers-equation.md). Writing $w=\log\psi$ gives

$$
q_X-qq_\theta-\epsilon q_{\theta\theta}
=2\epsilon\partial_\theta\left[w_X-\epsilon(w_{\theta\theta}+w_\theta^2)\right].
$$

An $X$-dependent multiplicative factor in $\psi$ removes the possible integration function. The [Cole-Hopf transformation](../../../../../../cole-hopf-transformation.md) therefore gives $\psi_X=\epsilon\psi_{\theta\theta}$. Normalize its initial value continuously at zero:

$$
\psi(\theta,0)=\begin{cases}1,&\theta<0,\\e^{U\theta/(2\epsilon)},&\theta>0.\end{cases}
$$

Split the [heat kernel](../../../../../../heat-kernel.md) integral at zero. Completing the square in the positive-half integral yields

$$
\boxed{\psi(\theta,X)=\frac12\operatorname{erfc}\left(\frac{\theta}{2\sqrt{\epsilon X}}\right)
+\frac12e^{U\theta/(2\epsilon)+U^2X/(4\epsilon)}\operatorname{erfc}\left(-\frac{\theta+UX}{2\sqrt{\epsilon X}}\right).}
$$

When differentiating, the Gaussian terms from the two [complementary error functions](../../../../../../complementary-error-function.md) cancel, because

$$
\frac{U\theta}{2\epsilon}+\frac{U^2X}{4\epsilon}-\frac{(\theta+UX)^2}{4\epsilon X}=-\frac{\theta^2}{4\epsilon X}.
$$

Thus the exact [viscous Burgers step solution with negative flux](../../../../../../viscous-burgers-step-solution-with-negative-flux.md) is

$$
\boxed{q(\theta,X)=\frac{U e^{U\theta/(2\epsilon)+U^2X/(4\epsilon)}\operatorname{erfc}\!\left(-\frac{\theta+UX}{2\sqrt{\epsilon X}}\right)}
{\operatorname{erfc}\!\left(\frac{\theta}{2\sqrt{\epsilon X}}\right)+e^{U\theta/(2\epsilon)+U^2X/(4\epsilon)}\operatorname{erfc}\!\left(-\frac{\theta+UX}{2\sqrt{\epsilon X}}\right)}.}
$$

For $X>0$ its denominator is positive, its tails tend to $0$ and $U$, and it approaches the initial step as $X\downarrow0$. At $\theta=-UX/2$ it equals $U/2$. Its [vanishing-viscosity limit](../../../../../../vanishing-viscosity-limit.md) gives the entropy shock above. At large $U\sqrt{X/\epsilon}$ near the moving shock center it approaches the travelling profile $U/[1+e^{-U(\theta+UX/2)/(2\epsilon)}]$, with thickness of order $\epsilon/U$.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3](../../3.md)
3. [Paper 78](../../../paper-78-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
