<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

The six critical [Fourier modes](../../../../../fourier-mode.md) are at $\pm\mathbf k_1,\pm\mathbf k_2,\pm\mathbf k_3$, with $\mathbf k_1+\mathbf k_2+\mathbf k_3=0$. Reality of the pattern pairs each positive-wavevector coefficient with the conjugate coefficient at the negative wavevector. The leading critical part of the [extended centre manifold](../../../../../extended-centre-manifold-for-a-parameter.md) parametrization is consequently

$$
u(\mathbf x,t)=\sum_{i=1}^3 A_i(t)e^{i\mathbf k_i\cdot\mathbf x}+\text{complex conjugate}+\text{slaved higher harmonics}.
$$

The displayed six-mode expression is its leading-order projection; nonlinear harmonics on the full [centre manifold](../../../../../center-manifold.md) need not vanish identically.

A translation $\mathbf d$ acts by $A_i\mapsto e^{i\mathbf k_i\cdot\mathbf d}A_i$. Each [monomial](../../../../../monomial.md) in the equation for $A_i$ must therefore carry wavevector $\mathbf k_i$. Since $-\mathbf k_{i+1}-\mathbf k_{i+2}=\mathbf k_i$, the allowed quadratic term is $A_{i+1}^*A_{i+2}^*$. At cubic order the allowed terms are $A_i|A_i|^2,A_i|A_{i+1}|^2,A_i|A_{i+2}|^2$. Rotation through $60$ degrees acts, with one choice of orientation, as

$$
(A_1,A_2,A_3)\longmapsto(A_2^*,A_3^*,A_1^*).
$$

Its square cyclically permutes the amplitudes, equating the coefficients across the three equations. Its cube conjugates every amplitude; [equivariance](../../../../../equivariant-map.md) under this half-turn makes all coefficients real. It does not interchange the two cross-coupling coefficients. A reflection would do that and force $b=c$, but that symmetry is expressly absent. Thus the [chiral hexagonal amplitude equations](../../../../../chiral-hexagonal-amplitude-equations.md) are

$$
\boxed{\dot A_i=\mu A_i+\alpha A_{i+1}^*A_{i+2}^*
-A_i(a|A_i|^2+b|A_{i+1}|^2+c|A_{i+2}|^2),}
$$

at the retained order, with cyclic indices and real coefficients. The missing opening modulus bar in the last cubic term of the printed formula must be supplied; phase [equivariance](../../../../../equivariant-map.md) requires $|A_{i+2}|^2$.

Write $A_i=r_ie^{i\phi_i}$, with all three amplitudes nonzero, and let $\Phi=\phi_1+\phi_2+\phi_3$. Separating real and imaginary parts gives

$$
\dot r_i=\mu r_i+\alpha r_{i+1}r_{i+2}\cos\Phi
-r_i(ar_i^2+br_{i+1}^2+cr_{i+2}^2),\qquad
\dot\phi_i=-\alpha\frac{r_{i+1}r_{i+2}}{r_i}\sin\Phi.
$$

Hence the [phase locking of a resonant hexagonal triad](../../../../../phase-locking-of-a-resonant-hexagonal-triad.md) obeys

$$
\dot\Phi=-\alpha\left(\frac{r_2r_3}{r_1}+\frac{r_3r_1}{r_2}+\frac{r_1r_2}{r_3}\right)\sin\Phi.
$$

For $\alpha>0$, $\Phi=0$ is phase stable and $\Phi=\pi$ is phase unstable. Two independent translation coordinates remove two phases; since the wavevectors sum to zero, the remaining phase is exactly $\Phi$. Thus **a stable fully active phase-locked pattern can be represented by three positive real amplitudes after choosing the spatial origin**. The statement is modulo translations, not a restriction on every representative. Boundary states must also be retained: the zero solution is stable for $\mu<0$, and rolls have two zero amplitudes. These are the necessary qualifications to a literal claim that all stable solutions are strictly positive.

In the real nonnegative subspace, a roll is

$$
\boxed{(A_1,A_2,A_3)=(r,0,0),\qquad r^2=\mu/a,\qquad\mu>0,}
$$

or a cyclic permutation. For hexagons let $s=a+b+c$, which is positive under the assumptions. The equal-amplitude branches solve $\mu+\alpha r-sr^2=0$, giving

$$
\boxed{r_\pm=\frac{\alpha\pm\sqrt{\alpha^2+4s\mu}}{2s},}
$$

with only positive roots retained. The upper branch exists for $\mu\geq-\alpha^2/(4s)$; the lower branch is positive for $-\alpha^2/(4s)\leq\mu<0$. They meet at a fold.

For a purported rectangle $(p,p,q)$ with $p,q>0$, subtract its first two equilibrium equations after dividing each by its own amplitude. The quadratic terms agree, and the difference is $(c-b)(p^2-q^2)=0$. Since $(b-a)(c-a)<0$ implies $b\ne c$, it forces $p=q$. A state with exactly two nonzero amplitudes is also impossible because the quadratic term drives the zero third amplitude. Thus **there are no nontrivial rectangles**.

In fact no other unequal positive equilibria are possible under the straddling cross-couplings. Here is the [uniqueness of positive hexagon equilibria with straddling cross-couplings](../../../../../uniqueness-of-positive-hexagon-equilibria-with-straddling-cross-couplings.md) argument. Put $x_i=r_i^2$, $p=r_1r_2r_3>0$. The equilibrium equations imply

$$
a x_i+b x_{i+1}+c x_{i+2}-\frac{\alpha p}{x_i}=\mu.
$$

Consider $b>a>c$, write $B=b-a>0$, $C=c-a<0$, and relabel cyclically so $x_1$ is maximal. If $x_2\geq x_3$, subtracting equations one and two gives

$$
B(x_2-x_3)+C(x_3-x_1)=\alpha p(1/x_1-1/x_2).
$$

The left side is positive unless all three are equal, while the right side is nonpositive. If $x_2\leq x_3$, subtract equations two and three instead:

$$
B(x_3-x_1)+C(x_1-x_2)=\alpha p(1/x_2-1/x_3).
$$

Now the left side is negative unless all are equal and the right side is nonnegative. Both cases force equality. For $c>a>b$, reverse the cyclic orientation and exchange $b,c$. Thus the only nonzero equilibria in this subspace are the stated rolls and hexagons.

At a roll the active radial [eigenvalue](../../../../../eigenvalue.md) is $-2\mu$. The two inactive amplitudes have real-part [linearization](../../../../../linearization.md)

$$
\begin{pmatrix}\mu(1-c/a)&\alpha r\\\alpha r&\mu(1-b/a)\end{pmatrix}.
$$

Its determinant is $\mu^2(a-c)(a-b)/a^2-\alpha^2\mu/a<0$. It therefore has a positive [eigenvalue](../../../../../eigenvalue.md): **the rolls are unstable for every $\mu>0$**, which is stronger than the large-$\mu$ conclusion. In the complex system there is also a neutral translation phase, and the imaginary transverse block has the same determinant.

At a positive hexagon the real-amplitude Jacobian is circulant, with diagonal $d=-2ar^2-\alpha r$ and off-diagonals $p=\alpha r-2br^2$, $q=\alpha r-2cr^2$. Its uniform [eigenvector](../../../../../eigenvector.md) $(1,1,1)$ has [eigenvalue](../../../../../eigenvalue.md)

$$
\lambda_{\parallel}=d+p+q=\alpha r-2sr^2.
$$

The other two [eigenvectors](../../../../../eigenvector.md) lie in the zero-sum subspace; using the two nontrivial cube roots of unity gives

$$
\boxed{\lambda_\pm=(b+c-2a)r^2-2\alpha r\ \pm i\sqrt3(b-c)r^2.}
$$

For sufficiently large $\mu$, $r\sim\sqrt{\mu/s}$, and the positive term $(b+c-2a)r^2$ dominates the quadratic-coupling term $2\alpha r$. Thus **the hexagons are unstable at large $\mu$**, while the uniform radial direction on the upper branch is stable. The two translation phases are neutral and the total phase has [eigenvalue](../../../../../eigenvalue.md) $-3\alpha r$, so the amplitude instability is genuine.

More precisely, the upper branch is amplitude stable between its fold and the [chiral hexagon Hopf threshold](../../../../../chiral-hexagon-hopf-threshold.md)

$$
r_H=\frac{2\alpha}{b+c-2a},\qquad
\mu_H=\frac{2\alpha^2(4a+b+c)}{(b+c-2a)^2}.
$$

At this threshold the conjugate pair crosses with nonzero frequency because $b\ne c$, permitting a [Hopf bifurcation](../../../../../hopf-bifurcation.md). The linear calculation locates the crossing; the nonlinear [normal form](../../../../../normal-form-dynamical-systems.md) decides the stability and direction of its periodic branch.

The dynamics are bounded in the retained model. For $S=r_1^2+r_2^2+r_3^2$ in the positive phase-locked subspace,

$$
\dot S=2\mu S+6\alpha r_1r_2r_3-2aS^2-2(b+c-2a)\sum_{i<j}r_i^2r_j^2.
$$

Since $r_1r_2r_3\leq(S/3)^{3/2}$, the negative quadratic-in-$S$ term dominates at large amplitude. For large positive $\mu$, the origin, rolls and hexagons are all unstable, so generic bounded dynamics cannot end at an asymptotically stable steady pattern. The chiral difference $b-c$ favors successive changes in dominant roll orientation, in the spirit of the [Küppers–Lortz instability](../../../../../kuppers-lortz-instability.md). Oscillatory competition or periodic switching is the natural behavior near the Hopf transition; linear stability alone does not establish a unique global limit cycle. With $\alpha=0$, coordinate planes are invariant and heteroclinic roll switching is possible. For $\alpha>0$ a missing third mode is regenerated when two others are present, so that exact boundary-plane heteroclinic picture is broken. Finally, sufficiently large $\mu$ is a conclusion of the cubic truncation; far from onset, omitted higher-order terms can change the physical pattern dynamics.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 70](../../paper-70-split.md)
3. [Iii](../../split.md)
4. [2009](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
