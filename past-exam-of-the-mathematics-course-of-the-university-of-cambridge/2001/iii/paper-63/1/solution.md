<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

The unbroken group is the [stabilizer subgroup](../../../../../stabilizer-subgroup.md) of the chosen [vacuum expectation value](../../../../../vacuum-expectation-value.md):

$$
\boxed{H=\{h\in G:h\phi_0=\phi_0\}.}
$$

Its [Lie algebra](../../../../../lie-algebra-split.md) consists of generators $T$ with $T\phi_0=0$. The [vacuum manifold](../../../../../vacuum-manifold.md) is the orbit $G\phi_0\simeq G/H$ under the stated transitivity assumption. Its tangent space is the image of $T\mapsto T\phi_0$, so its dimension is $r=\dim G-\dim H$.

Let $K_{ij}=\partial_i\partial_jV(\phi_0)$ be the [scalar mass matrix](../../../../../scalar-mass-matrix.md), with canonical scalar [kinetic terms](../../../../../kinetic-term.md). Invariance of the [scalar potential](../../../../../scalar-potential.md) gives $(\partial_iV)(T_a\phi)_i=0$ for every $\phi$. Differentiate with respect to $\phi_j$ and evaluate at the minimum, where $\partial_iV=0$:

$$
K_{ji}(T_a\phi_0)_i=0.
$$

Thus every independent tangent direction is a zero [eigenvector](../../../../../eigenvector.md) of $K$. These are the [Goldstone directions in the scalar mass matrix](../../../../../goldstone-directions-in-the-scalar-mass-matrix.md); for a global symmetry they are $r$ physical massless [Goldstone bosons](../../../../../goldstone-boson.md). For a generic nondegenerate minimum transverse to the orbit, they are precisely all the zero eigenvalues. Without that nondegeneracy assumption, additional massless scalars are possible.

For a local [gauge group](../../../../../gauge-group.md), use the [orthogonal unitary-gauge slice near a scalar vacuum](../../../../../orthogonal-unitary-gauge-slice-near-a-scalar-vacuum.md). Since $\phi_0^TT_a\phi_0=0$ by antisymmetry, the proposed condition is equivalent to

$$
(\phi-\phi_0)^TT_a\phi_0=0.
$$

It sets the gauge-orbit components of the scalar fluctuation to zero. This is an admissible local [unitary gauge](../../../../../unitary-gauge.md): on a basis of independent broken tangent vectors $v_a=T_a\phi_0$, the variation of these conditions under the broken gauge parameters is $v_a^Tv_b$. This [Gram matrix](../../../../../gram-matrix.md) is invertible on that basis, so the [implicit function theorem](../../../../../implicit-function-theorem.md) selects the required gauge transformation near the vacuum. Unbroken transformations remain as a residual $H$ gauge symmetry; no global gauge slice through zeros of the scalar field is being asserted.

Write $\phi=\phi_0+h$. To quadratic order, the covariant [kinetic term](../../../../../kinetic-term.md) contains

$$
\frac12(\partial_\mu h)^T\partial^\mu h+gA_\mu^a(T_a\phi_0)^T\partial^\mu h+\frac12g^2A_\mu^aA^{b\mu}(T_a\phi_0)^TT_b\phi_0.
$$

The middle term vanishes in this [unitary gauge](../../../../../unitary-gauge.md). The [gauge-boson mass rank from a real scalar vacuum](../../../../../gauge-boson-mass-rank-from-a-real-scalar-vacuum.md) is therefore determined by

$$
\boxed{(M_A^2)_{ab}=g^2(T_a\phi_0)^TT_b\phi_0.}
$$

These are squared masses: the physical [gauge boson](../../../../../gauge-boson.md) masses are square roots of the matrix's nonzero eigenvalues after diagonalization. For real $c_a$,

$$
c_a(M_A^2)_{ab}c_b=g^2\left|\sum_ac_aT_a\phi_0\right|^2\geq0.
$$

Its kernel consists exactly of the unbroken generators. With $g\ne0$, the rank is $r$, so **exactly $\dim G-\dim H$ gauge-field combinations become massive**. Each removed scalar [Goldstone mode](../../../../../goldstone-boson.md) supplies the extra longitudinal polarization of a massive [gauge boson](../../../../../gauge-boson.md).

The remaining physical scalar fluctuations lie in the orthogonal complement of the orbit tangent space. They have no massless modes if $K$ is positive definite on that complement. The unconditional absence of massless scalars does not follow from the printed assumptions. For a concrete counterexample, take a real doublet, $G=SO(2)$ and

$$
V(\phi)=\lambda(\phi_1^2+\phi_2^2-v^2)^4,\qquad \lambda>0,\quad v>0,\quad\phi_0=(v,0).
$$

Its entire minimum set is one circle orbit, as required, but its [Hessian matrix](../../../../../hessian-matrix.md) vanishes at the minimum. Gauging the rotation gives one vector of squared mass $g^2v^2$ and removes the angular scalar. The radial scalar remains massless at quadratic order, since its potential starts at fourth order in the radial fluctuation. This is an [accidental massless radial mode beyond Goldstone modes](../../../../../accidental-massless-radial-modes-beyond-goldstone-modes.md). Thus the intended no-massless-scalar conclusion needs nonzero transverse curvature.

In the [Standard Model](../../../../../standard-model-split.md), the [Higgs doublet](../../../../../higgs-field.md) contains four real components and breaks $SU(2)_L\times U(1)_Y$ to $U(1)_{\rm em}$. Three [Goldstone bosons](../../../../../goldstone-boson.md) become the longitudinal components of $W^\pm$ and $Z$, while the photon remains massless. The remaining radial [Higgs boson](../../../../../higgs-boson.md) is massive for the ordinary quartic potential with positive curvature. With $\langle H\rangle=(0,v_{\rm EW}/\sqrt2)^T$,

$$
m_W=gv_{\rm EW}/2,\qquad m_Z=v_{\rm EW}\sqrt{g^2+g'^2}/2,\qquad m_h^2=2\lambda v_{\rm EW}^2.
$$

The colour gauge group is unbroken. This is the [Higgs mechanism](../../../../../higgs-mechanism.md), with the generic curvature condition realized by the standard Higgs potential.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 63](../../paper-63-split.md)
3. [Iii](../../split.md)
4. [2001](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
