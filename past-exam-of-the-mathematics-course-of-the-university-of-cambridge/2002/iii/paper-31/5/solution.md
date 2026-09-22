<h1 id="5/solution">Solution</h1>

↑ **Parent:** [5](../5.md)

Write $f=u+iv$. The [Cauchy-Riemann equations](../../../../../cauchy-riemann-equations.md) give $v_x=-u_y$, $v_y=u_x$ and $\Delta u=\Delta v=0$. Since the two Brownian coordinates are [independent](../../../../../independent-random-variables.md), $[X]_t=[Y]_t=t$ and $[X,Y]_t=0$. The [Itô formula](../../../../../ito-s-lemma.md) therefore becomes

$$
dU_t=u_x(Z_t)dX_t+u_y(Z_t)dY_t,\qquad dV_t=-u_y(Z_t)dX_t+u_x(Z_t)dY_t.
$$

Stop in balls on which the derivatives are bounded. The stopped integrals are [martingales](../../../../../martingale-split.md), proving that $U$ and $V$ are [local martingales](../../../../../local-martingale.md). Their coefficient rows have equal squared length and are [orthogonal](../../../../../orthogonal-vectors.md). Thus

$$
\boxed{[U]_t=[V]_t=\int_0^t|f'(Z_s)|^2ds,\qquad [U,V]_t=0.}
$$

These are [quadratic covariations of an analytic Brownian image](../../../../../quadratic-covariations-of-an-analytic-brownian-image.md); [orthogonality](../../../../../orthogonal-vectors.md) does not in general imply [independence](../../../../../independent-random-variables.md) of the two transformed coordinates.

For the exit law, put $c=2a^2$. Squaring sends the positive quadrant to the upper half-plane, sends $a+ia$ to $ic$, and the [Möbius transformation](../../../../../mobius-transformation.md) $w\mapsto(w-ic)/(w+ic)$ sends the upper half-plane to the unit disk with the starting point sent to zero. Its composition is the displayed [conformal map](../../../../../conformal-map.md). The exit time is finite: it is the minimum of the two almost surely finite one-dimensional hitting times of zero. There is no hit at the quadrant's corner, since a [planar Brownian motion](../../../../../planar-brownian-motion.md) started away from zero avoids that point.

We can justify the uniform image exit law without assuming a conformal-time-change theorem. For each integer $n\ge1$, the real and imaginary parts of $f(Z_{t\wedge T})^n$ are bounded [martingales](../../../../../martingale-split.md) obtained from [harmonic functions](../../../../../harmonic-function.md). At the start their values are zero. The [bounded convergence theorem](../../../../../bounded-convergence-theorem.md) at the finite exit time gives $\mathbb E f(Z_T)^n=0$. The boundary image has modulus one, and conjugation gives the vanishing negative Fourier moments as well. Trigonometric polynomials are dense among [continuous functions](../../../../../continuous-function.md) on the [unit circle](../../../../../complex-unit-circle.md), so these moments characterize the [uniform distribution](../../../../../continuous-uniform-distribution.md) there.

Consequently the real variable $W=Z_T^2$ is the inverse image of a uniform point $e^{i\Theta}$ under that [Möbius transformation](../../../../../mobius-transformation.md):

$$
W=ic\,\frac{1+e^{i\Theta}}{1-e^{i\Theta}}=-c\cot(\Theta/2).
$$

The Jacobian of this change of variable gives the centered [Cauchy distribution](../../../../../cauchy-distribution.md) of scale $c$:

$$
p_W(w)=\frac{c}{\pi(w^2+c^2)},\qquad w\in\mathbb R.
$$

Positive $w$ corresponds to exit at $\sqrt w$ on the real axis; negative $w$ corresponds to exit at $i\sqrt{-w}$ on the imaginary axis. Pulling back by $w=\pm r^2$ therefore gives the complete boundary law

$$
\boxed{\mathbb P(Z_T\in dr)=\frac{4a^2r}{\pi(r^4+4a^4)}dr,\qquad \mathbb P(Z_T\in i\,dr)=\frac{4a^2r}{\pi(r^4+4a^4)}dr\quad(r>0).}
$$

Here $dr$ on each axis denotes length along that axis, not two-dimensional area measure. Each density integrates to $1/2$, with no remaining atoms. Equivalently the chosen axis is a fair Bernoulli choice [independent](../../../../../independent-random-variables.md) of the radius, and

$$
\boxed{\mathbb P(|Z_T|\le r)=\frac2\pi\arctan\!\left(\frac{r^2}{2a^2}\right),\quad r\ge0.}
$$

This is [Brownian exit law from a quadrant](../../../../../brownian-exit-law-from-a-quadrant.md), obtained as a [harmonic measure](../../../../../harmonic-measure.md) and not as an absolutely continuous planar density.

## ↑ Ancestors (10)

1. [5](../5.md)
2. [Paper 31](../../paper-31-split.md)
3. [Iii](../../split.md)
4. [2002](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
