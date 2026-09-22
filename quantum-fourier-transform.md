# Quantum Fourier transform

↑ **Parent:** [Quantum theory](quantum-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Quantum_Fourier_transform)

The quantum Fourier transform maps $|k\rangle$ to $N^{-1/2}\sum_j e^{2\pi ijk/N}|j\rangle$.

**Table of contents**

- [Dyadic quantum Fourier transform circuit](#dyadic-quantum-fourier-transform-circuit)
- [Product decomposition of a Fourier phase state](#product-decomposition-of-a-fourier-phase-state)
- [Fourier sample](#fourier-sample)
- [Quantum Fourier transform over a finite abelian group](#quantum-fourier-transform-over-a-finite-abelian-group)
- [Square of the quantum Fourier transform](#square-of-the-quantum-fourier-transform)
- [Quantum Fourier transform of a periodic coset state](#quantum-fourier-transform-of-a-periodic-coset-state)
- [Quantum period finding](#quantum-period-finding)
  - [Exact period recovery from a Fourier sample](#exact-period-recovery-from-a-fourier-sample)
    - [Two-sample exact period recovery](#two-sample-exact-period-recovery)
    - [Heralded exact quantum period finding when the period divides the register size](#heralded-exact-quantum-period-finding-when-the-period-divides-the-register-size)
      - [Quantum Fourier sampling of powers of three modulo ten](#quantum-fourier-sampling-of-powers-of-three-modulo-ten)
- [Hidden subgroup problem](#hidden-subgroup-problem)
  - [Discrete-logarithm Fourier sampling](#discrete-logarithm-fourier-sampling)
    - [Linear congruence from a discrete-logarithm Fourier sample](#linear-congruence-from-a-discrete-logarithm-fourier-sample)
  - [Coset state](#coset-state)
    - [Periodic coset state](#periodic-coset-state)
  - [Group shift operator](#group-shift-operator)
  - [Abelian hidden-subgroup Fourier sampling](#abelian-hidden-subgroup-fourier-sampling)
  - [Simon's problem](#simon-s-problem)
    - [Classical collision query bound for Simon's problem](#classical-collision-query-bound-for-simon-s-problem)
    - [Simon's algorithm](#simon-s-algorithm)
      - [Expected query count for Simon sampling](#expected-query-count-for-simon-sampling)
      - [Single-sample distribution in Simon's algorithm](#single-sample-distribution-in-simon-s-algorithm)
      - [Orthogonal complement over the binary field](#orthogonal-complement-over-the-binary-field)
  - [Stabilizer as a hidden subgroup](#stabilizer-as-a-hidden-subgroup)
- [Cyclic shift operator](#cyclic-shift-operator)
  - [Cyclic shift diagonalization by the quantum Fourier transform](#cyclic-shift-diagonalization-by-the-quantum-fourier-transform)
- [Quantum phase estimation](#quantum-phase-estimation)
  - [Quantum phase estimation tail bound](#quantum-phase-estimation-tail-bound)
  - [Near-grid quantum phase estimation](#near-grid-quantum-phase-estimation)
  - [Parallel phase multiplication by coherent fanout](#parallel-phase-multiplication-by-coherent-fanout)
  - [Quantum phase estimation with a maximally mixed target](#quantum-phase-estimation-with-a-maximally-mixed-target)
  - [Nearest-integer success bound for quantum phase estimation](#nearest-integer-success-bound-for-quantum-phase-estimation)
  - [Dyadic phase-gate identification](#dyadic-phase-gate-identification)
  - [Tensor-product eigenphase amplification](#tensor-product-eigenphase-amplification)
  - [Positive-phase fractional power of a unitary operator](#positive-phase-fractional-power-of-a-unitary-operator)
  - [Quantum spectral filtering](#quantum-spectral-filtering)
    - [Singular obstruction to normalized quantum matrix multiplication](#singular-obstruction-to-normalized-quantum-matrix-multiplication)
    - [Success probability of positive quantum spectral filtering](#success-probability-of-positive-quantum-spectral-filtering)
  - [Exact quantum phase estimation](#exact-quantum-phase-estimation)

## Dyadic quantum Fourier transform circuit

↑ **Parent:** [Quantum Fourier transform](quantum-fourier-transform.md)

In most-significant-bit-first order, let $x=x_1\cdots x_n$ and $0.x_j\cdots x_n=\sum_{l=j}^n x_l2^{-(l-j+1)}$. On a [computational-basis state](quantum-theory.md#computational-basis-state), process wire $j$ with a [Hadamard gate](quantum-theory.md#hadamard-gate), then [controlled phase gates](quantum-theory.md#controlled-phase-gate) $R_{l-j+1}$ controlled by unprocessed wire $l$ for each $l>j$. Wire $j$ becomes $(|0\rangle+e^{2\pi i0.x_j\cdots x_n}|1\rangle)/\sqrt2$. Reversing the final wire order yields the positive-exponent [quantum Fourier transform](quantum-fourier-transform.md). There are $n$ [Hadamard gates](quantum-theory.md#hadamard-gate) and $n(n-1)/2$ [controlled phase gates](quantum-theory.md#controlled-phase-gate). Physical reversal costs $\lfloor n/2\rfloor$ [swap operators](quantum-information-theory.md#swap-operator), each expressible as three [controlled-NOT gates](quantum-theory.md#controlled-not-gate), themselves implemented with [Hadamard gates](quantum-theory.md#hadamard-gate) and a [Controlled-Z gate](quantum-theory.md#controlled-z-gate). Thus the entire construction uses $O(n^2)$ gates from the specified family.

## Product decomposition of a Fourier phase state

↑ **Parent:** [Quantum Fourier transform](quantum-fourier-transform.md)

Write the integer label in most-significant-bit-first order as $l=\sum_jb_j2^{n-j}$. The phase factors as $e^{i\phi l}=\prod_je^{i\phi b_j2^{n-j}}$, giving the displayed [product state](bell-state.md#product-state). For dyadic Fourier phases this explains why the Fourier basis states are unentangled even though a general [quantum Fourier transform](quantum-fourier-transform.md) can create [entanglement](bell-state.md#entangled-state).

## Fourier sample

↑ **Parent:** [Quantum Fourier transform](quantum-fourier-transform.md)

A Fourier sample is a [computational-basis measurement](quantum-theory.md#quantum-measurement-in-the-computational-basis) outcome after applying a [quantum Fourier transform](quantum-fourier-transform.md) $F$ to a [quantum state](quantum-system.md#quantum-state) $|\psi\rangle$. Its distribution is given by the squared Fourier amplitudes. For a uniform periodic coset of spacing $r\mid N$, samples are the multiples $sN/r$ with uniform $s\in\mathbb Z_r$. Samples need not individually reveal the whole period: a [greatest common divisor](divisibility.md#greatest-common-divisor) can remove factors from a single reduced denominator, motivating [two-sample exact period recovery](#two-sample-exact-period-recovery).

## Quantum Fourier transform over a finite abelian group

↑ **Parent:** [Quantum Fourier transform](quantum-fourier-transform.md)

For a [finite abelian group](group.md#finite-abelian-group) $G$ with character group $\widehat G$, the quantum Fourier transform is

$$
|g\rangle\longmapsto\frac1{\sqrt{|G|}}\sum_{\chi\in\widehat G}\chi(g)|\chi\rangle,
$$

up to complex conjugation according to the transform convention.

## Square of the quantum Fourier transform

↑ **Parent:** [Quantum Fourier transform](quantum-fourier-transform.md)

The [root-of-unity filter](algebra.md#root-of-unity-filter) gives

$$
\operatorname{QFT}_N^2|x\rangle=|-x\bmod N\rangle.
$$

Thus $\operatorname{QFT}_N^4=I$, while the square is an involution whose eigenvalues lie in $\{1,-1\}$.

## Quantum Fourier transform of a periodic coset state

↑ **Parent:** [Quantum Fourier transform](quantum-fourier-transform.md)

Let $r$ divide $N$ and

$$
|\alpha\rangle=\frac1{\sqrt{N/r}}
\sum_{j=0}^{N/r-1}|x_0+jr\rangle.
$$

The geometric sum in the quantum Fourier transform vanishes unless $c$ is a multiple of $N/r$. Thus measurement after the transform returns the $r$ values

$$
c=0,\frac Nr,\ldots,(r-1)\frac Nr
$$

with equal probabilities $1/r$.

## Quantum period finding

↑ **Parent:** [Quantum Fourier transform](quantum-fourier-transform.md)

For a function of period $r$ dividing $N$, prepare a uniform superposition of inputs, evaluate the function into a second register, and measure that register. The first register becomes a periodic coset state. Applying the [quantum Fourier transform](quantum-fourier-transform.md) and measuring gives

$$
c=s\frac Nr,
\qquad 0\leq s<r.
$$

### Exact period recovery from a Fourier sample

↑ **Parent:** [Quantum period finding](#quantum-period-finding)

For the exact sample $c=sN/r$, reducing

$$
\frac cN=\frac sr
$$

recovers denominator $r/\gcd(s,r)$. Thus one sample reveals the full period exactly when $s$ is coprime to $r$; otherwise it reveals only a proper divisor and the algorithm must obtain more information.

#### Two-sample exact period recovery

↑ **Parent:** [Exact period recovery from a Fourier sample](#exact-period-recovery-from-a-fourier-sample)

Suppose a function has least period $r\mid N$ and distinct values on distinct period cosets. Two independent [Fourier samples](#fourier-sample) have the form $c_j=s_jN/r$ with uniform $s_j\in\mathbb Z_r$. The displayed candidate is $r/\gcd(r,s_1,s_2)$, so exact recovery occurs when no prime divisor of $r$ divides both residues. The [Chinese remainder theorem](mathematics.md#chinese-remainder-theorem) gives probability $\prod_{\ell\mid r}(1-\ell^{-2})\ge1/\zeta(2)=6/\pi^2$, using the [Euler product](analytic-number-theory.md#euler-product). Unlike a single-sample coprimality probability, this bound is uniformly greater than one half. A candidate-period test makes successful recovery heralded when such a test is available.

#### Heralded exact quantum period finding when the period divides the register size

↑ **Parent:** [Exact period recovery from a Fourier sample](#exact-period-recovery-from-a-fourier-sample)

Suppose a function on $\mathbb Z_N$ has least period $r\mid N$ and is injective on each period. A Fourier sample $c=sN/r$ gives the candidate denominator $q=r/\gcd(s,r)$. If equality of function values can be tested efficiently, then $q$ is the full period exactly when $f(q)=f(0)$, so each successful run is certified. A sample succeeds with probability $\varphi(r)/r$, and an inverse-polylogarithmic lower bound for this ratio permits amplification to constant success probability with polynomially many repetitions.

##### Quantum Fourier sampling of powers of three modulo ten

↑ **Parent:** [Heralded exact quantum period finding when the period divides the register size](#heralded-exact-quantum-period-finding-when-the-period-divides-the-register-size)

The function $f(x)=3^x\bmod10$ on $\mathbb Z_{12}$ has period four. Measuring function value $3$ in its uniform input-output state leaves $(|1\rangle+|5\rangle+|9\rangle)/\sqrt3$. The quantum Fourier transform modulo twelve then returns each of $0,3,6,9$ with probability $1/4$.

## Hidden subgroup problem

↑ **Parent:** [Quantum Fourier transform](quantum-fourier-transform.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Hidden_subgroup_problem)

The hidden subgroup problem asks for a subgroup $H\leq G$ given an oracle $f:G\to X$ that is constant on each left coset of $H$ and takes different values on different cosets. Abelian instances are solved by preparing coset states and applying a group [quantum Fourier transform](quantum-fourier-transform.md).

### Discrete-logarithm Fourier sampling

↑ **Parent:** [Hidden subgroup problem](#hidden-subgroup-problem)

For a [generator of a group](group.md#generator-of-a-group) $g$ of order $M$ and $x=g^y$, the function $f(a,b)=g^ax^{-b}$ hides the [subgroup](group.md#subgroup) $\{(yb,b):b\in\mathbb Z_M\}$ of $\mathbb Z_M^2$. Each [fiber](function.md#fiber-of-a-function) is an affine [coset](group-theory.md#coset) $\{(yb+k,b):b\in\mathbb Z_M\}$. Measuring the function register gives its normalized [coset state](#coset-state). Applying the positive-exponent [quantum Fourier transform](quantum-fourier-transform.md) to both input registers gives amplitude

$$
\frac{e^{2\pi ikc_1/M}}{M\sqrt M}\sum_{b=0}^{M-1}e^{2\pi ib(yc_1+c_2)/M}.
$$

The [finite geometric series](sequence-and-series.md#finite-geometric-series) vanishes off $c_2=-yc_1$ and equals $M$ on that line. Thus each allowed output pair has [probability](probability-theory.md#probability) $1/M$, independently of the coset offset. If $\gcd(c_1,M)=1$, a [modular inverse](number-theory.md#modular-multiplicative-inverse) recovers $y=-c_2c_1^{-1}$.

#### Linear congruence from a discrete-logarithm Fourier sample

↑ **Parent:** [Discrete-logarithm Fourier sampling](#discrete-logarithm-fourier-sampling)

Let $d=\gcd(c_1,M)$. A supported sample guarantees $d\mid c_2$. Dividing its [linear congruence](modular-arithmetic.md#linear-congruence) by $d$ gives an invertible coefficient modulo $M/d$ and a unique residue $y_0$ there. The $d$ compatible [discrete logarithms](coding-theory.md#discrete-logarithm-problem) modulo $M$ are $y_0+jM/d$ for $0\leq j<d$. Only $d=1$ determines the [discrete logarithm](coding-theory.md#discrete-logarithm-problem) from the sample alone; $(c_1,c_2)=(0,0)$ conveys no information for $M>1$.

### Coset state

↑ **Parent:** [Hidden subgroup problem](#hidden-subgroup-problem)

For a finite group $G$, subgroup $H$, and $g\in G$, the coset state is the uniform superposition

$$
|gH\rangle=\frac1{\sqrt{|H|}}\sum_{h\in H}|gh\rangle.
$$

#### Periodic coset state

↑ **Parent:** [Coset state](#coset-state)

For $r\mid N$, a periodic coset state in the computational basis of $\mathbb Z_N$ is

$$
\frac1{\sqrt{N/r}}\sum_{j=0}^{N/r-1}|x_0+jr\rangle.
$$

It is the [coset state](#coset-state) of the subgroup $r\mathbb Z_N$ translated by $x_0$.

### Group shift operator

↑ **Parent:** [Hidden subgroup problem](#hidden-subgroup-problem)

For a [finite abelian group](group.md#finite-abelian-group) $G$, $U(h)|g\rangle=|g+h\rangle$ defines the [regular representation](representation-theory.md#regular-representation) on the basis labelled by $G$. The [linear characters](representation-theory.md#linear-character) give the common [eigenbasis](linear-operator-theory.md#eigenbasis)

$$
|v_\chi\rangle=|G|^{-1/2}\sum_g\overline{\chi(g)}|g\rangle,
\qquad U(h)|v_\chi\rangle=\chi(h)|v_\chi\rangle.
$$

[Character orthogonality](representation-theory.md#character-orthogonality) proves orthonormality, and changing variables by the [translation in a group](group.md#translation-in-a-group) proves the eigenvalue formula.

### Abelian hidden-subgroup Fourier sampling

↑ **Parent:** [Hidden subgroup problem](#hidden-subgroup-problem)

Measuring the [coset state](#coset-state) $|g_0+K\rangle$ in the [group shift operator](#group-shift-operator) [eigenbasis](linear-operator-theory.md#eigenbasis) samples uniformly from the [annihilator of a subgroup of a finite abelian group](group.md#annihilator-of-a-subgroup-of-a-finite-abelian-group) $K^\perp$. Indeed,

$$
\langle v_\chi|g_0+K\rangle
=\frac{\chi(g_0)}{\sqrt{|G||K|}}\sum_{k\in K}\chi(k),
$$

so the [character-sum cancellation lemma](group.md#character-sum-cancellation-lemma) gives probability $|K|/|G|$ on $K^\perp$ and zero elsewhere. The [modulus](complex-analysis.md#modulus) of $\chi(g_0)$ is one, so the offset has no effect on the distribution.

<h3 id="simon-s-problem">Simon's problem</h3>

↑ **Parent:** [Hidden subgroup problem](#hidden-subgroup-problem)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Simon's_problem)

Simon's problem asks for the hidden string $p\in\{0,1\}^n$ promised by $f(x)=f(y)$ exactly when $x\mathbin\oplus y\in\{0^n,p\}$. It is the [hidden subgroup problem](#hidden-subgroup-problem) on $(\mathbb Z_2)^n$ with hidden subgroup $\{0^n,p\}$.

<h4 id="classical-collision-query-bound-for-simon-s-problem">Classical collision query bound for Simon's problem</h4>

↑ **Parent:** [Simon's problem](#simon-s-problem)

For an unknown nonzero period, a collision $f(x)=f(y)$ reveals the period $x\mathbin\oplus y$. [Birthday problem](probability-and-statistics.md#birthday-problem) sampling finds one using $O(2^{n/2})$ queries with bounded error. A matching lower bound follows by choosing the period and output labels randomly: without a collision, $q$ queries rule out at most $\binom q2$ candidate periods. For $q=o(2^{n/2})$, almost all periods remain consistent with the transcript. The exponential separation is in query complexity, compared with [Simon's algorithm](#simon-s-algorithm)'s linear quantum query count.

<h4 id="simon-s-algorithm">Simon's algorithm</h4>

↑ **Parent:** [Simon's problem](#simon-s-problem)

Simon's algorithm prepares hidden-subgroup [coset states](#coset-state), applies the [quantum Fourier transform](quantum-fourier-transform.md) over $(\mathbb Z_2)^n$, and samples vectors $y$ satisfying $y\cdot p=0$ over $\mathbb F_2$. Repeated samples and [Gaussian elimination](numerical-linear-algebra.md#gaussian-elimination) recover $p$ with $O(n)$ oracle queries and polynomial computation.

##### Expected query count for Simon sampling

↑ **Parent:** [Simon's algorithm](#simon-s-algorithm)

With a nonzero hidden period, [Simon's algorithm](#simon-s-algorithm) samples uniformly from its $(n-1)$-dimensional [orthogonal complement over the binary field](#orthogonal-complement-over-the-binary-field). At rank $k$, a new sample raises the rank with probability $1-2^{k-(n-1)}$. Summing the geometric waiting times gives an expected $n-1+\sum_{j=1}^{n-1}(2^j-1)^{-1}<n+1$ queries. After $n-1+c$ samples, the probability of insufficient rank is less than $2^{-c}$, by a [union bound](probability-inequality.md#boole-s-inequality) over the nonzero linear functionals that could annihilate all samples.

<h5 id="single-sample-distribution-in-simon-s-algorithm">Single-sample distribution in Simon's algorithm</h5>

↑ **Parent:** [Simon's algorithm](#simon-s-algorithm)

If the hidden string is zero, one oracle-Hadamard run samples every $y\in\mathbb F_2^n$ with probability $2^{-n}$. If the hidden string is nonzero, it samples every $y$ satisfying $y\cdot p=0$ with probability $2^{-(n-1)}$ and every other string with probability zero. Pairing $x$ with $x\mathbin\oplus p$ makes the forbidden amplitudes cancel.

##### Orthogonal complement over the binary field

↑ **Parent:** [Simon's algorithm](#simon-s-algorithm)

For a subspace $W\leq\mathbb F_2^n$, its orthogonal complement is $W^\perp=\{y:x\cdot y=0\text{ for every }x\in W\}$, where the dot product is evaluated modulo two.

### Stabilizer as a hidden subgroup

↑ **Parent:** [Hidden subgroup problem](#hidden-subgroup-problem)

For a [group action](group-action.md) $F:G\times X\to X$ and fixed $x$, the orbit map $f_x(g)=F(g,x)$ hides the [stabilizer subgroup](group-action.md#stabilizer-subgroup) $G_x$: $f_x(g)=f_x(h)$ exactly when $h^{-1}g\in G_x$, equivalently when $g$ and $h$ lie in the same left coset of $G_x$.

## Cyclic shift operator

↑ **Parent:** [Quantum Fourier transform](quantum-fourier-transform.md)

On a basis indexed by $\mathbb Z_N$, a cyclic shift operator has the form $U(a)|b\rangle=|a+b\bmod N\rangle$. The [quantum Fourier transform](quantum-fourier-transform.md) simultaneously diagonalizes all such shifts.

### Cyclic shift diagonalization by the quantum Fourier transform

↑ **Parent:** [Cyclic shift operator](#cyclic-shift-operator)

For the cyclic shift $S|j\rangle=|j+1\bmod N\rangle$ and the convention

$$
\operatorname{QFT}_N|k\rangle=N^{-1/2}\sum_j e^{2\pi ijk/N}|j\rangle,
$$

the Fourier states obey

$$
S\operatorname{QFT}_N|k\rangle=e^{-2\pi ik/N}\operatorname{QFT}_N|k\rangle.
$$

Consequently $S=\operatorname{QFT}_N D\operatorname{QFT}_N^{-1}$, where $D|k\rangle=e^{-2\pi ik/N}|k\rangle$.

## Quantum phase estimation

↑ **Parent:** [Quantum Fourier transform](quantum-fourier-transform.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Quantum_phase_estimation)

Given controlled powers of a unitary $U$ and an eigenstate $U|\psi\rangle=e^{2\pi i\phi}|\psi\rangle$, quantum phase estimation outputs an approximation to $\phi$. If the input is a superposition of eigenstates, measurement selects an eigenphase with probability equal to the squared magnitude of its coefficient.

### Quantum phase estimation tail bound

↑ **Parent:** [Quantum phase estimation](#quantum-phase-estimation)

Let $L=2^t$, let $j_0$ be the nearest label to $L\phi$, and let $m\geq2$. The exact [quantum phase estimation](#quantum-phase-estimation) amplitude is $L^{-1}\sum_{a=0}^{L-1}e^{2\pi ia(\phi-j/L)}$. The sine bound on circular distances gives probability at most $1/(4d_j^2)$, where $d_j$ is the centered distance from $j$ to $L\phi$. At label distance $\ell$ from $j_0$, $|d_j|\geq\ell-1/2$, with at most two labels for each $\ell$. Since $(\ell-1/2)^{-2}\leq[(\ell-1)\ell]^{-1}$, the tail telescopes to the displayed bound. Adding $u$ control [qubits](quantum-system.md#qubit) beyond $b$ desired phase bits gives circular accuracy below $2^{-b}$ with failure probability at most $[2(2^u-1)]^{-1}$.

### Near-grid quantum phase estimation

↑ **Parent:** [Quantum phase estimation](#quantum-phase-estimation)

For register size $N=2^t$ and [eigenphase](vector-space.md#eigenphase) $\phi=2\pi n/N+\epsilon$, the amplitude of decoded label $m$ is $N^{-1}\sum_{k=0}^{N-1}e^{ik(\phi-2\pi m/N)}$. The [finite geometric series](sequence-and-series.md#finite-geometric-series) gives $P(n)=\sin^2(N\epsilon/2)/[N^2\sin^2(\epsilon/2)]$. If $N|\epsilon|\ll1$, this is $1-(N^2-1)\epsilon^2/12+O(N^4\epsilon^4)$. Thus the nearest exactly representable phase is returned with [probability](probability-theory.md#probability) near one, not with certainty unless the offset vanishes.

// Target: quantum-error-correction.bigb

### Parallel phase multiplication by coherent fanout

↑ **Parent:** [Quantum phase estimation](#quantum-phase-estimation)

Use [CNOT gates](quantum-theory.md#controlled-not-gate) to encode one logical [qubit](quantum-system.md#qubit) and $r-1$ zero ancillas into the repetition subspace spanned by $|0^r\rangle,|1^r\rangle$. Apply the [phase gate](quantum-theory.md#phase-gate) in parallel to all $r$ physical [qubits](quantum-system.md#qubit), then undo the encoding. The logical phase is multiplied by $r$ in one oracle-time layer. This copies computational-basis labels coherently rather than cloning an arbitrary [quantum state](quantum-system.md#quantum-state). Blocks of sizes $1,2,4,\ldots,2^{n-1}$ prepare a dyadic Fourier phase state using $2^n-1$ parallel oracle applications.

### Quantum phase estimation with a maximally mixed target

↑ **Parent:** [Quantum phase estimation](#quantum-phase-estimation)

For a $d$-dimensional [unitary operator](vector-space.md#unitary-operator) $V=\sum_{j=1}^de^{i\phi_j}|v_j\rangle\langle v_j|$, a [maximally mixed state](density-matrix.md#maximally-mixed-state) $I/d$ on its target is the equal mixture of these [orthonormal](inner-product.md#orthonormal-set) [eigenvectors](linear-operator-theory.md#eigenvector). Therefore [quantum phase estimation](#quantum-phase-estimation) with register size $L$ produces label $m$ with [probability](probability-theory.md#probability)

$$
p(m)=\frac1d\sum_{j=1}^d|a_m(\phi_j)|^2,\qquad a_m(\phi)=\frac1L\sum_{x=0}^{L-1}e^{ix(\phi-2\pi m/L)}.
$$

This follows by [linearity](vector-space.md#linearity) of [unitary time evolution](quantum-system.md#unitary-time-evolution) and the [Born rule](wave-function.md#born-rule) on the spectral mixture. If every [eigenphase](vector-space.md#eigenphase) has an exact $L$-grid label, that label has [probability](probability-theory.md#probability) equal to its multiplicity divided by $d$. Otherwise the exact distribution has tails, and the nearest labels are guaranteed only the [nearest-integer success bound for quantum phase estimation](#nearest-integer-success-bound-for-quantum-phase-estimation) weighted by the corresponding spectral [probabilities](probability-theory.md#probability).

### Nearest-integer success bound for quantum phase estimation

↑ **Parent:** [Quantum phase estimation](#quantum-phase-estimation)

For a [unitary operator](vector-space.md#unitary-operator) [eigenphase](vector-space.md#eigenphase) $\phi$, an $n$-qubit [quantum phase estimation](#quantum-phase-estimation) register of size $L=2^n$ has output [probability amplitude](wave-function.md#probability-amplitude)

$$
a_m(\phi)=\frac1L\sum_{x=0}^{L-1}e^{ix(\phi-2\pi m/L)}.
$$

Choose the nearest integer label $m$ to $L\phi/(2\pi)$, with labels understood modulo $L$, and put $d=L\phi/(2\pi)-m$, taking the representative $|d|\leq1/2$. The [finite geometric series](sequence-and-series.md#finite-geometric-series) gives $|a_m|=|\sin(\pi d)|/[L|\sin(\pi d/L)|]$. For $0<|d|\leq1/2$, [concavity](real-analysis.md#concave-function) of sine gives $|\sin(\pi d)|\geq2|d|$, while $|\sin(\pi d/L)|\leq\pi|d|/L$. Thus the [probability](probability-theory.md#probability) of the nearest label is at least $4/\pi^2$. At $d=0$ it is exactly one. If two labels tie for nearest, each satisfies the bound.

### Dyadic phase-gate identification

↑ **Parent:** [Quantum phase estimation](#quantum-phase-estimation)

For the [phase gate](quantum-theory.md#phase-gate) $R_a=\operatorname{diag}(1,e^{2\pi ia/2^n})$, apply powers $R_a^{2^{n-1}},\ldots,R_a$ to a [uniform quantum superposition](quantum-theory.md#uniform-quantum-superposition) on $n$ qubits. Binary positional weights multiply the phases into $e^{2\pi iax/2^n}$ on basis vector $|x\rangle$. The inverse [quantum Fourier transform](quantum-fourier-transform.md) returns $|a\rangle$ exactly, by [orthogonality of roots of unity](algebra.md#orthogonality-of-roots-of-unity). Preparing the powers by repeated applications uses $2^n-1$ copies of $R_a$; this does not claim a number of gate calls polynomial in $n$. If $a$ is odd, its powers generate the entire set of dyadic phase gates because $a$ has a [modular inverse](number-theory.md#modular-multiplicative-inverse) modulo $2^n$.

### Tensor-product eigenphase amplification

↑ **Parent:** [Quantum phase estimation](#quantum-phase-estimation)

An [eigenstate](energy-eigenvalue.md#eigenstate) with phase $\phi$ becomes an eigenstate with phase $n\phi$ under the tensor product of $n$ copies of the [unitary operator](vector-space.md#unitary-operator). A promise $0\le\phi<1/n$ prevents modulo-one aliasing. For $n=2^s$ and dyadic $\phi=x/2^m$, [exact quantum phase estimation](#exact-quantum-phase-estimation) then needs $m-s$ phase bits and $2^{m-s}-1$ queries to a supplied joint controlled oracle. This is a saving in joint-oracle calls, not in the total number of individual oracle invocations needed to build that joint operation.

### Positive-phase fractional power of a unitary operator

↑ **Parent:** [Quantum phase estimation](#quantum-phase-estimation)

Choose eigenphase representatives $0\leq\phi_j<1$ for a [unitary operator](vector-space.md#unitary-operator) $U$ and a positive integer $M$. Its positive-phase fractional power acts on each [eigenstate](energy-eigenvalue.md#eigenstate) by $e^{2\pi i\phi_j/M}$. This branch uses arguments in $[0,2\pi)$ and can differ from the usual complex principal branch using $(-\pi,\pi]$. For exactly dyadic phases, [exact quantum phase estimation](#exact-quantum-phase-estimation) stores each label in a coherent phase register; bitwise [phase gates](quantum-theory.md#phase-gate) multiply it by the required phase, and inverse phase estimation removes the labels. Keeping the phase register unmeasured preserves arbitrary [eigenstate](energy-eigenvalue.md#eigenstate) superpositions and resets the [ancilla qubits](quantum-information-theory.md#ancilla-qubit). With only controlled-$U$ and controlled-$U^{-1}$ primitives, the direct method uses $2(2^n-1)$ oracle calls for $n$ exact phase bits.

### Quantum spectral filtering

↑ **Parent:** [Quantum phase estimation](#quantum-phase-estimation)

Let a [Hermitian operator](hilbert-space.md#hermitian-operator) $A$ have dyadic [eigenvalues](linear-operator-theory.md#eigenvalue) $\lambda_j=c_j/2^t$ in $[0,1)$ for known $t$, with controlled access to the [unitary operator](vector-space.md#unitary-operator) $U=e^{2\pi iA}$. This interval ensures that different [eigenvalues](linear-operator-theory.md#eigenvalue) have different [eigenphases](vector-space.md#eigenphase); exact representability alone would not exclude phase aliasing, as $0$ and $1$ both give phase zero. Let a real [function](function.md) $h$ obey $|h(\lambda_j)|\leq1$, and assume the required [quantum variable rotations](quantum-theory.md#quantum-variable-rotation) are available. Coherent [exact quantum phase estimation](#exact-quantum-phase-estimation), a [quantum variable rotation](quantum-theory.md#quantum-variable-rotation) and [uncomputation](quantum-theory.md#uncomputation) implement

$$
|u_j\rangle|0\rangle\longmapsto|u_j\rangle\left(\sqrt{1-h(\lambda_j)^2}|0\rangle+h(\lambda_j)|1\rangle\right).
$$

[Postselection](quantum-measurement.md#postselection) on flag one gives $h(A)|b\rangle$ normalized, with [probability](probability-theory.md#probability) $\|h(A)|b\rangle\|^2$, provided this vector is nonzero. Erasing the [eigenvalue](linear-operator-theory.md#eigenvalue) label by [uncomputation](quantum-theory.md#uncomputation) is essential to preserve coherence between different [eigenvectors](linear-operator-theory.md#eigenvector). On this dyadic spectrum, $U^{2^t}=I$ gives $U^{-1}=U^{2^t-1}$, so reversing the phase-estimation gates is possible using forward controlled-$U$ calls. The choice $h(\lambda)=\lambda$ multiplies by $A$; a scaled reciprocal gives the different filter used in the [HHL algorithm](quantum-theory.md#hhl-algorithm).

#### Singular obstruction to normalized quantum matrix multiplication

↑ **Parent:** [Quantum spectral filtering](#quantum-spectral-filtering)

If $|b\rangle$ lies in the [kernel](kernel-of-a-linear-map.md) of $A$, then $A|b\rangle=0$ has no normalized [quantum state](quantum-system.md#quantum-state). A request to produce that normalized vector with positive [probability](probability-theory.md#probability) is consequently undefined. For example, $A=\operatorname{diag}(0,1/2)$ on one [qubit](quantum-system.md#qubit) has distinct dyadic [eigenvalues](linear-operator-theory.md#eigenvalue), but annihilates $|0\rangle$. The corrected filtering assertion requires $A|b\rangle\neq0$; it cannot be repaired by assigning a positive success probability to this input.

#### Success probability of positive quantum spectral filtering

↑ **Parent:** [Quantum spectral filtering](#quantum-spectral-filtering)

For $0\leq A<I$ and normalized $|b\rangle=\sum_j\beta_j|u_j\rangle$, filtering by $h(\lambda)=\lambda$ succeeds with

$$
P=\sum_j|\beta_j|^2\lambda_j^2\geq\lambda_{\min}^2.
$$

The inequality follows by replacing each nonnegative $\lambda_j^2$ by its minimum and using $\sum_j|\beta_j|^2=1$. Equality holds exactly when all occupied [eigenvectors](linear-operator-theory.md#eigenvector) belong to the minimum-[eigenvalue](linear-operator-theory.md#eigenvalue) [eigenspace](linear-operator-theory.md#eigenspace). If $\lambda_{\min}=0$, success is positive exactly for inputs outside the [kernel](kernel-of-a-linear-map.md) of $A$.

### Exact quantum phase estimation

↑ **Parent:** [Quantum phase estimation](#quantum-phase-estimation)

If $U|\psi\rangle=e^{2\pi ij/N}|\psi\rangle$, controlled powers of $U$ applied to a uniform $N$-state control register produce

$$
|\phi_j\rangle=\frac1{\sqrt N}\sum_{k=0}^{N-1}e^{2\pi ijk/N}|k\rangle.
$$

These states are the Fourier basis. Applying the inverse quantum Fourier transform and measuring returns $j$ with probability one.

## ↑ Ancestors (4)

1. [Quantum theory](quantum-theory.md)
2. [Branches of physics](physics.md#branches-of-physics)
3. [Physics](physics.md)
4. [Codex Wiki](README.md)

## ← Incoming links (52)

- [Cyclic shift operator](#cyclic-shift-operator)
- [Discrete-logarithm Fourier sampling](#discrete-logarithm-fourier-sampling)
- [Dyadic phase-gate identification](#dyadic-phase-gate-identification)
- [Dyadic quantum Fourier transform circuit](#dyadic-quantum-fourier-transform-circuit)
- [Fourier sample](#fourier-sample)
- [Hidden subgroup problem](#hidden-subgroup-problem)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-25.md#4/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-33.md#5/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-53.md#2/1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-58.md#2/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-58.md#1/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-58.md#1/d/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-57.md#4/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-57.md#4/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-57.md#4/d/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-49.md#4/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-67.md#1/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-67.md#1/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-67.md#4/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-58.md#1/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-58.md#1/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-61.md#1/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-61.md#3/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-324.md#1/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-324.md#1/iii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-324.md#1/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-324.md#1/b/iii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-324.md#3/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-324.md#3/b/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/ii/paper-3.md#15d/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/ii/paper-3.md#15d/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/ii/paper-4.md#10d/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/iii/paper-324.md#1/a/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/iii/paper-324.md#1/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/iii/paper-324.md#4/a/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2020/ii/paper-4.md#10c/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2021/iii/paper-324.md#1/b/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2021/iii/paper-324.md#2/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2022/iii/paper-324.md#4/b/iii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/ii/paper-2.md#15d/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/ii/paper-2.md#15d/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/ii/paper-3.md#10d/d/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2024/ii/paper-2.md#10e/d/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2024/iii/paper-324.md#1/c/iii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2025/iii/paper-324.md#3/a/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2025/iii/paper-324.md#3/c/solution)
- [Solution](past-exam-of-the-quantum-information-course-of-the-university-of-cambridge/2014/paper-1.md#2/solution)
- [Product decomposition of a Fourier phase state](#product-decomposition-of-a-fourier-phase-state)
- [Quantum Fourier sampling bound for order finding](quantum-theory.md#quantum-fourier-sampling-bound-for-order-finding)
- [Quantum period finding](#quantum-period-finding)
- [Qutrit linear-function identification](quantum-theory.md#qutrit-linear-function-identification)
- [Simon's algorithm](#simon-s-algorithm)
