<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Use the natural [dihedral group](../../../../../../dihedral-group.md) generators $\rho z=e^{2\pi i/n}z$ and $mz=\bar z$, and orient the unfolding parameter so the trivial [equilibrium](../../../../../../equilibrium-point-of-a-dynamical-system.md) loses stability as $\mu$ increases through zero. Rotation equivariance requires a [monomial](../../../../../../monomial.md) $z^p\bar z^q$ in $\dot z$ to have $p-q\equiv1\pmod n$, while reflection makes its coefficient real. These constraints give the [dihedral steady-state normal form](../../../../../../dihedral-steady-state-normal-form.md). The reflection axes have angles $\theta=k\pi/n$ and one-dimensional [fixed-point subspaces of a group action](../../../../../../fixed-point-subspace-of-a-group-action.md); their [equilibria](../../../../../../equilibrium-point-of-a-dynamical-system.md) are the branches guaranteed by the [equivariant branching lemma](../../../../../../equivariant-branching-lemma.md).

For $n=3$, a generic quadratic anisotropy dominates:

$$
\dot z=\mu z+b\bar z^2+a z|z|^2+\cdots,\qquad b\ne0.
$$

In [polar coordinates](../../../../../../polar-coordinates.md), $\dot r=\mu r+br^2\cos3\theta+O(r^3)$ and $\dot\theta=-br\sin3\theta+O(r^2)$. At a nonzero [equilibrium](../../../../../../equilibrium-point-of-a-dynamical-system.md), $\chi=\cos3\theta=\pm1$ and $r=-\mu/(b\chi)+O(\mu^2)>0$. There are three symmetry-related [equilibria](../../../../../../equilibrium-point-of-a-dynamical-system.md) on each parameter side, on opposite half-axes as the sign of $\mu$ changes. The radial and angular [eigenvalues](../../../../../../eigenvalue.md) are $-\mu+O(\mu^2)$ and $3\mu+O(\mu^2)$, respectively. Hence **all three nonzero branches are saddles in the full plane**, even though radial stability exchanges at the crossing. The origin is a sink for $\mu<0$ and a source for $\mu>0$. The reflection [normaliser](../../../../../../normalizer.md) has no residual sign reversal in this odd dihedral case, so these are transcritical-like branches, not symmetry-forced pitchforks.

For $n=4$, both relevant nonlinearities are cubic:

$$
\dot z=\mu z+a z|z|^2+b\bar z^3+O(|z|^5),\qquad
\dot r=r\bigl(\mu+(a+b\cos4\theta)r^2\bigr),\quad
\dot\theta=-br^2\sin4\theta.
$$

There are two conjugacy classes of reflection isotropy: the coordinate axes, with $\chi=\cos4\theta=1$, and the diagonals, with $\chi=-1$. Generically $b\ne0$ and $a\pm b\ne0$. Each class has a [pitchfork bifurcation](../../../../../../pitchfork-bifurcation-normal-form.md), with four symmetry-related [equilibria](../../../../../../equilibrium-point-of-a-dynamical-system.md) when its squared radius is positive:

$$
\boxed{r_\chi^2=-\frac\mu{a+b\chi},\qquad
\rho_{\mathrm{rad}}=-2\mu,\qquad
\rho_{\mathrm{ang}}=-4b\chi r_\chi^2.}
$$

These formulas give all generic existence and stability cases. If $a<-|b|$, both classes emerge for $\mu>0$; the class with $b\chi>0$ consists of stable nodes and the other of saddles. If $a>|b|$, both classes exist for $\mu<0$; the class with $b\chi>0$ consists of saddles and the other of sources. If $|a|<|b|$, one class exists on each side and both consist of saddles. Equality $a=\pm b$ is nongeneric and requires higher-order terms. Unlike the odd dihedral cases, the residual [normaliser](../../../../../../normalizer.md) quotient contains a sign reversal, enforcing exact paired pitchfork branches.

For $n=5$, cubic radial saturation occurs before the first angular anisotropy:

$$
\dot z=\mu z+a z|z|^2+b\bar z^4+O(|z|^5),\qquad
\dot r=r\bigl(\mu+a r^2+b r^3\cos5\theta+\cdots\bigr),\quad
\dot\theta=-br^3\sin5\theta+\cdots.
$$

For generic $a,b\ne0$, ten [equilibria](../../../../../../equilibrium-point-of-a-dynamical-system.md) lie on the reflection half-axes whenever $-\mu/a>0$, divided into two distinct five-point group orbits. Their radii and [eigenvalues](../../../../../../eigenvalue.md) are

$$
r_\chi=\sqrt{-\mu/a}+O(\mu),\qquad
\rho_{\mathrm{rad}}=-2\mu+O(|\mu|^{3/2}),\qquad
\rho_{\mathrm{ang}}=-5b\chi r_\chi^3+O(r_\chi^4),\quad\chi=\pm1.
$$

If $a<0$, they emerge for $\mu>0$: the five with $b\chi>0$ are stable nodes and the other five are saddles. If $a>0$, they exist for $\mu<0$: the five with $b\chi>0$ are saddles and the others are sources. The leading amplitude scaling is pitchfork-like, but the quartic term distinguishes opposite half-axes and generally gives different corrections to their radii; there is no exact sign-reversal symmetry on an individual fixed line. Thus **$D_3$ has quadratic saddle branches, $D_4$ has two cubic axial branch types, and $D_5$ has cubic radial branches whose angular stability splits at quartic order**.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 85](../../../paper-85-split.md)
4. [Iii](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
