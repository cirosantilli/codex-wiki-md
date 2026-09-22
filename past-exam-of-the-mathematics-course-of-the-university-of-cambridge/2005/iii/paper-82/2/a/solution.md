<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Assume the coefficients are sufficiently differentiable in the region considered, with no material discontinuity or [caustic](../../../../../../wave-caustic.md) at the front. Let $t=T(\mathbf x)$ describe arrival time, $\mathbf p=\nabla T$ the slowness vector, and $\mathbf n$ the unit [elastic wave](../../../../../../elastic-wave.md) propagation normal. For any field, its jump is the value immediately behind the front minus that immediately ahead. If the first nonzero jump occurs in the kth time [derivative](../../../../../../derivative.md), $k\geq2$, write

$$
[\partial_t^ku_i]=A_i(\mathbf x),\qquad u_i=A_iF_k(t-T)+B_iF_{k+1}(t-T)+\cdots,\quad F_j(s)=s_+^j/j!.
$$

A smooth background may be added without changing these leading jumps. Since $F_j'=F_{j-1}$, [differentiation](../../../../../../differentiation.md) expresses spatial jumps in terms of $p_j$ and time-derivative jumps. The restriction $k\geq2$ lets [displacement field](../../../../../../displacement-field-mechanics.md) and its first time [derivative](../../../../../../derivative.md) remain continuous and avoids an imposed impulsive source at the front.

Insert this local expansion in $\rho\partial_t^2u_i=\partial_j(c_{ijpq}\partial_pu_q)$. The coefficient of $F_{k-2}$ is

$$
\left(c_{ijpq}p_jp_p-\rho\delta_{iq}\right)A_q=0.
$$

For isotropic [elasticity](../../../../../../elasticity-physics.md) the slowness acoustic [matrix](../../../../../../matrix.md) is $\mu|\mathbf p|^2I+(\lambda+\mu)\mathbf p\mathbf p^T$. Its longitudinal [eigenvalue](../../../../../../eigenvalue.md) is $(\lambda+2\mu)|\mathbf p|^2$. The P branch therefore gives the [eikonal equation](../../../../../../eikonal-equation.md) and polarization

$$
\boxed{|\nabla T|=\alpha^{-1},\qquad\mathbf n=\alpha\nabla T,\qquad A_i=a^{[k]}n_i.}
$$

The next coefficient, $F_{k-1}$, is

$$
\left(c_{ijpq}p_jp_p-\rho\delta_{iq}\right)B_q=c_{ijpq}p_j\partial_pA_q+\partial_j(c_{ijpq}p_pA_q).
$$

The [matrix](../../../../../../matrix.md) on the left is symmetric and annihilates $\mathbf n$. Project onto $n_i$ to obtain its solvability condition. Put $a=a^{[k]}$. The two projected terms can be evaluated without dropping [gradients](../../../../../../gradient.md) of [mass density](../../../../../../density.md) or moduli:

$$
n_ic_{ijpq}p_j\partial_p(an_q)=\rho\alpha\,\mathbf n\cdot\nabla a+\frac{\lambda a}{\alpha}\nabla\cdot\mathbf n,
$$



$$
n_i\partial_j(c_{ijpq}p_pan_q)=\nabla\cdot(\rho\alpha a\mathbf n)-\frac{\lambda a}{\alpha}\nabla\cdot\mathbf n.
$$

These identities use $|\mathbf n|^2=1$, hence $n_q\partial_pn_q=0$, and $(\lambda+2\mu)/\alpha=\rho\alpha$. Their curvature terms cancel, leaving

$$
2\rho\alpha\,\mathbf n\cdot\nabla a+a\nabla\cdot(\rho\alpha\mathbf n)=0.
$$

Multiplying by $a$ proves the requested [P-wavefront discontinuity transport](../../../../../../p-wavefront-discontinuity-transport.md) law,

$$
\boxed{\partial_q\left[\rho\alpha\left(a^{[k]}\right)^2n_q\right]=0.}
$$

The [wave amplitude](../../../../../../wave-amplitude.md) here is real for a real jump; a complex [wave amplitude](../../../../../../wave-amplitude.md) uses the corresponding modulus-squared law. An [elastic ray](../../../../../../elastic-ray.md) follows $d\mathbf x/ds=\mathbf n$, with arclength $s$ and $dt/ds=1/\alpha$. If $J$ is the infinitesimal cross-sectional area of a neighboring ray tube, $d\log J/ds=\nabla\cdot\mathbf n$. Thus $\rho\alpha a^2J$ is constant along that tube, the [ray-tube conservation for a P-wave jump](../../../../../../ray-tube-conservation-for-a-p-wave-jump.md). This defines the geometrical spreading and shows why the [wave amplitude](../../../../../../wave-amplitude.md) changes with material properties even before attenuation is considered. At a [caustic](../../../../../../wave-caustic.md) the simple ray-tube [wave amplitude](../../../../../../wave-amplitude.md) is singular and a uniform local description is needed.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 82](../../../paper-82-split.md)
4. [Iii](../../../split.md)
5. [2005](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
