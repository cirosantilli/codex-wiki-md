<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Set $\hbar=1$. Work on the strip $0\leq\sigma\leq\pi$ in [conformal gauge](../../../../../conformal-gauge.md), with worldsheet signature $(-,+)$ and target signature $(-,+,\ldots,+)$. In [light-cone gauge in string theory](../../../../../light-cone-gauge-in-string-theory.md), the independent fields are the $d=D-2=24$ transverse coordinates. Put the [Neumann boundary condition](../../../../../neumann-boundary-condition.md) at $\sigma=0$ and the [Dirichlet boundary condition](../../../../../dirichlet-boundary-condition.md) at $\sigma=\pi$; reversing the endpoints exchanges cosine and sine modes without changing the spectrum. The fixed endpoint is $X^i(\tau,\pi)=y^i$.

Varying the transverse [Polyakov action](../../../../../polyakov-action.md) gives $(\partial_\tau^2-\partial_\sigma^2)X^i=0$ and the spatial boundary contribution $-(2\pi\alpha')^{-1}\int d\tau\,[X'^i\delta X^i]_0^\pi$. At the free endpoint this vanishes precisely when $X'^i=0$; at the fixed endpoint $\delta X^i=0$. [Separation of variables](../../../../../separation-of-variables.md) then gives $\cos(r\sigma)$ with $\cos(r\pi)=0$, hence $r=n+\tfrac12$, $n=0,1,\ldots$. These are [Neumann-Dirichlet open-string boundary conditions](../../../../../neumann-dirichlet-open-string-boundary-condition.md). No dynamical transverse [worldsheet zero mode](../../../../../worldsheet-zero-mode.md) survives: a constant solution must equal the prescribed $y^i$, and a linear-in-$\sigma$ solution violates the free-end condition.

Write $X^i-y^i=\sum_{r>0}q_r^i(\tau)\cos(r\sigma)$. The [orthogonality](../../../../../orthogonal-vectors.md) relation $\int_0^\pi\cos(r\sigma)\cos(s\sigma)d\sigma=(\pi/2)\delta_{rs}$ reduces the action to independent [harmonic oscillators](../../../../../simple-harmonic-motion.md):

$$
S_\perp=\frac1{8\alpha'}\int d\tau\sum_{i=1}^{24}\sum_{r>0}\bigl((\dot q_r^i)^2-r^2(q_r^i)^2\bigr),\qquad P_r^i=\frac{\dot q_r^i}{4\alpha'}.
$$

The [canonical commutation relations](../../../../../canonical-commutation-relation.md) $[q_r^i,P_s^j]=i\delta^{ij}\delta_{rs}$ determine normalized [annihilation operators](../../../../../annihilation-operator.md) at $\tau=0$

$$
a_r^i=\sqrt{\frac r{8\alpha'}}q_r^i+i\sqrt{\frac{2\alpha'}r}P_r^i,\qquad
\boxed{[a_r^i,a_s^{j\dagger}]=\delta^{ij}\delta_{rs},\quad[a_r^i,a_s^j]=[a_r^{i\dagger},a_s^{j\dagger}]=0.}
$$

Thus $q_r^i=\sqrt{2\alpha'/r}\,(a_r^ie^{-ir\tau}+a_r^{i\dagger}e^{ir\tau})$. These formulas derive the quantization from the action rather than import integer-moded open-string rules.

For the usual phased [string oscillators](../../../../../string-oscillator.md), set $\alpha_r^i=-i\sqrt r\,a_r^i$ and $\alpha_{-r}^i=i\sqrt r\,a_r^{i\dagger}$ for $r>0$. Then the [half-integer open-string oscillator](../../../../../half-integer-open-string-oscillator.md) expansion and algebra are

$$
X^i=y^i+i\sqrt{2\alpha'}\sum_{r\in\mathbb Z+1/2}\frac{\alpha_r^i}{r}e^{-ir\tau}\cos(r\sigma),\qquad
\boxed{[\alpha_r^i,\alpha_s^j]=r\delta^{ij}\delta_{r+s,0},\quad\alpha_r^{i\dagger}=\alpha_{-r}^i.}
$$

The corresponding field [momentum](../../../../../momentum.md) density is $\Pi_i=\dot X^i/(2\pi\alpha')$. Completeness of the mixed-boundary [eigenfunctions](../../../../../eigenfunction.md) gives $[X^i(\sigma),\Pi_j(\sigma')]=i\delta^i_j\delta_{\mathrm{ND}}(\sigma,\sigma')$, where $\delta_{\mathrm{ND}}=(2/\pi)\sum_{r>0}\cos(r\sigma)\cos(r\sigma')$. This is a [distribution](../../../../../distribution-mathematical-analysis.md) identity on the mixed-boundary function space, not an unrestricted value at a fixed endpoint with a [Dirichlet boundary condition](../../../../../dirichlet-boundary-condition.md).

Classically, the transverse [Virasoro algebra](../../../../../virasoro-algebra.md) zero-mode generator is

$$
\boxed{L_{0,\mathrm{cl}}^\perp=\frac12\sum_{i=1}^{24}\sum_{r\in\mathbb Z+1/2}\alpha_{-r}^i\alpha_r^i=\sum_{i=1}^{24}\sum_{r>0}\alpha_{-r}^i\alpha_r^i.}
$$

There is no transverse [momentum](../../../../../momentum.md) term. If the two light-cone directions are common directions with [Neumann boundary conditions](../../../../../neumann-boundary-condition.md), the full zero-mode constraint adds $\alpha'p_\parallel^2=-2\alpha'p^+p^-$: $L_{0,\mathrm{cl}}=\alpha'p_\parallel^2+L_{0,\mathrm{cl}}^\perp$. This assumption about the longitudinal directions is needed to interpret oscillator levels as target-space masses.

Quantizing the symmetrically ordered transverse generator gives $L_0^\perp=N+E_0$, where the [string level operator](../../../../../string-level-operator.md) is $N=\sum_{i,r>0}r a_r^{i\dagger}a_r^i$. Each [harmonic oscillator](../../../../../simple-harmonic-motion.md) contributes $r/2$ to the [vacuum energy](../../../../../vacuum-energy.md). Use [zeta function regularization](../../../../../zeta-function-regularization.md) and the [Riemann zeta function](../../../../../riemann-zeta-function.md) with the actual half-integer spectrum:

$$
\sum_{n\geq0}(n+\tfrac12)^{-s}=(2^s-1)\zeta_R(s),\qquad
\sum_{r>0}^{\mathrm{reg}}r=(2^{-1}-1)\zeta_R(-1)=\frac1{24}.
$$

Consequently the [Neumann-Dirichlet string zero-point energy](../../../../../neumann-dirichlet-string-zero-point-energy.md) is

$$
\boxed{E_0=\frac{24}{2}\frac1{24}=\frac12,\qquad L_0=\alpha'p_\parallel^2+N+\frac12.}
$$

In the common convention $L_0=\alpha'p_\parallel^2+N-a$, the [normal-ordering constant of a string](../../../../../normal-ordering-constant-of-a-string.md) is $a=-\tfrac12$. This positive shift differs from the $-1$ [vacuum energy](../../../../../vacuum-energy.md) of 24 integer-moded transverse [bosons](../../../../../boson.md). The difference between those two vacuum energies is $3/2$. To distinguish zero-mode conventions, the [ND twist conformal weight](../../../../../bosonic-nd-boundary-changing-conformal-weight.md) is $1/16$ per transverse boson. With 24 bosons, the plane matter generator is $L_0^{\mathrm{plane}}=\alpha'p_\parallel^2+N+3/2$; its physical open-string condition $L_0^{\mathrm{plane}}-1=0$ is exactly the strip/light-cone constraint $\alpha'p_\parallel^2+N+1/2=0$ used here. The transverse plane and strip constants differ by the [central charge](../../../../../central-charge.md) shift $c_\perp/24=24/24=1$. A common exponential frequency cutoff independently gives $\sum_{r>0}r e^{-\varepsilon r}=\varepsilon^{-2}+1/24+O(\varepsilon^2)$, confirming the finite part and avoiding invalid termwise manipulation of divergent sums.

Let $a_r^i|0\rangle=0$. The [lowest levels of a fully transverse ND bosonic string](../../../../../lowest-levels-of-a-fully-transverse-nd-bosonic-string.md) are

$$
\begin{array}{c|c|c|c}
N&\text{states}&L_0^\perp&\text{multiplicity}\\\hline
0&|0\rangle&1/2&1\\
1/2&a_{1/2}^{i\dagger}|0\rangle&1&24\\
1&a_{1/2}^{i\dagger}a_{1/2}^{j\dagger}|0\rangle&3/2&300
\end{array}
$$

The third level has two $r=1/2$ excitations; there is no $r=1$ oscillator. Its indices are symmetric because the [creation operators](../../../../../creation-operator.md) commute. With $L_0=0$ and the common longitudinal [momentum](../../../../../momentum.md) convention, the rest energies and masses obey

$$
\boxed{\alpha'M^2=\frac12,\ 1,\ \frac32\quad\text{at the first three levels}.}
$$

At fixed positive $p^+$ the corresponding light-cone energies are $p^-=(N+1/2)/(2\alpha'p^+)$; the table lists excitation levels, not a spectrum that remains discrete if longitudinal [momentum](../../../../../momentum.md) is varied continuously.

The surviving transverse rotations form $SO(24)$. The ground state is a [scalar](../../../../../scalar.md), the next level its [vector](../../../../../vector.md), and the third level the [symmetric square](../../../../../symmetric-square.md) of the vector. Separating its trace gives

$$
\boxed{\mathbf1,\qquad\mathbf{24},\qquad\operatorname{Sym}^2(\mathbf{24})=\mathbf{299}\oplus\mathbf1.}
$$

The trace state is proportional to $\sum_i(a_{1/2}^{i\dagger})^2|0\rangle$; subtracting this trace gives the 299-dimensional [symmetric traceless square](../../../../../symmetric-trace-free-square-of-the-defining-orthogonal-representation.md).

There is a qualification to the printed “little group”. The [little group with mixed string boundary conditions](../../../../../little-group-with-mixed-string-boundary-conditions.md) must preserve the endpoints as well as [momentum](../../../../../momentum.md). These [boundary conditions](../../../../../boundary-condition.md) break the full 26-dimensional [Lorentz group](../../../../../lorentz-group.md), so the massive states above cannot be classified as representations of the unbroken 26-dimensional massive [little group](../../../../../little-group.md) $SO(25)$. In a D1–D25 realization the common worldvolume has Lorentz group $SO(1,1)$ and trivial connected massive little group; $SO(24)$ acts on the ND coordinates as an internal rotation group. **The scalar, vector and symmetric trace-free decomposition is under the surviving transverse SO(24), with this boundary-background qualification.**

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 306](../../paper-306-split.md)
3. [Iii](../../split.md)
4. [2017](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
