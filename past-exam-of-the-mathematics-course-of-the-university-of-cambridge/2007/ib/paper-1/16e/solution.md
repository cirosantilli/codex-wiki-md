<h1 id="16e/solution">Solution</h1>

↑ **Parent:** [16E](../16e.md)

A steady localized [electric current density](../../../../../current-density.md) satisfies $\nabla\cdot\mathbf j=0$, from charge conservation or the divergence of Ampère's equation. Choose an enclosing region whose boundary lies outside its support; extending the integration region does not change the source integrals. The [divergence theorem](../../../../../divergence-theorem.md) applied componentwise gives

$$
\nabla\cdot(x_i\mathbf j)=j_i,\qquad
\nabla\cdot(x_ix_k\mathbf j)=x_kj_i+x_ij_k.
$$

Their boundary fluxes vanish, proving the [localized steady-current moment identities](../../../../../localized-steady-current-moment-identities.md)

$$
\boxed{\int_V\mathbf j\,dV=0,\qquad
\int_Vx_ij_k\,dV=-\int_Vx_kj_i\,dV.}
$$

For discontinuous but localized currents the same argument uses the distributional steady conservation law and an outer enclosing surface.

The [magnetic vector potential](../../../../../magnetic-vector-potential.md) is a [vector field](../../../../../vector-field.md) with $\mathbf B=\nabla\times\mathbf A$, consistent with $\nabla\cdot\mathbf B=0$. It is defined up to $\mathbf A\mapsto\mathbf A+\nabla\chi$. The steady Maxwell equation $\nabla\times\mathbf B=\mu_0\mathbf j$ gives

$$
\nabla(\nabla\cdot\mathbf A)-\nabla^2\mathbf A=\mu_0\mathbf j.
$$

In the [Coulomb gauge](../../../../../coulomb-gauge.md) $\nabla\cdot\mathbf A=0$, the equation is $\nabla^2\mathbf A=-\mu_0\mathbf j$, whose decaying Green-function solution is the one supplied in the source.

Let $r=|\mathbf x|$ and expand its kernel uniformly over the bounded source region:

$$
\frac1{|\mathbf x-\mathbf x'|}=\frac1r+\frac{\mathbf x\cdot\mathbf x'}{r^3}+O(r^{-3}).
$$

The first term integrates to zero. Put $T_{ki}=\int x'_kj_i(\mathbf x')\,dV'$, an antisymmetric tensor by the earlier identity. Define the [magnetic dipole moment](../../../../../magnetic-dipole-moment.md) $m_\ell=\frac12\epsilon_{\ell ki}T_{ki}$, so $T_{ki}=\epsilon_{ki\ell}m_\ell$. Consequently

$$
A_i=\frac{\mu_0}{4\pi r^3}x_kT_{ki}+O(r^{-3})
=\frac{\mu_0}{4\pi r^3}(\mathbf m\times\mathbf x)_i+O(r^{-3}),
$$

or

$$
\boxed{\mathbf A(\mathbf x)=\frac{\mu_0}{4\pi}\frac{\mathbf m\times\mathbf x}{r^3}+O(r^{-3}),\qquad
\mathbf m=\frac12\int_V\mathbf x'\times\mathbf j(\mathbf x')\,dV'.}
$$

The displayed dipole term has size $r^{-2}$. If $\mathbf m=0$, it vanishes and a higher multipole determines the leading [magnetic field](../../../../../magnetic-field.md) instead.

For $r>0$, $\nabla\cdot(\mathbf x/r^3)=0$ and

$$
\nabla\times(\mathbf m\times\mathbf x/r^3)
=-(\mathbf m\cdot\nabla)(\mathbf x/r^3)
=\frac{3\mathbf x(\mathbf m\cdot\mathbf x)}{r^5}-\frac{\mathbf m}{r^3}.
$$

Therefore **the far [magnetic field](../../../../../magnetic-field.md) is**

$$
\boxed{\mathbf B(\mathbf x)=\frac{\mu_0}{4\pi r^3}
\left[3(\mathbf m\cdot\widehat{\mathbf x})\widehat{\mathbf x}-\mathbf m\right]+O(r^{-4}).}
$$

## ↑ Ancestors (10)

1. [16E](../16e.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ib](../../split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
