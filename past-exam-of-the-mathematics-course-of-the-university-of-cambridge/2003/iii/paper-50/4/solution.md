<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

Write the integrand, without its common overall factor, as $\mathcal L=\partial_+X\cdot\partial_-X-\psi_1\cdot\partial_-\psi_1-\psi_2\cdot\partial_+\psi_2$. Keep each constant [Grassmann variable](../../../../../grassmann-variable.md) on the left. For the first [supersymmetry](../../../../../supersymmetry-split.md) component, varying the bosonic term gives

$$
\varepsilon_1\left(\partial_+\psi_1\cdot\partial_-X+\partial_+X\cdot\partial_-\psi_1\right).
$$

Varying its [fermion](../../../../../fermion.md) term gives $-\varepsilon_1\partial_+X\cdot\partial_-\psi_1+\varepsilon_1\psi_1\cdot\partial_-\partial_+X$. The plus sign in the second term comes from moving the odd parameter past $\psi_1$. The middle terms cancel and the rest form $\varepsilon_1\partial_+(\psi_1\cdot\partial_-X)$. The second [supersymmetry](../../../../../supersymmetry-split.md) component similarly gives $\varepsilon_2\partial_-(\psi_2\cdot\partial_+X)$. Hence, off shell,

$$
\boxed{\delta\mathcal L=\varepsilon_1\partial_+(\psi_1\cdot\partial_-X)+\varepsilon_2\partial_-(\psi_2\cdot\partial_+X).}
$$

This proves the local total-derivative identity for rigid [worldsheet supersymmetry](../../../../../worldsheet-supersymmetry.md); the [action](../../../../../action.md) is invariant when the corresponding boundary flux vanishes and the transformation preserves the allowed fields. A constant parameter preserves a periodic [boson](../../../../../boson.md) and a periodic [fermion](../../../../../fermion.md). In a [Neveu–Schwarz sector](../../../../../neveu-schwarz-sector.md), however, $\delta X=\varepsilon\psi$ is antiperiodic for constant $\varepsilon$ and does not preserve the periodic [boson](../../../../../boson.md). Thus the bulk identity does not supply a global constant supercharge in every spin sector. This is the [spin-structure obstruction to constant worldsheet supersymmetry](../../../../../spin-structure-obstruction-to-constant-worldsheet-supersymmetry.md); the local superconformal formulation handles the different sectors consistently.

For independent field variations, [integration by parts](../../../../../integration-by-parts.md) gives bulk terms

$$
\delta\mathcal L\big|_{\rm bulk}=-2\delta X\cdot\partial_+\partial_-X-2\delta\psi_1\cdot\partial_-\psi_1-2\delta\psi_2\cdot\partial_+\psi_2.
$$

The [equations of motion](../../../../../equation-of-motion.md) are therefore

$$
\boxed{\partial_+\partial_-X=0,\qquad\partial_-\psi_1=0,\qquad\partial_+\psi_2=0.}
$$

For variations vanishing at the temporal ends, the spatial seam term is proportional to the difference between its values at $\sigma=2\pi$ and $\sigma=0$ of

$$
-2\partial_\sigma X\cdot\delta X+\psi_1\cdot\delta\psi_1-\psi_2\cdot\delta\psi_2.
$$

The bosonic part cancels for [closed string](../../../../../closed-string.md) periodicity, also in a fixed winding sector. For a real [fermion](../../../../../fermion.md) impose $\psi_a(2\pi)=s_a\psi_a(0)$ and the same relation on its variation. Seam cancellation requires $s_a^2=1$, so the two untwisted possibilities are **periodic, $s_a=+1$ ([Ramond sector](../../../../../ramond-sector.md)), or antiperiodic, $s_a=-1$ ([Neveu–Schwarz sector](../../../../../neveu-schwarz-sector.md))**. The two chiralities of a [closed string](../../../../../closed-string.md) can choose these signs independently, giving R–R, NS–NS, R–NS and NS–R sectors. This discussion assumes the ordinary Lorentz-invariant untwisted [boundary conditions](../../../../../boundary-condition.md) of the flat theory.

The chiral equations and boundary signs give the following [Fourier series](../../../../../fourier-series-split.md)

$$
\psi_1^\mu(\tau,\sigma)=\sum_{r\in\mathbb Z+\nu_1}\psi_{1r}^\mu e^{-ir(\tau+\sigma)},\qquad\psi_2^\mu(\tau,\sigma)=\sum_{r\in\mathbb Z+\nu_2}\psi_{2r}^\mu e^{-ir(\tau-\sigma)},
$$

where $\nu_a=0$ in R and $\nu_a=1/2$ in NS. Thus integer or half-integer modes follow directly from the [Fourier series](../../../../../fourier-series-split.md) monodromy. With the conventional [string oscillator](../../../../../string-oscillator.md) normalization their anticommutation relations and reality conditions are

$$
\{\psi_{ar}^\mu,\psi_{bs}^\nu\}=\delta_{ab}\eta^{\mu\nu}\delta_{r+s,0},\qquad (\psi_{ar}^\mu)^\dagger=\psi_{a,-r}^\mu.
$$

For an [open string](../../../../../open-string.md) the endpoint gluing identifies the two sets of coefficients, leaving one R or NS tower.

In ten-dimensional [light-cone gauge in string theory](../../../../../light-cone-gauge-in-string-theory.md), the eight transverse bosonic modes have positive integer level and each NS fermionic creator has a positive half-integer level. For the [unprojected low levels of the open RNS string](../../../../../unprojected-low-levels-of-the-open-rns-string.md), all states through $\alpha'M^2=1$ in the [NS sector](../../../../../neveu-schwarz-sector.md) are

$$
\begin{array}{c|c|c|c}
N&\alpha'M^2&\text{oscillator states on }|0;p\rangle&\text{number}\\
0&-1/2&|0;p\rangle&1\\
1/2&0&\psi_{-1/2}^i|0;p\rangle&8\\
1&1/2&\alpha_{-1}^i|0;p\rangle,\quad\psi_{-1/2}^i\psi_{-1/2}^j|0;p\rangle\ (i<j)&8+28=36\\
3/2&1&\psi_{-3/2}^i|0;p\rangle,\quad\alpha_{-1}^i\psi_{-1/2}^j|0;p\rangle,\quad\psi_{-1/2}^i\psi_{-1/2}^j\psi_{-1/2}^k|0;p\rangle\ (i<j<k)&8+64+56=128
\end{array}
$$

The antisymmetric index restrictions are consequences of fermionic anticommutation; the [boson](../../../../../boson.md)–[fermion](../../../../../fermion.md) pair has all 64 choices. The displayed partitions exhaust levels at most $3/2$. Here the NS [normal-ordering constant of a string](../../../../../normal-ordering-constant-of-a-string.md) is $a=1/2$.

In the [R sector](../../../../../ramond-sector.md) $a=0$, and the zero modes satisfy $\{\psi_0^i,\psi_0^j\}=\delta^{ij}$. Thus $\gamma^i=\sqrt2\psi_0^i$ generate the [Ramond zero-mode Clifford algebra](../../../../../ramond-zero-mode-clifford-algebra.md). The unprojected ground states $|S;p\rangle$ span a sixteen-dimensional transverse [spinor](../../../../../spinor.md) space, $8_s\oplus8_c$. All states in the requested range are

$$
\begin{array}{c|c|c|c}
N&\alpha'M^2&\text{states}&\text{number}\\
0&0&|S;p\rangle&16\\
1&1&\alpha_{-1}^i|S;p\rangle,\quad\psi_{-1}^i|S;p\rangle&128+128=256.
\end{array}
$$

There is no intervening half-level, since all nonzero R modes have integer level. Acting with the zero modes only moves within the ground [spinor](../../../../../spinor.md) space and does not generate further independent copies.

The [GSO projection](../../../../../gso-projection.md) keeps odd NS fermion-excitation parity, removing the tachyonic vacuum and the entire $N=1$ NS level. In R it keeps one [eigenvalue](../../../../../eigenvalue.md) of total [fermion](../../../../../fermion.md) parity, whose zero-mode part is [spinor](../../../../../spinor.md) [chirality](../../../../../chirality-physics.md). It leaves eight massless [spinor](../../../../../spinor.md) states. At R level one, the retained families are $\alpha_{-1}^i|S_+\rangle$ and $\psi_{-1}^i|S_-\rangle$, of opposite ground [chirality](../../../../../chirality-physics.md), so there are $64+64=128$ states. The retained NS states are [spacetime](../../../../../spacetime.md) [bosons](../../../../../boson.md) and the R states [spacetime](../../../../../spacetime.md) [fermions](../../../../../fermion.md). Consequently **the retained levels have $8_B=8_F$ at mass zero and $128_B=128_F$ at $\alpha'M^2=1$, with no [tachyon](../../../../../tachyon.md)**.

Equality at every higher mass level follows from the standard [Jacobi abstruse identity](../../../../../jacobi-abstruse-identity.md), or equivalently the equality of the transverse [generating functions](../../../../../generating-function.md)

$$
\frac{\prod_{n\geq1}(1+q^{n-1/2})^8-\prod_{n\geq1}(1-q^{n-1/2})^8}{2q^{1/2}\prod_{n\geq1}(1-q^n)^8}=8\frac{\prod_{n\geq1}(1+q^n)^8}{\prod_{n\geq1}(1-q^n)^8}.
$$

The left side counts the projected NS [bosons](../../../../../boson.md), the right side the projected R [fermions](../../../../../fermion.md). Their common coefficients start $8+128q+\cdots$. This consistent truncation yields [spacetime](../../../../../spacetime.md) [supersymmetry](../../../../../supersymmetry-split.md); the bulk [worldsheet](../../../../../worldsheet.md) symmetry alone would not remove the [tachyon](../../../../../tachyon.md) or impose the projection.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 50](../../paper-50-split.md)
3. [Iii](../../split.md)
4. [2003](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
