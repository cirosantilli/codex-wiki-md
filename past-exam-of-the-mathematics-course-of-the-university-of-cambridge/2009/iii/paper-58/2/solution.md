<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Choose a local [orthonormal coframe](../../../../../orthonormal-coframe-in-spacetime.md) $e^A$ with $g=\eta_{AB}e^Ae^B$. The [Levi-Civita connection](../../../../../levi-civita-connection.md) is represented by the [connection 1-forms](../../../../../connection-1-form-split.md) satisfying

$$
de^A+\omega^A{}_B\wedge e^B=0,\qquad \omega_{AB}=\eta_{AC}\omega^C{}_B=-\omega_{BA}.
$$

The [gamma matrices](../../../../../gamma-matrices.md) satisfy the [Clifford algebra](../../../../../clifford-algebra.md) relations $\{\gamma^A,\gamma^B\}=2\eta^{AB}I$. The matrices $\tfrac14[\gamma^A,\gamma^B]$ represent the infinitesimal orthogonal transformations on [spinor fields](../../../../../spinor-field.md); lifting the frame connection to this representation defines the [spinor covariant derivative](../../../../../spinor-covariant-derivative.md)

$$
\boxed{\nabla_\mu\epsilon=\partial_\mu\epsilon+\frac14\omega_{\mu AB}\gamma^A\gamma^B\epsilon
=\partial_\mu\epsilon+\frac18\omega_{\mu AB}[\gamma^A,\gamma^B]\epsilon.}
$$

Both frame indices are summed, so each antisymmetric pair occurs twice. Under a [local Lorentz transformation](../../../../../local-lorentz-transformation.md) with spin lift $S$, the [spin connection](../../../../../spin-connection.md) transforms as $\Omega_\mu\mapsto S\Omega_\mu S^{-1}-(\partial_\mu S)S^{-1}$ and $\epsilon\mapsto S\epsilon$; consequently $\nabla_\mu\epsilon\mapsto S\nabla_\mu\epsilon$. This establishes covariance. Global construction requires a compatible [spin structure](../../../../../spin-structure.md) (and the appropriate [orientation](../../../../../orientation-of-a-simplex.md) and [time orientation](../../../../../time-orientation.md)); the formulas themselves work on a local [orthonormal frame](../../../../../orthonormal-frame-in-spacetime.md) patch.

The supplied [gamma matrices](../../../../../gamma-matrices.md) have squares $-I,I,I$ and anticommute pairwise, so $\eta=\operatorname{diag}(-1,1,1)$. Work on a connected regular patch with $r>0$ and $V\ne0$. Since the metric depends only on $V^2$, we may use its positive smooth square root $V>0$. Take

$$
e^0=V\,dt,\qquad e^1=dr/V,\qquad e^2=r\,d\theta.
$$

Their [exterior derivatives](../../../../../exterior-derivative.md) are $de^0=-V'e^0\wedge e^1$, $de^1=0$, and $de^2=(V/r)e^1\wedge e^2$. Solving [Cartan's first structure equation](../../../../../cartan-s-first-structure-equation.md) and imposing [Lorentzian connection-form antisymmetry](../../../../../lorentzian-connection-form-antisymmetry.md) gives

$$
\omega^0{}_1=\omega^1{}_0=VV'\,dt,\qquad \omega^2{}_1=V\,d\theta,\qquad \omega^1{}_2=-V\,d\theta.
$$

In particular $\omega_{01}=-VV'\,dt$ and $\omega_{12}=-V\,d\theta$. The [parallel spinor](../../../../../parallel-spinor.md) equations are therefore

$$
\partial_t\epsilon-\frac{VV'}2\gamma^0\gamma^1\epsilon=0,\qquad
\partial_r\epsilon=0,\qquad
\partial_\theta\epsilon-\frac V2\gamma^1\gamma^2\epsilon=0.
$$

Differentiate the angular equation with respect to $r$ and use $\partial_r\epsilon=0$. This gives $V'\gamma^1\gamma^2\epsilon=0$. Since $(\gamma^1\gamma^2)^2=-I$, this matrix is invertible. A [parallel spinor](../../../../../parallel-spinor.md) that vanishes at any point vanishes everywhere on the connected domain, by uniqueness of [parallel transport](../../../../../parallel-transport.md). Thus a nonzero [parallel spinor](../../../../../parallel-spinor.md) implies $V'=0$ throughout the patch. **There are no nonzero parallel spinors unless $V$ is constant.** The zero [spinor field](../../../../../spinor-field.md) is always a solution, so “nonzero” is essential in interpreting the printed assertion. A smooth original $V$ of either sign is constant on such a patch exactly when $|V|$ is constant; $V=0$ is excluded because the given metric is not defined there.

Write the constant as $c=|V|>0$, and introduce $T=ct$, $\rho=r/c$, and $\phi=c\theta$. The metric becomes

$$
ds^2=-dT^2+d\rho^2+\rho^2d\phi^2.
$$

A circle at small $\rho$ has circumference $cP\rho$ if $\theta$ has period $P$, whereas its proper radius is $\rho$. Smoothness requires circumference divided by radius to tend to $2\pi$, not a multiple of $2\pi$. Conversely, when $cP=2\pi$, the coordinates $X=\rho\cos\phi$, $Y=\rho\sin\phi$ exhibit a smooth flat spatial disk. Hence

$$
\boxed{\theta\ \text{must have period }2\pi/c.}
$$

For a prescribed period $2\pi$, this requires $c=1$; otherwise there is a [conical singularity](../../../../../conical-singularity.md) at the apex.

For constant $V=c$, the time and radial equations make the components independent of $t,r$. The angular equation has all solutions

$$
\boxed{\epsilon(t,r,\theta)=\exp\!\left(\frac{c\theta}2\gamma^1\gamma^2\right)\epsilon_0
=\left[\cos\frac{c\theta}2\,I-\sin\frac{c\theta}2\,\gamma^0\right]\epsilon_0,}
$$

where $\epsilon_0$ is an arbitrary constant two-component [spinor field](../../../../../spinor-field.md) and $\gamma^1\gamma^2=-\gamma^0$. There are two independent real solutions for real [spinor fields](../../../../../spinor-field.md), or two independent complex solutions if complex spinors are used. At the smooth angular period, these polar-frame components change sign. This is exactly the [polar-frame parallel spinor](../../../../../polar-frame-parallel-spinor.md) transformation under the spin lift of a full rotation: the rotating polar [orthonormal frame](../../../../../orthonormal-frame-in-spacetime.md) does not extend through the origin. The [spin structure](../../../../../spin-structure.md) extending over the disk uses this antiperiodic polar trivialization; in a Cartesian [orthonormal frame](../../../../../orthonormal-frame-in-spacetime.md) the same [parallel spinors](../../../../../parallel-spinor.md) have constant components and extend smoothly. Requiring periodic components in the rotating frame would select the other spin structure on the punctured disk, which does not extend over its center.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 58](../../paper-58-split.md)
3. [Iii](../../split.md)
4. [2009](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
