<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

**Solving the massive subsidiary conditions.** In [light-cone coordinates](../../../../../light-cone-coordinates.md), use $ds^2=-2dX^+dX^-+\delta_{IJ}dX^IdX^J$ and write $d=D-2$. The divergence condition reads

$$
-\partial_-h_{+n}-\partial_+h_{-n}+\partial_Ih_{In}=0.
$$

Thus, when $\partial_-$ is invertible,

$$
h_{+n}=\partial_-^{-1}\!\left(-\partial_+h_{-n}+\partial_Ih_{In}\right).
$$

First apply this with $n=-$, then with $n=I$, and finally with $n=+$; symmetry supplies the mixed components already determined. The [trace](../../../../../matrix-trace.md) condition becomes

$$
\delta^{IJ}h_{IJ}=2h_{+-}
=2\partial_-^{-1}\!\left(-\partial_+h_{--}+\partial_Ih_{I-}\right).
$$

The independent components are $h_{--}$, $h_{-I}$ and the [trace](../../../../../matrix-trace.md)-free part of $h_{IJ}$. Under transverse rotations they form a [scalar representation](../../../../../scalar-representation.md), a [vector representation](../../../../../vector-representation.md), and a [symmetric traceless rank-two tensor](../../../../../symmetric-trace-free-square-of-the-defining-orthogonal-representation.md). Therefore

$$
\boxed{1+d+\left[\frac{d(d+1)}2-1\right]
=\frac{d(d+3)}2=\frac{(D-2)(D+1)}2.}
$$

This is the [light-cone decomposition of a massive spin-two field](../../../../../light-cone-decomposition-of-a-massive-spin-two-field.md) for $D\geq3$. In $D=2$, the [trace](../../../../../matrix-trace.md) and divergence give $h_{+-}=h_{++}=0$ and $\partial_+h_{--}=0$. The massive wave equation then forces $h_{--}=0$, so there are no polarizations, consistent with the zero value of the printed count. The [massive particle little group](../../../../../massive-particle-little-group.md) is $SO(D-1)=SO(d+1)$, and its [symmetric traceless square](../../../../../symmetric-trace-free-square-of-the-defining-orthogonal-representation.md) branches as

$$
\operatorname{Sym}_0^2(\mathbb R^{d+1})\downarrow SO(d)
=\operatorname{Sym}_0^2(\mathbb R^d)\oplus\mathbb R^d\oplus\mathbb R.
$$

The mixed components with the extra direction give the vector; one independent [trace](../../../../../matrix-trace.md) combination gives the scalar. These are exactly the polarizations of a [massive spin-two field](../../../../../massive-spin-two-field.md). The remaining independent components retain the massive [Klein-Gordon equation](../../../../../klein-gordon-equation.md).

**Transverse bosonic modes and mass levels.** The variables $\alpha_k^I$ are Fourier amplitudes of the physical transverse [open-string mode expansion](../../../../../open-string-mode-expansion.md). Classically, reality requires $\alpha_{-k}^I=(\alpha_k^I)^*$. The symplectic term in the action fixes their quantum [commutators](../../../../../commutator.md):

$$
[\alpha_k^I,\alpha_l^J]=k\,\delta^{IJ}\delta_{k+l,0},\qquad
(\alpha_k^I)^\dagger=\alpha_{-k}^I.
$$

With [string tension](../../../../../string-tension.md) convention $\alpha'=(2\pi T)^{-1}$, the zero mode of the constraint gives

$$
\mathcal M_{\mathrm{cl}}^2=\frac1{\alpha'}\sum_{k>0}\alpha_{-k}\cdot\alpha_k.
$$

The longitudinal nonzero modes have already been removed in [light-cone gauge in string theory](../../../../../light-cone-gauge-in-string-theory.md). Quantum [normal ordering](../../../../../normal-ordering.md) introduces the [string intercept](../../../../../normal-ordering-constant-of-a-string.md) $a$, giving the [open bosonic string mass spectrum](../../../../../open-bosonic-string-mass-spectrum.md)

$$
\boxed{M^2=\frac{N-a}{\alpha'},\qquad
N=\sum_{k>0}\alpha_{-k}\cdot\alpha_k
=\sum_{k>0}k\,a_k^\dagger\cdot a_k,\quad
a_k^I=\alpha_k^I/\sqrt k.}
$$

Each [bosonic occupation number](../../../../../bosonic-occupation-number.md) is a nonnegative integer, so $N$ is a nonnegative integer weighted by oscillator frequency.

Suppressing the common momentum label, the [lowest light-cone levels of an open bosonic string](../../../../../lowest-light-cone-levels-of-an-open-bosonic-string.md) are

$$
\begin{aligned}
N=0:&\quad|0;p\rangle,\\
N=1:&\quad\alpha_{-1}^I|0;p\rangle,\\
N=2:&\quad\alpha_{-2}^I|0;p\rangle,\qquad
\alpha_{-1}^I\alpha_{-1}^J|0;p\rangle.
\end{aligned}
$$

The [oscillator vacuum](../../../../../oscillator-vacuum.md) is annihilated by every positive $\alpha_k^I$. At level one there are only $d$ vector polarizations. For a Lorentz-consistent vector, these are the transverse polarizations of a massless particle, transforming under the rotation part of its [massless particle little group](../../../../../massless-particle-little-group.md). A [massive vector](../../../../../massive-vector-particle.md) would need $D-1$ polarizations, including a scalar under $SO(d)$ that is absent here. Thus **the first bosonic vector level must be massless**, fixing $a=1$.

At level two the commuting [creation operators](../../../../../creation-operator.md) give a [symmetric square](../../../../../symmetric-square.md). Its scalar [trace](../../../../../matrix-trace.md) and [symmetric traceless square](../../../../../symmetric-trace-free-square-of-the-defining-orthogonal-representation.md), together with the mode-two vector, are the massive-spin-two decomposition above. In the consistent bosonic theory they form one [massive spin-two field](../../../../../massive-spin-two-field.md) with $m^2=1/\alpha'$. The covariant equations describe its propagation while eliminating the redundant components. For $D=26$ the transverse counts are $300+24=324$, the [symmetric traceless rank-two tensor](../../../../../symmetric-trace-free-square-of-the-defining-orthogonal-representation.md) dimension of $SO(25)$.

**Half-integer fermionic modes.** The [Neveu–Schwarz sector](../../../../../neveu-schwarz-sector.md) has antiperiodic [worldsheet Majorana fermions](../../../../../worldsheet-majorana-fermion.md). Its [Neveu–Schwarz fermionic oscillators](../../../../../neveu-schwarz-fermionic-oscillator.md) obey

$$
\{b_r^I,b_s^J\}=\delta^{IJ}\delta_{r+s,0},\qquad
(b_r^I)^\dagger=b_{-r}^I,\qquad r\in\mathbb Z+\tfrac12.
$$

The [oscillator vacuum](../../../../../oscillator-vacuum.md) satisfies $\alpha_k^I|0;p\rangle=0$ for $k>0$ and $b_r^I|0;p\rangle=0$ for $r>0$. A negative fermion mode is a [fermionic creation operator](../../../../../fermionic-creation-operator.md) for a transverse worldsheet excitation. The [Neveu–Schwarz level operator](../../../../../neveu-schwarz-level-operator.md) and mass condition are

$$
N=\sum_{k>0}\alpha_{-k}\cdot\alpha_k+\sum_{r>0}r\,b_{-r}\cdot b_r,\qquad
M^2=\frac{N-a_{\mathrm{NS}}}{\alpha'}.
$$

The smallest positive frequency is $1/2$, so the only first-excited states are

$$
\boxed{b_{-1/2}^I|0;p\rangle,\qquad N=\tfrac12.}
$$

The same vector-polarization argument requires them to be massless in Lorentz-consistent quantization, fixing $a_{\mathrm{NS}}=1/2$.

At $N=1$, $\alpha_{-1}^I|0;p\rangle$ is a vector, while $b_{-1/2}^Ib_{-1/2}^J|0;p\rangle$ is the [exterior square](../../../../../exterior-square.md): interchanging the indices changes the sign and equal indices give zero. Together they branch from an antisymmetric tensor:

$$
\boxed{\mathbb R^d\oplus\Lambda^2(\mathbb R^d)
=\Lambda^2(\mathbb R^{d+1})\downarrow SO(d).}
$$

Thus the [Neveu–Schwarz level-one massive tensor](../../../../../neveu-schwarz-level-one-massive-tensor.md) has $(D-1)(D-2)/2$ polarizations and mass squared $1/(2\alpha')$. It differs from spin two because the two-fermion tensor is antisymmetric and has neither the symmetric [trace](../../../../../matrix-trace.md)-free representation nor its scalar [trace](../../../../../matrix-trace.md). At $D=10$, the count is $8+28=36$, compared with $44$ for a massive spin-two field. The specified states are **before the GSO projection**; the usual tachyon-removing [GSO projection](../../../../../gso-projection.md) also removes this integer level.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 49](../../paper-49-split.md)
3. [Iii](../../split.md)
4. [2015](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
