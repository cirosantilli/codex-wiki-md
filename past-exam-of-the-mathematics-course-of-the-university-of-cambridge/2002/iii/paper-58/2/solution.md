<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Use a real physical field, so the three positive [wavevectors](../../../../../wavevector.md) are accompanied by their complex-conjugate modes. Modulo lattice translations, the effective [symmetry group](../../../../../symmetry-group.md) is $G=\mathbb T^2\rtimes C_6$. Its translation [group action](../../../../../group-action.md) is

$$
T_{\theta_1,\theta_2}(A,B,C)=(e^{i\theta_1}A,e^{i\theta_2}B,e^{-i(\theta_1+\theta_2)}C).
$$

A $120^\circ$ rotation cyclically permutes the amplitudes; a half-turn $\kappa$ acts by simultaneous [complex conjugation](../../../../../complex-conjugation.md). Together these generate the sixfold rotation group. These formulas specify the [group action](../../../../../group-action.md) independently of the choice of orientation of the three [wavevectors](../../../../../wavevector.md).

For a nonzero real hexagon $(h,h,h)$, its [stabilizer subgroup](../../../../../stabilizer-subgroup.md) is the rotation group $C_6$. A translation fixes it only when all three phase factors equal one. Cyclic permutation forces a fixed vector to have equal components, and the half-turn forces those components to be real. Therefore $\operatorname{Fix}(C_6)=\{(a,a,a):a\in\mathbb R\}$. For a roll $(r,0,0)$ with nonzero real $r$, the [stabilizer subgroup](../../../../../stabilizer-subgroup.md) consists of the translations $T_{0,\theta}$ and the half-turn, with $\kappa T_{0,\theta}\kappa=T_{0,-\theta}$. It is $S^1\rtimes C_2$, isomorphic to $O(2)$ as an abstract group even though spatial reflections are absent. The circle eliminates $B,C$ from its [fixed-point subspace of a group action](../../../../../fixed-point-subspace-of-a-group-action.md), and the half-turn makes $A$ real. Thus

$$
\boxed{\operatorname{Fix}(H_{\rm hex})=\mathbb R(1,1,1),\qquad
\operatorname{Fix}(H_{\rm roll})=\mathbb R(1,0,0).}
$$

If unreduced physical translations are used, the full lattice kernel is included in both [stabilizer subgroups](../../../../../stabilizer-subgroup.md). The real representation on the six critical components is absolutely irreducible: translations distinguish the three Fourier pairs, rotations permute them, and the half-turn rules out a complex scalar in the commutant. The [equivariant branching lemma](../../../../../equivariant-branching-lemma.md) consequently supplies generic steady branches of both axial types at a transverse crossing of the common linear [eigenvalue](../../../../../eigenvalue.md). It guarantees existence, not stability or exhaustiveness of the possible branches.

Translation equivariance severely restricts the monomials in $\dot A$. Through cubic order they are $A$, $\overline B\,\overline C$, $|A|^2A$, $|B|^2A$ and $|C|^2A$: each has the same translation weight as $A$, using $\mathbf k_1+\mathbf k_2+\mathbf k_3=0$. The half-turn forces their coefficients to be real; the $120^\circ$ rotation gives the two cyclic counterpart equations. A spatial reflection would interchange $B,C$ and require equal cross-couplings, but it is not a symmetry here. After a real amplitude rescaling makes the generic nonzero quadratic coefficient one, the [rotational hexagon amplitude equations](../../../../../rotational-hexagon-amplitude-equations.md) are

$$
\dot A=\mu A+\overline B\,\overline C-\nu_1|A|^2A-(\nu_2+\delta)|B|^2A-(\nu_2-\delta)|C|^2A,
$$

with the other two equations obtained by cyclic permutation. All four coefficients are real; $\delta$ records the absence of spatial reflection. The normalization assumes the resonant quadratic coefficient is nonzero; its vanishing would be an additional degeneracy.

For the roll, $r^2=\mu/\nu_1$. The radial [eigenvalue](../../../../../eigenvalue.md) is $-2\mu$ and the phase of the active mode is a neutral translation. The transverse variables $(b,\overline c)$ have matrix

$$
\begin{pmatrix}\mu-(\nu_2-\delta)r^2&r\\r&\mu-(\nu_2+\delta)r^2\end{pmatrix}.
$$

Its two real [eigenvalues](../../../../../eigenvalue.md), each occurring twice in the full real linearization, are $-(\nu_2-\nu_1)r^2\pm\sqrt{\delta^2r^4+r^2}$. Define $d=\nu_2-\nu_1$ and $D_r=d^2-\delta^2$. Strict attraction modulo translation is therefore equivalent to

$$
\boxed{\nu_1>0,\quad \mu>0,\quad d>0,\quad D_r>0,\quad
\mu>\frac{\nu_1}{D_r}.}
$$

Indeed the larger transverse [eigenvalue](../../../../../eigenvalue.md) is negative precisely when $dr^2>\sqrt{\delta^2r^4+r^2}$, and squaring is legitimate only after requiring $d>0$. If $\delta^2>d^2$, that inequality is impossible. Equality $\delta^2=d^2$ is also insufficient because of the additional positive term $r^2$. Any nonzero roll that exists with $\nu_1<0$ already has a positive radial [eigenvalue](../../../../../eigenvalue.md); the degenerate case $\nu_1=0$ has no ordinary isolated nonzero roll branch.

For hexagons put $N=\nu_1+2\nu_2$. A nonzero real amplitude $h$ satisfies $\mu=Nh^2-h$, or $h=(1\pm\sqrt{1+4N\mu})/(2N)$ when $N\ne0$. Separate real and imaginary disturbances. The real [Jacobian matrix](../../../../../jacobian-matrix.md) is cyclic, with diagonal $-h-2\nu_1h^2$ and off-diagonal entries $h-2(\nu_2\pm\delta)h^2$. Its [eigenvalues](../../../../../eigenvalue.md) are

$$
\lambda_s=h-2Nh^2,\qquad
\lambda_\pm=-2h+2dh^2\pm2i\sqrt3\delta h^2.
$$

The imaginary [Jacobian matrix](../../../../../jacobian-matrix.md) has every entry equal to $-h$, giving [eigenvalues](../../../../../eigenvalue.md) $-3h,0,0$. The two zero modes translate the hexagonal pattern. Thus the general strict stability conditions for any nonzero root $h$ are

$$
\boxed{h>0,\qquad 2Nh>1,\qquad dh<1,\qquad \mu=Nh^2-h.}
$$

These conditions state [orbital stability](../../../../../orbital-stability.md) transverse to translations, not asymptotic convergence to one prescribed spatial phase. Equalities require a nonlinear bifurcation calculation.

When $\nu_2>\nu_1>0$, both $d,N$ are positive. The upper positive hexagon branch is radially stable after its [saddle-node bifurcation](../../../../../saddle-node-bifurcation.md) at $\mu=-1/(4N)$, $h=1/(2N)$; it remains stable until $h=1/d$. At this second threshold the pair $\lambda_\pm$ crosses the imaginary axis with nonzero frequency if $\delta\ne0$. The crossing is transverse, since $dh/d\mu=1/(2Nh-1)$ and the derivative of $-2h+2dh^2$ with respect to $h$ is two there. Hence, subject to the usual nonzero cubic coefficient, this is a [Hopf bifurcation](../../../../../hopf-bifurcation.md):

$$
\boxed{\mu_H=\frac{2\nu_1+\nu_2}{(\nu_2-\nu_1)^2},\qquad
\omega_H=\frac{2\sqrt3|\delta|}{(\nu_2-\nu_1)^2}.}
$$

For $\delta=0$ the same threshold has two zero real [eigenvalues](../../../../../eigenvalue.md), so it is not a Hopf bifurcation.

A possible [phase portrait](../../../../../phase-portrait.md) when neither steady branch is stable has an attracting periodic oscillation surrounding the unstable hexagon, with the three amplitudes waxing and waning cyclically. This is realized, for example, by $\nu_1=1$, $\nu_2=2$, $\delta=2$ just above $\mu_H=4$. Rolls are unstable for every positive $\mu$ because $\delta^2=4>d^2=1$. At the hexagon Hopf point $h=1$, the real spectrum is $-9,\pm4i\sqrt3$. Evaluation of the cubic [Hopf normal form](../../../../../hopf-normal-form.md) with a unit-norm critical eigenvector gives $\operatorname{Re}G_{21}=-64/27<0$, so this example has a [supercritical Hopf bifurcation](../../../../../supercritical-hopf-bifurcation.md) and an attracting small [limit cycle](../../../../../limit-cycle.md) in the real invariant subspace. The figure shows such a cycle at $\mu=4.2$ and an approaching trajectory; the positive octant is forward invariant because an amplitude's derivative at zero is the product of the other two. This is a possible portrait, rather than a claim that every parameter set with unstable rolls and hexagons has the same attractor. Stability asserted for the periodic orbit here is within the stipulated real subspace.

<a id="2/image-a-possible-real-amplitude-phase-portrait-an-attracting-oscillating-hexagon-with-unstable-steady-hexagon-and-roll-states"></a>
![](../../../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-58-oscillating-hexagons.png)

**[Figure 2](#2/image-a-possible-real-amplitude-phase-portrait-an-attracting-oscillating-hexagon-with-unstable-steady-hexagon-and-roll-states). A possible real-amplitude phase portrait: an attracting oscillating hexagon with unstable steady hexagon and roll states**.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 58](../../paper-58-split.md)
3. [Iii](../../split.md)
4. [2002](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
