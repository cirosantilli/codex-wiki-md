<h1 id="35d/solution">Solution</h1>

↑ **Parent:** [35D](../35d.md)

Use signature $(+,-,-,-)$, which is required for the stated tensor convention. Then $U_b=\gamma(1,-\mathbf v)$. The time component is $F^{0b}U_b=\gamma\mathbf E\cdot\mathbf v$, while $F^{ij}=-\epsilon_{ijk}B_k$ gives the spatial components $\gamma(\mathbf E+\mathbf v\times\mathbf B)$. Thus

$$
\boxed{F^{ab}U_b=\gamma(\mathbf E\cdot\mathbf v,\mathbf E+\mathbf v\times\mathbf B).}
$$

The scalar $\rho_*=J^bU_b$ is the charge density in the medium's rest frame. In that frame $U=(1,0)$, so $J-\rho_*U=(0,\mathbf j)$ and $F U=(0,\mathbf E)$. The rest-frame [Ohm's law](../../../../../ohm-s-law.md) is precisely their proportionality with rest conductivity $\sigma$. Both sides are [four-vectors](../../../../../four-vector.md), so its covariant form is

$$
\boxed{J^a-(J^bU_b)U^a=\sigma F^{ab}U_b.}
$$

The time and spatial components respectively give

$$
\rho-\gamma\rho_*=\sigma\gamma\mathbf E\cdot\mathbf v,\qquad
\mathbf j-\gamma\rho_*\mathbf v=\sigma\gamma(\mathbf E+\mathbf v\times\mathbf B).
$$

Eliminate $\rho_*$ to obtain

$$
\boxed{\mathbf j=\rho\mathbf v+\sigma\gamma[\mathbf E+\mathbf v\times\mathbf B-(\mathbf E\cdot\mathbf v)\mathbf v].}
$$

If the rest-frame charge density vanishes, set $\rho_*=0$, not necessarily $\rho=0$ in the lab frame. Then

$$
\boxed{\rho=\sigma\gamma\mathbf E\cdot\mathbf v,\qquad
\mathbf j=\sigma\gamma(\mathbf E+\mathbf v\times\mathbf B).}
$$

The induced lab charge is the term that cancels the longitudinal correction in the general formula.

## ↑ Ancestors (10)

1. [35D](../35d.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ii](../../split.md)
4. [2008](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
