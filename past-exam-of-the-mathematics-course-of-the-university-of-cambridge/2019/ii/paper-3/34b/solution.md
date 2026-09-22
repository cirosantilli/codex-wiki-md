<h1 id="34b/solution">Solution</h1>

↑ **Parent:** [34B](../34b.md)

[Bloch theorem](../../../../../bloch-s-theorem.md) states that the energy eigenstates of a Hamiltonian invariant under translations by a [Bravais lattice](../../../../../bravais-lattice.md) can be chosen as [Bloch states](../../../../../bloch-state.md)

$$
\boxed{
T_r|\psi_k\rangle=e^{-ik\cdot r}|\psi_k\rangle,
\qquad
\psi_k(x)=e^{ik\cdot x}u_k(x),
\qquad
u_k(x+r)=u_k(x).}
$$

Indeed, the [unitary operators](../../../../../unitary-operator.md) $T_r$ commute with one another because $T_rT_s=T_{r+s}=T_sT_r$, and they commute with $H$ by hypothesis. The [simultaneous diagonalization](../../../../../simultaneous-diagonalization.md) theorem therefore lets us diagonalize all translations within each energy eigenspace. Their eigenvalues form a unitary character $\chi$ of the additive lattice:

$$
\chi(r+s)=\chi(r)\chi(s),
\qquad |\chi(r)|=1.
$$

Writing $\chi(a_j)=e^{-ik\cdot a_j}$ on a primitive basis gives $\chi(r)=e^{-ik\cdot r}$. In position space, with $(T_r\psi)(x)=\psi(x-r)$, this implies $\psi_k(x+r)=e^{ik\cdot r}\psi_k(x)$. Hence $u_k(x)=e^{-ik\cdot x}\psi_k(x)$ is lattice-periodic. Adding a [reciprocal lattice](../../../../../reciprocal-lattice.md) vector to $k$ leaves the character unchanged, so the [crystal momentum](../../../../../crystal-momentum.md) lies in a [Brillouin zone](../../../../../brillouin-zone.md).

For

$$
a_1=\frac a2(\sqrt3,1),
\qquad
a_2=\frac a2(\sqrt3,-1),
$$

the equations $a_i\cdot b_j=2\pi\delta_{ij}$ give the reciprocal basis

$$
\boxed{
b_1=\left(\frac{2\pi}{\sqrt3a},\frac{2\pi}{a}\right),
\qquad
b_2=\left(\frac{2\pi}{\sqrt3a},-\frac{2\pi}{a}\right).}
$$

The reciprocal lattice is triangular, so the first Brillouin zone is its [Wigner-Seitz cell](../../../../../wigner-seitz-cell.md), a regular hexagon. Its six corners are

$$
\pm\frac{2b_1+b_2}{3},
\qquad
\pm\frac{b_1+2b_2}{3},
\qquad
\pm\frac{b_1-b_2}{3}.
$$

Reciprocal-lattice translations identify these corners in two classes of three. Representatives are

$$
\boxed{
K=\frac{2b_1+b_2}{3}
=\left(\frac{2\pi}{\sqrt3a},\frac{2\pi}{3a}\right),
\qquad
K'=\frac{b_1+2b_2}{3}
=\left(\frac{2\pi}{\sqrt3a},-\frac{2\pi}{3a}\right).}
$$

For example, $(b_1-b_2)/3=K'-b_2$, while the other equivalences follow by symmetry and reciprocal translations. This gives the requested sketch: a regular hexagon with the vertical edge from $K'$ to $K$ at $k_x=2\pi/(\sqrt3a)$ and alternating $K,K'$ corner classes.

For the [tight-binding model](../../../../../tight-binding.md), introduce the normalized Bloch sum

$$
|k\rangle=\frac1{\sqrt{N_s}}\sum_{r\in\Lambda}e^{ik\cdot r}|r\rangle.
$$

Each hop by $\pm a_j$ multiplies this state by $e^{\mp ik\cdot a_j}$. Thus the [two-direction nearest-neighbour tight-binding dispersion](../../../../../two-direction-nearest-neighbour-tight-binding-dispersion.md) is

$$
\boxed{
\begin{aligned}
E(k)
&=E_0-2\lambda\{\cos(k\cdot a_1)+\cos(k\cdot a_2)\}\\
&=E_0-4\lambda
\cos\left(\frac{\sqrt3ak_x}{2}\right)
\cos\left(\frac{ak_y}{2}\right).
\end{aligned}}
$$

Along the boundary edge from $K'$ to $K$, $k_x=2\pi/(\sqrt3a)$ and $|k_y|\leq2\pi/(3a)$, so

$$
E(k)=E_0+4\lambda\cos\left(\frac{ak_y}{2}\right).
$$

For $\lambda>0$, it rises from $E_0+2\lambda$ at either corner to $E_0+4\lambda$ at the midpoint; for $\lambda<0$ the ordering reverses. Globally the two cosines in the first expression can simultaneously equal $1$ or $-1$, and therefore

$$
\boxed{
E_{\min}=E_0-4|\lambda|,
\qquad
E_{\max}=E_0+4|\lambda|,
\qquad
\text{band width}=8|\lambda|.}
$$

Each orbital band contains two one-electron states per lattice site because an electron has two spin states. By [band filling](../../../../../band-filling.md), a valency of one leaves this band half-filled and the material conducts, whereas a valency of two fills it. A filled band can be insulating only if it is separated from every empty band by a positive [band gap](../../../../../band-gap.md).

The first band's maximum is $E_0+4|\lambda|$. If the second band's minimum is $E_0+\Delta$, a gap exists precisely when $\Delta>4|\lambda|$. Consequently, among the nontrivial fillings described here,

$$
\boxed{\text{the material is a band insulator when the valency is }2
\text{ and }\Delta>4|\lambda|.}
$$

For valency one the first band is partially filled. If $\Delta\leq4|\lambda|$, the bands overlap or touch, so even at valency two the [overlapping energy bands prevent a band insulator](../../../../../overlapping-energy-bands-prevent-a-band-insulator.md).

## ↑ Ancestors (10)

1. [34B](../34b.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ii](../../split.md)
4. [2019](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
