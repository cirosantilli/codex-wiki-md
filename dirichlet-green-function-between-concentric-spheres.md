# Dirichlet Green function between concentric spheres

↑ **Parent:** [Dirichlet Green function](dirichlet-green-function.md)

For the gap $a<r<b$, put $u_\ell(r)=r^\ell-a^{2\ell+1}r^{-\ell-1}$, $v_\ell(r)=r^{-\ell-1}-r^\ell/b^{2\ell+1}$ and $d_\ell=(2\ell+1)[1-(a/b)^{2\ell+1}]$. With orthonormal [spherical harmonics](spherical-harmonic.md), the [Dirichlet Green function](dirichlet-green-function.md) is

$$
G(\mathbf r,\mathbf r')=4\pi\sum_{\ell=0}^{\infty}\sum_{m=-\ell}^{\ell}
\overline{Y_{\ell m}(\Omega)}Y_{\ell m}(\Omega')\frac{u_\ell(r_<)v_\ell(r_>)}{d_\ell}.
$$

For a short verification, $u_\ell(a)=v_\ell(b)=0$ and both solve the radial [Laplace equation](laplace-equation.md). Their [Wronskian](wronskian.md) is $u_\ell v_\ell'-u_\ell'v_\ell=-d_\ell/r^2$. Thus the radial [derivative](derivative.md) jump is $-1/r'^2$; completeness of the [spherical harmonics](spherical-harmonic.md) gives the stated [Dirac delta function](dirac-delta-function.md) normalization. A [point charge](point-charge.md) has [electric potential](electric-potential.md) $qG/(4\pi\epsilon_0)$, and the inner-wall [surface charge density](surface-charge-density.md) is $-q\partial_rG|_{a^+}/(4\pi)$, with the angular source coordinates held fixed.

## ↑ Ancestors (6)

1. [Dirichlet Green function](dirichlet-green-function.md)
2. [Green's function](green-s-function-split.md)
3. [Analysis](analysis-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-electromagnetism-course-of-the-university-of-oxford/2023/1/c/i/solution.md)
