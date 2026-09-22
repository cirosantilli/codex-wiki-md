<h1 id="4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For $\lambda>0$ put $s=\sqrt\lambda$. The [equilibrium points](../../../../../../equilibrium-point-of-a-dynamical-system.md) are $(s,0)$ and $(-s,0)$, with

$$
J(x_*,0)=\begin{pmatrix}0&1\\2x_*&\mu+x_*\end{pmatrix},\quad
\det J=-2x_*,\quad\operatorname{tr}J=\mu+x_*.
$$

The positive branch is always a saddle. The negative branch is a sink for $\mu<s$ and a source for $\mu>s$; it is a node or focus according as $(\mu-s)^2-8s$ is positive or negative. At $\lambda=0$ the two branches meet in a [saddle-node bifurcation](../../../../../../saddle-node-bifurcation.md) when $\mu\ne0$; at $(\lambda,\mu)=(0,0)$ the double zero [eigenvalue](../../../../../../eigenvalue.md) with a nontrivial Jordan block gives a [Bogdanov–Takens bifurcation](../../../../../../bogdanov-takens-bifurcation.md). There are no real [equilibrium points](../../../../../../equilibrium-point-of-a-dynamical-system.md) for $\lambda<0$.

The [Hopf bifurcation](../../../../../../hopf-bifurcation.md) curve is $\mu=s>0$, equivalently $\lambda=\mu^2$ on its positive-$\mu$ branch. Its frequency is $\omega=\sqrt{2s}$. To determine the direction, shift $u=x+s$, $v=y$ at this threshold; then

$$
\dot u=v,\qquad \dot v=-\omega^2u+u^2+uv.
$$

Set $X=u$, $Y=-v/\omega$ to obtain $\dot X=-\omega Y$, $\dot Y=\omega X-X^2/\omega+XY$. A quadratic near-identity transformation, or harmonic averaging with its quadratic correction retained, gives the radial cubic coefficient

$$
\ell_H=\frac{-g_{XY}g_{XX}}{16\omega}
=\frac1{8\omega^2}>0,
$$

where $g=-X^2/\omega+XY$. The radial equation is $\dot R=(\mu-s)R/2+\ell_H R^3+\cdots$. Hence the [Hopf bifurcation](../../../../../../hopf-bifurcation.md) is **subcritical**, with an unstable small [periodic orbit](../../../../../../periodic-orbit.md) on the stable-focus side $\mu<s$.

The saddle's outgoing separatrix can return to its incoming separatrix, creating a [homoclinic orbit](../../../../../../homoclinic-orbit.md). This [global bifurcation](../../../../../../global-bifurcation.md) cannot be detected from the [equilibrium point](../../../../../../equilibrium-point-of-a-dynamical-system.md)'s [Jacobian matrix](../../../../../../jacobian-matrix.md) alone. The weakly Hamiltonian scaling below locates its curve and shows how the unstable Hopf cycle grows into the saddle loop. The final diagram includes the local saddle-node and Hopf curves and this global curve; it describes the neighborhood of the double-zero point.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [4](../../4.md)
3. [Paper 65](../../../paper-65-split.md)
4. [Iii](../../../split.md)
5. [2005](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
