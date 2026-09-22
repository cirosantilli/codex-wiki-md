<h1 id="15c/solution">Solution</h1>

↑ **Parent:** [15C](../15c.md)

In electrostatic equilibrium, a nonzero [electric field](../../../../../electric-field.md) inside a conductor would move its free charges. Hence $E=0$ in the conducting material and the potential is constant throughout each connected conductor. Immediately outside its surface the tangential [electric field](../../../../../electric-field.md) is zero. A Gaussian pillbox across the surface gives

$$
(E_{\rm out}-E_{\rm in})\cdot n=\frac\sigma{\epsilon_0}.
$$

Since $E_{\rm in}=0$, the [electrostatic boundary conditions at a conductor](../../../../../electrostatic-boundary-conditions-at-a-conductor.md) give

$$
\boxed{\sigma=\epsilon_0E_{\rm out}\cdot n}.
$$

For the widely separated shells, let their charges be $Q_1,Q_2$. Their common potential requires

$$
\frac{Q_1}{4\pi\epsilon_0R_1}
=\frac{Q_2}{4\pi\epsilon_0R_2},
\qquad Q_1+Q_2=Q.
$$

Thus the [charge sharing between distant connected spheres](../../../../../charge-sharing-between-distant-connected-spheres.md) is

$$
\boxed{
Q_1=\frac{R_1}{R_1+R_2}Q,
\qquad
Q_2=\frac{R_2}{R_1+R_2}Q}.
$$

For the [charge on connected concentric spherical shells](../../../../../charge-on-connected-concentric-spherical-shells.md), the potentials at the two radii are

$$
\Phi(R_1)=\frac1{4\pi\epsilon_0}
\left(\frac{Q_1}{R_1}+\frac{Q_2}{R_2}\right),
\qquad
\Phi(R_2)=\frac{Q_1+Q_2}{4\pi\epsilon_0R_2}.
$$

Equality forces $Q_1=0$. Hence

$$
\boxed{Q_1=0,
\qquad Q_2=Q},
$$

so all charge lies on the exterior of the outer shell.

For the neutral sphere in the uniform field, the far-field condition gives $\alpha=-E$. Constancy of the potential on $r=R$ gives $\beta=ER^3$. Therefore

$$
\boxed{
\Phi(r,\theta)=-E\left(r-\frac{R^3}{r^2}\right)\cos\theta}.
$$

The outward normal field at the surface is

$$
E_r(R,\theta)
=-\left.\frac{\partial\Phi}{\partial r}\right|_{r=R}
=3E\cos\theta.
$$

The [induced charge on a conducting sphere in a uniform electric field](../../../../../induced-charge-on-a-conducting-sphere-in-a-uniform-electric-field.md) is consequently

$$
\boxed{\sigma(\theta)=3\epsilon_0E\cos\theta}.
$$

Finally,

$$
\int_{S^2}\sigma\,dA
=6\pi\epsilon_0ER^2\int_0^\pi
\cos\theta\sin\theta\,d\theta=0,
$$

confirming neutrality.

## ↑ Ancestors (10)

1. [15C](../15c.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ib](../../split.md)
4. [2024](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
