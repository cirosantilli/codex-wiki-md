<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

Use [static gauge](../../../../../static-gauge.md) for a [D3-brane](../../../../../d3-brane.md) in flat space and let $X(\mathbf x)$ be one physical transverse displacement. Put $\mathbf E=2\pi\alpha'\mathbf F_0$ and $\mathbf B_i=\pi\alpha'\varepsilon_{ijk}F_{jk}$, so the fields entering the [DBI action](../../../../../dirac-born-infeld-action.md) are dimensionless. With no magnetic field, writing $\mathbf v=\nabla X$ gives

$$
\mathcal L=-T_3\sqrt{1+|\mathbf v|^2-|\mathbf E|^2-|\mathbf E\times\mathbf v|^2}.
$$

Introduce the [dimensionless electric displacement in DBI theory](../../../../../dimensionless-electric-displacement-in-dbi-theory.md), $\mathbf d=T_3^{-1}\partial\mathcal L/\partial\mathbf E$. Its [Hamiltonian density](../../../../../hamiltonian-density.md) obeys the [DBI Hamiltonian bound for an electric spike](../../../../../dbi-hamiltonian-bound-for-an-electric-spike.md):

$$
\left(\frac{\mathcal H}{T_3}\right)^2
=1+|\mathbf v|^2+|\mathbf d|^2+(\mathbf d\cdot\mathbf v)^2
=(1+\mathbf d\cdot\mathbf v)^2+|\mathbf d-\mathbf v|^2.
$$

The electric bound is saturated when $\mathbf d=\pm\nabla X$. On that locus the constitutive relation also gives $\mathbf E=\mathbf d$. With the [Gauss law constraint in gauge theory](../../../../../gauss-law-constraint-in-gauge-theory.md) away from charges, the electric [BPS equations for a one-scalar D3-brane](../../../../../bps-equations-for-a-one-scalar-d3-brane.md) are therefore

$$
\boxed{\mathbf E=\pm\nabla X,\qquad\mathbf B=0,\qquad\Delta X=0.}
$$

The magnetic version is $\mathbf B=\pm\nabla X$, $\mathbf E=0$. More generally, one constant charge angle gives the aligned dyonic branch $\mathbf E=\cos\vartheta\,\nabla X$, $\mathbf B=\sin\vartheta\,\nabla X$ with $X$ harmonic. A single aligned electric, magnetic or dyonic spike preserves eight of the D3 vacuum's sixteen [supersymmetry generators](../../../../../supersymmetry-generator.md). Thus “one-half BPS” here means one-half of the linearly realized worldvolume supersymmetry; the string–D3 configuration preserves one-quarter of the thirty-two spacetime supersymmetries.

The electric [BIon](../../../../../born-infeld-soliton.md) is the single-centre harmonic solution

$$
\boxed{X=X_\infty+\frac c r,\qquad\mathbf E=\pm\nabla X,\qquad
c=\pi g_s|N|\alpha'.}
$$

The sign fixes its electric charge and spike orientation. The scalar is an actual transverse coordinate, so $X\to\infty$ as $r\to0$ describes a long narrow spike emerging from an asymptotically planar [D3-brane](../../../../../d3-brane.md). It carries $|N|$ [fundamental strings](../../../../../fundamental-string.md) ending on the brane. A magnetic [BIon](../../../../../born-infeld-soliton.md) similarly represents [D1-branes](../../../../../d1-brane.md), and an aligned dyonic [BIon](../../../../../born-infeld-soliton.md) represents a [(p,q) string](../../../../../p-q-string.md).

The [string-tension interpretation of BIon energy](../../../../../string-tension-interpretation-of-bion-energy.md) follows explicitly. With $T_3=[(2\pi)^3g_s\alpha'^2]^{-1}$, the energy above the planar-brane vacuum outside a small radius $r_0$ is

$$
\Delta E=T_3\int_{r\geq r_0}|\nabla X|^2d^3x
=\frac{4\pi T_3c^2}{r_0}
=|N|T_{F1}\bigl(X(r_0)-X_\infty\bigr),\qquad T_{F1}=\frac1{2\pi\alpha'}.
$$

Its divergence is the energy of a semi-infinite string, with the correct finite tension. For a magnetic spike, $c=\pi|N|\alpha'$ instead, and the same calculation gives the [D1-brane](../../../../../d1-brane.md) tension $1/(2\pi g_s\alpha')$. The solution solves the full nonlinear [DBI action](../../../../../dirac-born-infeld-action.md), not just its weak-field expansion.

<a id="4/image-bion-geometry-a-d3-brane-develops-a-narrow-spike-carrying-string-charge"></a>
![](../../../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-57-bion-spike.png)

**[Figure 1](#4/image-bion-geometry-a-d3-brane-develops-a-narrow-spike-carrying-string-charge). BIon geometry: a D3-brane develops a narrow spike carrying string charge**.

The [validity of the abelian BIon approximation](../../../../../validity-of-the-abelian-bion-approximation.md) concerns its [derivative expansion](../../../../../derivative-expansion.md), string loops and gravitational backreaction. Large field strengths are included by the [DBI action](../../../../../dirac-born-infeld-action.md), but rapidly varying field strengths and embedding curvature require corrections. Far outside the singular core these corrections can be small. The transition region has $r\sim\sqrt c$; an electric throat can be parametrically controlled with $|N|g_s\gg1$ while keeping gravitational backreaction small with $g_s^2|N|\ll1$. For a magnetic throat the corresponding conditions are $|N|\gg1$ and $g_s|N|\ll1$. The weak-coupling and large-charge windows allow both requirements. The ideal $r\to0$ tip is not uniformly controlled by the single abelian effective action, so one should not infer exact microscopic core physics solely from its formal singularity.

Less supersymmetry survives when independent, compatible geometric or charge projectors must hold simultaneously. A useful purely geometric family is a [D3-brane](../../../../../d3-brane.md) whose spatial worldvolume is a [special Lagrangian submanifold](../../../../../special-lagrangian-submanifold.md) of $\mathbb C^3$. In a graph $z^i=x^i+iY^i(\mathbf x)$, the conditions are

$$
\omega|_\Sigma=0,\qquad\operatorname{Im}\Omega|_\Sigma=0,\qquad
\operatorname{Re}\Omega|_\Sigma=\operatorname{vol}_\Sigma,
\qquad \Omega=dz^1\wedge dz^2\wedge dz^3.
$$

The first condition makes $\partial_iY^j$ symmetric, so locally $Y=\nabla f$. Pulling back $\Omega$ gives $\det(I+iD^2f)\,dx^1\wedge dx^2\wedge dx^3$. Hence the phase-zero [special Lagrangian graph equation](../../../../../special-lagrangian-graph-equation.md) is

$$
\boxed{\Delta f=\det(D^2f),\qquad
1-\sigma_2(D^2f)>0,}
$$

where $\sigma_2$ is the sum of the pairwise products of the three Hessian [eigenvalues](../../../../../eigenvalue.md). The positive real branch fixes the orientation. These curved D3 geometries minimize volume by their [calibration](../../../../../calibration-differential-geometry.md) $\operatorname{Re}\Omega$ and generically preserve four spacetime supersymmetries, one-quarter of the D3 worldvolume supersymmetry. Special flat graphs can preserve more.

The generic count follows from the common tangent-plane projectors. With complex coordinate pairs $(1,4),(2,5),(3,6)$, the phase-preserving rotations require $(\Gamma_{14}-\Gamma_{25})\epsilon=0$ and $(\Gamma_{14}-\Gamma_{36})\epsilon=0$. Multiplication by $\Gamma_{14}$ turns these into two independent commuting involution conditions with eigenvalue $-1$. Each halves the sixteen-dimensional planar D3 eigenspace, leaving $16/2^2=4$. This is an intersection of compatible [kappa symmetry projectors](../../../../../kappa-symmetry-projector.md), rather than a count based on the rank of a single projector at one point.

Charge-carrying examples include compatible networks of differently oriented [(p,q) strings](../../../../../p-q-string.md) ending on D3-branes. At each [string junction](../../../../../string-junction.md), charge vectors add to zero and tension vectors balance; their directions and charge phases must also give common [kappa symmetry projectors](../../../../../kappa-symmetry-projector.md). They can impose further independent conditions beyond the planar D3 projector. Geometrically, several transverse scalar profiles describe the corresponding spikes and intersections. Merely replacing one electric spike by an aligned dyonic spike does not lower its preserved fraction; additional independent conditions are what reduce the common [Killing spinor](../../../../../killing-spinor.md) space.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 57](../../paper-57-split.md)
3. [Iii](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
