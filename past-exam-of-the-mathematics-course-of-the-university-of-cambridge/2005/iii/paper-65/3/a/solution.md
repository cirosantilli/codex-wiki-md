<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Take the leading real field to be $A e^{i(k_cx+\omega_0t)}+B e^{i(-k_cx+\omega_0t)}+\text{complex conjugate}$. A [spatial translation](../../../../../../spatial-translation.md) gives $(A,B)\mapsto(e^{ik_c\delta}A,e^{-ik_c\delta}B)$; a time translation gives $(A,B)\mapsto(e^{i\psi}A,e^{i\psi}B)$; spatial reflection exchanges $A$ and $B$.

For a monomial $A^j\overline A^kB^l\overline B^m$ in the first [amplitude equation](../../../../../../amplitude-equation.md), covariance requires $j-k+l-m=1$ and $j-k-l+m=1$. Hence $j-k=1$, $l-m=0$. At linear order only $A$ is allowed, no quadratic monomial satisfies these conditions, and the cubic possibilities are $A^2\overline A$ and $AB\overline B$. Reflection fixes the coefficients in the second equation. Removing the small common linear frequency correction by a rotating frame makes $\mu$ real. This derives the two cubic [amplitude equations](../../../../../../amplitude-equation.md), rather than merely postulating them.

Let $r=|A|^2$, $s=|B|^2$. Taking real parts gives

$$
\dot r=2r(\mu-\beta_r r-\gamma_r s),\qquad
\dot s=2s(\mu-\beta_r s-\gamma_r r).
$$

A [travelling wave](../../../../../../travelling-wave.md) has $(r,s)=(\mu/\beta_r,0)$, or its reflection, whenever $\mu/\beta_r>0$. Its phase evolves at $-\beta_i\mu/\beta_r$, shifting the physical oscillation frequency. The nonzero-amplitude radial [eigenvalue](../../../../../../eigenvalue.md) is $-2\mu$, while the absent mode has real growth rate $\mu(1-\gamma_r/\beta_r)$. Therefore, on the supercritical side,

$$
\boxed{\text{stable travelling wave: }\mu>0,\quad\beta_r>0,\quad\gamma_r>\beta_r.}
$$

The phase direction is neutral because of the symmetry, so stability means [orbital stability](../../../../../../orbital-stability.md). A branch with $\mu<0$ is radially unstable, whatever the transverse coefficient.

A [standing wave](../../../../../../standing-wave.md) has $r=s=h=\mu/(\beta_r+\gamma_r)>0$. Its two phases evolve together at $-(\beta_i+\gamma_i)h$; the relative phase fixes the spatial position of the standing pattern. In the two intensity directions the [eigenvalues](../../../../../../eigenvalue.md) are $-2\mu$ and $-2h(\beta_r-\gamma_r)$. Thus

$$
\boxed{\text{stable standing wave: }\mu>0,\quad\beta_r+\gamma_r>0,\quad\beta_r>\gamma_r.}
$$

Again the symmetry phases are neutral and the conclusion is [orbital stability](../../../../../../orbital-stability.md). Equality $\beta_r=\gamma_r$ leaves a continuum of mixed intensities at cubic order; equality $\beta_r+\gamma_r=0$ removes cubic standing-wave saturation. These degeneracies require higher-order terms and cannot be classified by the cubic truncation. The zero state is linearly stable for $\mu<0$ and unstable for $\mu>0$.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3](../../3.md)
3. [Paper 65](../../../paper-65-split.md)
4. [Iii](../../../split.md)
5. [2005](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
