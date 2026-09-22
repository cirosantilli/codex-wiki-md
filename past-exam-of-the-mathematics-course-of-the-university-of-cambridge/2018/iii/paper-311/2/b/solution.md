<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The [Physical-process first law for a rotating black hole](../../../../../../physical-process-first-law-for-a-rotating-black-hole.md) applies to a small perturbation of a stationary nonextremal vacuum [black hole](../../../../../../black-hole.md) by infalling neutral matter, followed by relaxation to stationarity. Its first-order form is

$$
\boxed{\delta M-\Omega_H\delta J=\frac{\kappa}{8\pi G}\delta A.}
$$

Here the background horizon generator is $\xi=t+\Omega_H\varphi$, normalized by the unit time translation at infinity, and its [surface gravity](../../../../../../surface-gravity.md) is constant, $\kappa>0$, as in the [Zeroth law of black-hole mechanics](../../../../../../zeroth-law-of-black-hole-mechanics.md). The formula neglects terms quadratic in the perturbation. Choose the process sufficiently weak that the horizon generators used below have no large caustics, and assume appropriate early and late stationary limits and convergent fluxes.

On the background [Killing horizon](../../../../../../killing-horizon.md), choose an affine generator $\ell=d/d\lambda$ such that $\xi=\kappa\lambda\ell$; the bifurcation or early stationary limit corresponds to $\lambda=0$. The background [null expansion](../../../../../../null-expansion.md) and [null shear](../../../../../../null-shear.md) vanish. The [null twist](../../../../../../null-twist.md) is zero because the perturbed event horizon is a [null hypersurface](../../../../../../null-hypersurface.md). Linearizing the [Null Raychaudhuri equation](../../../../../../null-raychaudhuri-equation.md) and using the [Einstein field equations](../../../../../../einstein-field-equations.md) gives

$$
\frac{d(\delta\theta)}{d\lambda}=-\delta R_{ab}\ell^a\ell^b=-8\pi G\,\delta T_{ab}\ell^a\ell^b.
$$

The expansion squared and shear squared are second order, and the metric-trace part of the Einstein equations vanishes in this null contraction. Future stationarity sets $\delta\theta\to0$. To first order $\delta\theta$ is the derivative of the fractional area change, so, using the background area element $dA_0$,

$$
\delta A=\int dA_0\int_0^\infty\delta\theta\,d\lambda
=8\pi G\int dA_0\int_0^\infty\lambda\,\delta T_{ab}\ell^a\ell^b\,d\lambda.
$$

The integration by parts uses $[\lambda\delta\theta]_0^\infty=0$, guaranteed by the stated endpoint conditions.

The conserved [stress-energy current from a Killing vector](../../../../../../stress-energy-current-from-a-killing-vector.md) gives the absorbed mass and angular momentum, with signs

$$
\delta M=\int_{\mathcal N}\delta T_{ab}t^a\ell^b\,d\lambda\,dA_0,\qquad
\delta J=-\int_{\mathcal N}\delta T_{ab}\varphi^a\ell^b\,d\lambda\,dA_0.
$$

Consequently

$$
\delta M-\Omega_H\delta J
=\int_{\mathcal N}\delta T_{ab}\xi^a\ell^b\,d\lambda\,dA_0
=\kappa\int_{\mathcal N}\lambda\delta T_{ab}\ell^a\ell^b\,d\lambda\,dA_0,
$$

which proves the law. Any other escaping flux must be accounted for separately when identifying these absorbed charges with the changes in the black hole. Electric-charge variations would require the corresponding potential-charge term; they are excluded in this version. The convention $16\pi G=1$ in Question 1 is not needed here.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 311](../../../paper-311-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
