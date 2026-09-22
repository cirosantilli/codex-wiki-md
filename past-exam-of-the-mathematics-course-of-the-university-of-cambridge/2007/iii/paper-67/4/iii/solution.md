<h1 id="4/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Choose a signed angular coordinate along the source-lens line. The [singular isothermal sphere lens](../../../../../../singular-isothermal-sphere-lens.md) equation is

$$
\beta=\theta-\theta_E\operatorname{sgn}\theta.
$$

For $\beta>0$, the positive image is $\theta_+=\beta+\theta_E$. A negative image would require $\theta_-=\beta-\theta_E<0$, which is possible only for $\beta<\theta_E$. Here $\beta=4$ arcmin and $\theta_E=1$ arcmin, so **there is only one image, at $\theta=5$ arcmin**. Formally using the negative-image formula would produce a positive value, inconsistent with the branch from which it was obtained.

The paper defines its vector deflection as source minus image angle, $\boldsymbol\alpha_{\rm paper}=(\beta-\theta)\hat{\boldsymbol\theta}$. This is the negative of the usual reduced deflection in $\boldsymbol\beta=\boldsymbol\theta-\boldsymbol\alpha_{\rm standard}$. Therefore its relation to [lensing convergence](../../../../../../lensing-convergence.md) is

$$
\boxed{\kappa=-\frac12\nabla_\theta\cdot\boldsymbol\alpha_{\rm paper}.}
$$

For the [SIS](../../../../../../singular-isothermal-sphere.md), $\boldsymbol\alpha_{\rm paper}=-\theta_E\hat{\boldsymbol\theta}$. The two-dimensional polar-coordinate divergence gives

$$
\nabla_\theta\cdot\boldsymbol\alpha_{\rm paper}
=\frac1\theta\frac{d}{d\theta}(-\theta_E\theta)=-\frac{\theta_E}{\theta},
\qquad \boxed{\kappa=\frac{\theta_E}{2\theta}.}
$$

Using a plus sign with the printed inward deflection would incorrectly give negative convergence.

For a small intrinsically circular source, differentiate the [thin gravitational lens equation](../../../../../../thin-gravitational-lens-equation.md). The radial and tangential source-image [Jacobian matrix](../../../../../../jacobian-matrix.md) eigenvalues are

$$
\lambda_r=1,\qquad \lambda_t=1-\frac{\theta_E}{\theta}.
$$

Thus the image is stretched tangentially around the lens centre, with no radial stretch in this idealized model. At $\theta=5$ arcmin, $\lambda_t=4/5$; the image is an ellipse with tangential-to-radial axis ratio $5/4$. It is not a complete ring. This local description assumes a source small enough that the Jacobian is nearly constant across it.

The signed [lensing magnification](../../../../../../lensing-magnification.md) is

$$
\mu=\frac1{(1-\kappa)^2-|\gamma|^2}.
$$

Since the [lensing shear](../../../../../../lensing-shear.md) magnitude equals $\kappa$, it reduces to $\mu=(1-2\kappa)^{-1}$. At the image, $\kappa=\theta_E/(2\theta)=1/10$, hence

$$
\boxed{\mu=\frac1{1-1/5}=\frac54=1.25.}
$$

The image has positive parity and is $25\%$ brighter for the same intrinsic source. [Gravitational lensing](../../../../../../gravitational-lensing.md) preserves [surface brightness](../../../../../../surface-brightness.md), so this flux amplification follows from its larger apparent solid angle. In evaluating the convergence, use the image angle $5$ arcmin, not the source angle $4$ arcmin.

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [4](../../4.md)
3. [Paper 67](../../../paper-67-split.md)
4. [Iii](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
