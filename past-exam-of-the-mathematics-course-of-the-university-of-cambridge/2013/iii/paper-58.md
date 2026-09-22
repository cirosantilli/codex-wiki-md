# Paper 58

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2013/paper_58.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2013/paper_58.pdf)

**Table of contents**

- [1](#1)
  - [a](#1/a)
    - [Solution](#1/a/solution)
  - [b](#1/b)
    - [Solution](#1/b/solution)
- [2](#2)
  - [i](#2/i)
    - [Solution](#2/i/solution)
  - [ii](#2/ii)
    - [Solution](#2/ii/solution)
  - [iii](#2/iii)
    - [Solution](#2/iii/solution)
- [3](#3)
  - [a](#3/a)
    - [Solution](#3/a/solution)
  - [b](#3/b)
    - [i](#3/b/i)
      - [Solution](#3/b/i/solution)
    - [ii](#3/b/ii)
      - [Solution](#3/b/ii/solution)
    - [iii](#3/b/iii)
      - [Solution](#3/b/iii/solution)
- [4](#4)
  - [a](#4/a)
    - [i](#4/a/i)
      - [Solution](#4/a/i/solution)
    - [ii](#4/a/ii)
      - [Solution](#4/a/ii/solution)
  - [b](#4/b)
    - [i](#4/b/i)
      - [Solution](#4/b/i/solution)
    - [ii](#4/b/ii)
      - [Solution](#4/b/ii/solution)
    - [iii](#4/b/iii)
      - [Solution](#4/b/iii/solution)

## 1

↑ **Parent:** [Paper 58](paper-58.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

The PDF's small superscript is essential: $f(x)=a^x\bmod N$. Interpret $r$ as the least positive period, the [multiplicative order](../../../number-theory.md#multiplicative-order) of $a$ modulo $N$. If one permitted an unspecified nonminimal period, the answer would not be identifiable; for example, $a=1,N=8$ gives the same constant function with period one or period eight. Under the promised periodic modular-exponential interpretation, $a^r\equiv1\pmod N$, so $a$ is a unit. Thus

$$
a^x\equiv a^y\pmod N\quad\Longleftrightarrow\quad r\mid(x-y).
$$

In particular, different residue classes modulo $r$ have different function values, which is necessary for the usual [quantum period finding](../../../quantum-theory.md#quantum-period-finding) coset argument.

Prepare $N^{-1/2}\sum_x|x\rangle|1\rangle$ by applying the [quantum Fourier transform](../../../quantum-theory.md#quantum-fourier-transform) to the first register. Use repeated squaring to precompute $a^{2^j}\bmod N$, then multiply the value register by that known number controlled on bit $j$ of $x$. These controlled modular multiplications are reversible because $a$ is a unit; their inverses use the modular inverses of the same constants. This produces $N^{-1/2}\sum_x|x\rangle|a^x\bmod N\rangle$ with a polynomial number of the assumed arithmetic operations. Known work registers can be uncomputed.

Measure the value register. Since $r\mid N$, its fiber is exactly one coset, and the first register becomes

$$
\frac1{\sqrt{N/r}}\sum_{\ell=0}^{N/r-1}|x_0+\ell r\rangle.
$$

The [quantum Fourier transform of a periodic coset state](../../../quantum-theory.md#quantum-fourier-transform-of-a-periodic-coset-state) is supported uniformly on the $r$ outcomes $c=jN/r$, $0\le j<r$. Indeed the inner [geometric series](../../../real-analysis.md#geometric-series) $\sum_{\ell=0}^{N/r-1}e^{2\pi i\ell rc/N}$ is zero unless $(N/r)\mid c$, and each allowed amplitude has modulus $1/\sqrt r$.

Take two independent [Fourier samples](../../../quantum-theory.md#fourier-sample) $c_1,c_2$ and return

$$
\boxed{\widehat r=\frac N{\gcd(N,c_1,c_2)}=\frac r{\gcd(r,j_1,j_2)}.}
$$

This is [two-sample exact period recovery](../../../quantum-theory.md#two-sample-exact-period-recovery). The [Chinese remainder theorem](../../../mathematics.md#chinese-remainder-theorem) makes divisibility of independent uniform residues independent across the different prime divisors of $r$. For each such prime $\ell$, both $j_1$ and $j_2$ are divisible by $\ell$ with probability $\ell^{-2}$. Therefore

$$
\Pr(\widehat r=r)=\prod_{\ell\mid r\atop\ell\ {\rm prime}}(1-\ell^{-2})\ge\prod_{\ell\ {\rm prime}}(1-\ell^{-2})=\frac1{\zeta(2)}=\frac6{\pi^2}>\frac12.
$$

The number-theoretic facts used here are the [Chinese remainder theorem](../../../mathematics.md#chinese-remainder-theorem), the [Euler product](../../../analytic-number-theory.md#euler-product) for the [Riemann zeta function](../../../analytic-number-theory.md#riemann-zeta-function) at two, and $\zeta(2)=\pi^2/6$. The candidate can also be certified by $a^{\widehat r}\equiv1\pmod N$: it divides the least period, so this equality holds exactly when it is the full period. Each preparation, reversible evaluation, [QFT](../../../quantum-theory.md#quantum-fourier-transform), measurement and [greatest common divisor](../../../number-theory.md#greatest-common-divisor) calculation has the assumed or standard [polynomial time](../../../computer-science.md#polynomial-time) cost in $\log N$. Two runs suffice for the desired constant success probability. **[Quantum period finding](../../../quantum-theory.md#quantum-period-finding) recovers the least period with probability at least $6/\pi^2$ in [polynomial time](../../../computer-science.md#polynomial-time).**

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

Use the [quantum Fourier transform](../../../quantum-theory.md#quantum-fourier-transform) convention $F_N|k\rangle=N^{-1/2}\sum_{j=0}^{N-1}\omega^{jk}|j\rangle$, where $\omega=e^{2\pi i/N}$. Reindexing the shifted sum gives

$$
S F_N|k\rangle=\frac1{\sqrt N}\sum_j\omega^{jk}|j+1\rangle=\omega^{-k}\frac1{\sqrt N}\sum_{\ell}\omega^{\ell k}|\ell\rangle.
$$

Thus the [cyclic shift operator](../../../quantum-theory.md#cyclic-shift-operator) has these [eigenvectors](../../../linear-operator-theory.md#eigenvector), with [eigenvalues](../../../linear-operator-theory.md#eigenvalue) $e^{-2\pi i k/N}$. This is [cyclic shift diagonalization by the quantum Fourier transform](../../../quantum-theory.md#cyclic-shift-diagonalization-by-the-quantum-fourier-transform), and it implies $S=F_ND F_N^\dagger$ with $D|k\rangle=\omega^{-k}|k\rangle$.

For $N=4$, the binary encoding is $k=2x+y$, with $x$ the more significant [qubit](../../../quantum-mechanics.md#qubit). The required diagonal phase is

$$
e^{-2\pi i(2x+y)/4}=(-1)^x(-i)^y,
$$

so $D=P_{-1}\otimes P_{-i}$. **The allowed-gate circuit is therefore**

$$
\boxed{S=\operatorname{QFT}_4(P_{-1}\otimes P_{-i})\operatorname{QFT}_4^{-1}.}
$$

In execution order, apply the inverse [QFT](../../../quantum-theory.md#quantum-fourier-transform), then the two [phase gates](../../../quantum-theory.md#phase-gate), then the forward [QFT](../../../quantum-theory.md#quantum-fourier-transform). There is no extra global phase. Reversing the Fourier sign convention would conjugate both [phase gate](../../../quantum-theory.md#phase-gate) parameters.

## 2

↑ **Parent:** [Paper 58](paper-58.md)

<h3 id="2/i">i</h3>

↑ **Parent:** [2](#2)

<h4 id="2/i/solution">Solution</h4>

↑ **Parent:** [I](#2/i)

A good item must exist, so assume $1\le k<N$; if $k=0$, the requested search is impossible, while $k=N$ makes every output good. Put $p=k/N$ and $\theta=\arcsin\sqrt p$. Normalize the good and bad components of the [uniform superposition state](../../../quantum-circuit.md#uniform-superposition-state) as

$$
|g\rangle=\frac1{\sqrt k}\sum_{f(x)=1}|x\rangle,\qquad|b\rangle=\frac1{\sqrt{N-k}}\sum_{f(x)=0}|x\rangle,\qquad|\psi_0\rangle=\sin\theta|g\rangle+\cos\theta|b\rangle.
$$

The [Boolean phase oracle](../../../quantum-theory.md#marked-state-phase-oracle) negates $|g\rangle$ and fixes $|b\rangle$. The [Grover diffusion operator](../../../quantum-theory.md#grover-diffusion-operator) is $-I_{\psi_0}=2|\psi_0\rangle\langle\psi_0|-I$. Its implementation is independent of $f$: conjugate the reflection about $|0^n\rangle$ by [Hadamard gates](../../../quantum-theory.md#hadamard-gate). One [Grover search algorithm](../../../quantum-theory.md#grover-s-algorithm) iteration is

$$
G=-I_{\psi_0}I_f=\begin{pmatrix}\cos2\theta&\sin2\theta\\-\sin2\theta&\cos2\theta\end{pmatrix}_{g,b}.
$$

Hence, by the [Grover rotation angle](../../../quantum-theory.md#grover-rotation-angle) formula,

$$
G^j|\psi_0\rangle=\sin((2j+1)\theta)|g\rangle+\cos((2j+1)\theta)|b\rangle.
$$

Choose the nonnegative integer $j$ nearest to $\pi/(4\theta)-1/2$. Its final angle differs from $\pi/2$ by at most $\theta$, so a [computational-basis measurement](../../../quantum-theory.md#quantum-measurement-in-the-computational-basis) succeeds with probability at least $\cos^2\theta=1-p$. The allowed small-density regime includes $p\le1/3$, giving the requested $2/3$ bound. Each iteration uses one [Boolean phase oracle](../../../quantum-theory.md#marked-state-phase-oracle) query, and $j=O(1/\sqrt p)=O(\sqrt{N/k})$.

For $k=N/4$, $\theta=\pi/6$ and one iteration reaches $3\theta=\pi/2$ exactly. **Thus one query gives a good outcome with certainty:**

$$
\boxed{G|\psi_0\rangle=|g\rangle\quad(k=N/4).}
$$

This is [exact Grover search on four entries](../../../quantum-theory.md#exact-grover-search-on-four-entries) applied to a marked fraction of one quarter, not only to a four-element register.

<h3 id="2/ii">ii</h3>

↑ **Parent:** [2](#2)

<h4 id="2/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#2/ii)

The [amplitude amplification theorem](../../../quantum-theory.md#amplitude-amplification) concerns a known preparation [quantum circuit](../../../quantum-circuit.md) $A$ and a good-subspace projector $\Pi$. Write $A|0\rangle=\sin\theta|g\rangle+\cos\theta|b\rangle$, with $\sin^2\theta=p=\|\Pi A|0\rangle\|^2$. Let $S_0=I-2|0\rangle\langle0|$ and $S_\chi=I-2\Pi$. Then

$$
Q=-A S_0A^\dagger S_\chi,\qquad\boxed{\|\Pi Q^jA|0\rangle\|^2=\sin^2((2j+1)\theta).}
$$

The [reflection operators](../../../quantum-theory.md#reflection-operator) preserve the two-dimensional good-bad plane and rotate it by $2\theta$, so $O(1/\sqrt p)$ iterations amplify a small known success probability to a constant close to one. Each iteration uses one good-subspace phase test and one use each of $A,A^\dagger$, together with a known reflection. **[Amplitude amplification](../../../quantum-theory.md#amplitude-amplification) provides a quadratic improvement in the number of repetitions of a successful preparation.** The query cost of the preparation and its inverse must be included when they themselves use the input oracle. [Exact amplitude amplification](../../../quantum-theory.md#exact-amplitude-amplification) uses additional known-overlap preparation or phase matching to avoid integer-iteration overshoot.

<h3 id="2/iii">iii</h3>

↑ **Parent:** [2](#2)

<h4 id="2/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#2/iii)

Under the usual reversible-circuit interpretation, there is a genuine [obstruction to uniform probability lowering by a unitary](../../../quantum-theory.md#obstruction-to-uniform-probability-lowering-by-a-unitary) in the printed premise. The universal assertion cannot hold for arbitrary $p$: it fails already at the search density $p=k/N$.

An explicit counterexample uses $N=4$, one good basis state $|0\rangle$, $p=1/4$ and $p'=1/8$. The six pure states

$$
|\psi_{j,\pm}\rangle=\frac12|0\rangle\pm\frac{\sqrt3}{2}|j\rangle,\qquad j=1,2,3,
$$

all have good probability $1/4$. Their equally weighted [density operator](../../../quantum-theory.md#density-matrix) is $I_4/4$, a [maximally mixed state](../../../quantum-theory.md#maximally-mixed-state). Every [unitary operator](../../../vector-space.md#unitary-operator) $C$ leaves this mixture unchanged, so its average output good probability remains $1/4$. The printed assertion would instead make all six output probabilities $1/8$, a contradiction. More generally, averaging states $\sqrt{k/N}|g\rangle+e^{i\alpha}\sqrt{1-k/N}|b\rangle$ uniformly over good and bad basis vectors and two opposite phases gives $I_N/N$, proving the same obstruction at the actual search density $p=k/N$.

The intended conditional construction needs only a supplied reversible preparation that lowers the success probability of the particular starting state, not of every state. Here is the complete argument under that weaker resource assumption. Count $C$ and $C^\dagger$ as supplied, query-free operations, as required for the claimed input-oracle bound. Let $\theta=\arcsin\sqrt{k/N}$ and choose

$$
j=\left\lceil\frac\pi{4\theta}-\frac12\right\rceil,\qquad\theta_* =\frac\pi{4j+2},\qquad p_* =\sin^2\theta_*\le\frac kN.
$$

If equality holds, use the original preparation. Otherwise use the stipulated preparation on $|\psi_0\rangle$ to obtain $|\psi_*\rangle=C|\psi_0\rangle$ with good probability $p_*$. Its [reflection operator](../../../quantum-theory.md#reflection-operator) is implementable by

$$
I_{\psi_*}=C I_{\psi_0}C^\dagger.
$$

The good and bad components may be nonuniform, but [amplitude amplification](../../../quantum-theory.md#amplitude-amplification) applies to this same two-dimensional decomposition. After $j$ iterations of $-I_{\psi_*}I_f$, its good probability is

$$
\boxed{\sin^2((2j+1)\theta_*)=1,\qquad j=O\!\left(\sqrt{N/k}\right).}
$$

Thus **the stated exact-query conclusion follows from accessible preparation of one known-overlap state and its inverse.** If the supplied preparation uses oracle queries, those costs cannot be omitted.

A physically realizable [known-state success dilution for exact amplitude amplification](../../../quantum-theory.md#known-state-success-dilution-for-exact-amplitude-amplification) is available in the standard enlarged marking-oracle model. Append a flag in $\sqrt{1-q}|0\rangle+\sqrt q|1\rangle$, where $q=p_*/p$, and call a joint state good only when $f(x)=1$ and the flag is one. This prepared state's success probability is exactly $pq=p_*$. Reflect about this known product preparation and mark the joint good subspace; $j$ ordinary iterations then succeed with certainty. A supplied controlled phase oracle gives one marking query per iteration, or a Boolean bit oracle computes $f$, applies the joint phase and uncomputes $f$ in two queries. Measuring the data therefore returns a good $x$ with certainty in $O(\sqrt{N/k})$ queries. This changes the state space and marking test, and does not assert the impossible universal $n$-qubit circuit. Controlled access is an additional resource in a bare phase-oracle model, so it is made explicit rather than silently assumed.

## 3

↑ **Parent:** [Paper 58](paper-58.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

This is the [Deutsch-Jozsa test with an arbitrary uniform-state unitary](../../../quantum-theory.md#deutsch-jozsa-test-with-an-arbitrary-uniform-state-unitary), and does not require $N$ to be a power of two. Choose a known [unitary operator](../../../vector-space.md#unitary-operator) $F$ such that $F|0\rangle=|s\rangle=N^{-1/2}\sum_i|i\rangle$. Prepare the target [qubit](../../../quantum-mechanics.md#qubit) in $|{-}\rangle=(|0\rangle-|1\rangle)/\sqrt2$. One Boolean-oracle call gives [quantum phase kickback](../../../quantum-theory.md#phase-kickback):

$$
O_{\mathbf x}|i\rangle|{-}\rangle=(-1)^{x_i}|i\rangle|{-}\rangle.
$$

Apply $F^\dagger$ to the index register. The amplitude on $|0\rangle$ is

$$
\frac1N\sum_i(-1)^{x_i}.
$$

It equals $+1$ or $-1$ for the two constant strings, and equals zero for a balanced string. Consequently **a single query decides the promised problem exactly:** measure the index register and report constant for outcome zero, balanced for any other outcome. This is the [Deutsch-Jozsa algorithm](../../../quantum-theory.md#deutsch-jozsa-algorithm) with the available exact state-preparation operation.

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/i">i</h4>

↑ **Parent:** [B](#3/b)

<h5 id="3/b/i/solution">Solution</h5>

↑ **Parent:** [I](#3/b/i)

Let $|u_i\rangle$ denote the specified image of $|i\rangle|0\rangle$. Its components comprise $N-1$ distinct ordered-pair basis states, each with coefficient $\pm N^{-1/2}$, together with $|0,0\rangle$ with coefficient $N^{-1/2}$. Hence $\langle u_i|u_i\rangle=1$.

For distinct indices $i<j$, only two output basis states occur in both images. Their common $|0,0\rangle$ contributions have product $1/N$, while the $|i,j\rangle$ contributions have product $-1/N$. Thus

$$
\boxed{\langle u_i|u_j\rangle=\delta_{ij}.}
$$

The specified map is therefore a [linear isometry](../../../hilbert-space.md#linear-isometry-of-hilbert-spaces) on the $N$-dimensional input subspace. Complete the input vectors $|i,0\rangle$ to an [orthonormal basis](../../../linear-algebra.md#orthonormal-basis) of the $N^2$-dimensional space, and independently complete their images $|u_i\rangle$ to another [orthonormal basis](../../../linear-algebra.md#orthonormal-basis). Map the first full basis to the second. This is a [unitary extension of a finite-dimensional isometry](../../../hilbert-space.md#unitary-extension-of-a-finite-dimensional-isometry), giving the required $\widetilde U$. **The prescribed columns are orthonormal, so a full [unitary extension](../../../hilbert-space.md#unitary-extension-of-a-finite-dimensional-isometry) exists.** Its construction depends only on $N$, not on the unknown string, and is permitted by the question's exact-unitary assumption.

<h4 id="3/b/ii">ii</h4>

↑ **Parent:** [B](#3/b)

<h5 id="3/b/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#3/b/ii)

Let $w$ be the number of ones. The displayed output state assigns the outcome $(0,0)$ probability

$$
\boxed{\Pr(0,0)=\frac{(N-2w)^2}{N^2}.}
$$

For a constant string, $w=0$ or $N$, so this probability is one. For a balanced string, $w=N/2$, so it is zero. Under the promise, **$(0,0)$ certifies a constant string, and any other possible outcome certifies a balanced string.** A nonzero ordered-pair outcome must have $i<j$ and $\widehat x_i-\widehat x_j\ne0$, which also certifies $x_i\ne x_j$ without separately reading either bit. This is the fact used by [opposite-pair elimination for exact quantum balance testing](../../../quantum-theory.md#opposite-pair-elimination-for-exact-quantum-balance-testing).

<h4 id="3/b/iii">iii</h4>

↑ **Parent:** [B](#3/b)

<h5 id="3/b/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#3/b/iii)

Maintain a known list of the still-active indices, initially all $N=2K$ positions. On a list of even size $M$, perform the three-step construction with $M$ replacing $N$. A known reversible relabeling prepares and queries the corresponding original indices, so [quantum phase kickback](../../../quantum-theory.md#phase-kickback) still needs only one call to $O_{\mathbf x}$. The full [unitary extension](../../../hilbert-space.md#unitary-extension-of-a-finite-dimensional-isometry) for that current size is independent of the remaining unknown values. It is allowed even when $M$ is not a power of two.

If the measurement gives $(0,0)$, its amplitude is the imbalance divided by $M$. A balanced active string has zero such amplitude, so an observed zero pair certifies that the active string is unbalanced. Return unbalanced immediately. No probability-of-error estimate is needed: an impossible outcome never occurs in the balanced case.

Otherwise the measured pair corresponds to two opposite bits. Delete those two indices and repeat. Each deletion removes exactly one zero and one one, preserving the difference between their counts. Thus the active string is balanced if and only if the original one is balanced. If all indices are removed, return balanced. This is [opposite-pair elimination for exact quantum balance testing](../../../quantum-theory.md#opposite-pair-elimination-for-exact-quantum-balance-testing); it never requires determining which member of a deleted pair is zero.

Each query either terminates with a valid imbalance certificate or reduces the active length by two. After at most $K$ opposite-pair outcomes the active list is empty. **The result is certain on every input, with worst-case query count**

$$
\boxed{Q(N)\le N/2=K.}
$$

The same argument includes the $M=2$ last step: equal bits give $(0,0)$ with certainty, while opposite bits give the sole nonzero pair with certainty. There is no additional final query. The measurement probabilities are normalized because $(M-2w)^2+4w(M-w)=M^2$.

## 4

↑ **Parent:** [Paper 58](paper-58.md)

<h3 id="4/a">a</h3>

↑ **Parent:** [4](#4)

<h4 id="4/a/i">i</h4>

↑ **Parent:** [A](#4/a)

<h5 id="4/a/i/solution">Solution</h5>

↑ **Parent:** [I](#4/a/i)

For $n\ge2$, the [Pauli X gate](../../../quantum-theory.md#pauli-x-gate) and [Pauli Z gate](../../../quantum-theory.md#pauli-z-gate) act on different [qubits](../../../quantum-mechanics.md#qubit) in $X_0Z_1$, so they commute. Their product is a [Hermitian matrix](../../../hilbert-space.md#hermitian-operator) and squares to the [identity operator](../../../vector-space.md#identity-operator). Its [eigenvalues](../../../linear-operator-theory.md#eigenvalue) have modulus one; equivalently it is a [unitary operator](../../../vector-space.md#unitary-operator). Therefore **its [spectral norm](../../../continuous-dual-space.md#matrix-2-norm) is**

$$
\boxed{\|X_0Z_1\|=1.}
$$

The $n\ge2$ qualification is necessary because the qubit labelled one does not exist for $n=1$.

<h4 id="4/a/ii">ii</h4>

↑ **Parent:** [A](#4/a)

<h5 id="4/a/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#4/a/ii)

The printed upper summation limit introduces $Z_n$ although only qubits $0,\ldots,n-1$ were defined. Literally the final term is undefined. Use the natural open-chain repair

$$
H_{\rm open}=\sum_{i=1}^{n-1}h_i,\qquad h_i=X_{i-1}Z_i.
$$

This preserves the stated $n$-qubit system and agrees with the supplied sum-of-squares hint. If a cyclic convention $Z_n=Z_0$ was intended instead, it must be stated; the same argument works for its $n$ terms when $n\ge2$. For $n=1$, the repaired open chain is empty and the target is the identity.

Here is a [product-formula Hamiltonian simulation](../../../quantum-theory.md#product-formula-hamiltonian-simulation) using exactly the two supplied lemmas. Let $L=n-1$ and choose an integer $r\ge L$. Every $h_i$ is a norm-one [Hermitian matrix](../../../hilbert-space.md#hermitian-operator). One time slice is the product of [two-qubit gates](../../../quantum-circuit.md#two-qubit-gate)

$$
P_r=e^{ih_1/r}\cdots e^{ih_L/r},\qquad\widetilde U=P_r^r.
$$

To compare a partial product with $e^{i(h_1+\cdots+h_j)/r}$, first propagate the previous error through the next [unitary gate](../../../quantum-circuit.md#quantum-logic-gate), which preserves the [spectral norm](../../../continuous-dual-space.md#matrix-2-norm), and then use Lemma A with $A=-(h_1+\cdots+h_{j-1})/r$, $B=-h_j/r$. Both [norms](../../../functional-analysis.md#norm) are at most $j/r\le1$. Its new error is at most $c(j/r)^2$ for a universal constant $c$. For an explicit choice, $c=4$ follows from the unitary Taylor bounds $\|e^{iA}-I-iA\|\le\|A\|^2/2$ and $\|e^{iA}-I\|\le\|A\|$. Induction and the [triangle inequality](../../../topological-analysis.md#triangle-inequality) therefore give

$$
\|P_r-e^{iH_{\rm open}/r}\|\le\frac c{r^2}\sum_{j=2}^{L}j^2=O\!\left(\frac{L^3}{r^2}\right).
$$

Lemma B, the [unitary product telescoping](../../../continuous-dual-space.md#unitary-product-telescoping) bound, now compares the $r$ repeated slices with $(e^{iH_{\rm open}/r})^r=e^{iH_{\rm open}}$:

$$
\|\widetilde U-e^{iH_{\rm open}}\|\le\frac{c\sum_{j=2}^{L}j^2}{r}.
$$

Take, for example, $r=\max(1,L,\lceil2c\sum_{j=2}^{L}j^2/\epsilon\rceil)$. If the sum is zero the product is already exact; otherwise its error is at most $\epsilon/2<\epsilon$. There are $Lr$ [two-qubit gates](../../../quantum-circuit.md#two-qubit-gate). **This explicit lemma-based construction has fourth-degree dependence on $n$ for fixed precision:**

$$
\boxed{\text{gate count}=O(n^2+n^4/\epsilon),\qquad\|U-\widetilde U\|<\epsilon.}
$$

This is a sufficient polynomial, not an optimality claim. The polynomial-degree statement treats $\epsilon$ as fixed; the inverse-precision dependence is displayed separately. No first-order term error is accumulated without the required repeated-slice factor.

<h3 id="4/b">b</h3>

↑ **Parent:** [4](#4)

<h4 id="4/b/i">i</h4>

↑ **Parent:** [B](#4/b)

<h5 id="4/b/i/solution">Solution</h5>

↑ **Parent:** [I](#4/b/i)

For a [unitary operator](../../../vector-space.md#unitary-operator) $W$, $WW^\dagger=I$. Thus for every nonnegative integer $j$,

$$
(W^\dagger H W)^j=W^\dagger H^jW.
$$

Insert this into the convergent [matrix exponential](../../../linear-operator-theory.md#matrix-exponential) series in the finite-dimensional qubit setting:

$$
W^\dagger e^{iH}W=\sum_{j=0}^\infty\frac{i^j}{j!}W^\dagger H^jW=\sum_{j=0}^\infty\frac{i^j}{j!}(W^\dagger HW)^j.
$$

**Consequently unitary conjugation commutes with the exponential:**

$$
\boxed{W^\dagger e^{iH}W=e^{iW^\dagger HW}.}
$$

For an unbounded self-adjoint [Hamiltonian](../../../classical-mechanics.md#hamiltonian), the same identity follows from the [spectral theorem for normal operators](../../../hilbert-space.md#spectral-theorem-for-normal-operators), with the domain transported by $W$; no unbounded power-series manipulation is needed.

<h4 id="4/b/ii">ii</h4>

↑ **Parent:** [B](#4/b)

<h5 id="4/b/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#4/b/ii)

Use one target [ancilla qubit](../../../quantum-information-theory.md#ancilla-qubit) initially in $|0\rangle$. Apply a [CNOT gate](../../../quantum-theory.md#controlled-not-gate) from each data [qubit](../../../quantum-mechanics.md#qubit) $x_j$ to that same target, for $j=1,\ldots,n$. Each [CNOT gate](../../../quantum-theory.md#controlled-not-gate) adds its control bit modulo two without changing the control. After all $n$ gates the target contains the [parity bit](../../../coding-theory.md#parity-bit) $f(x)=x_1\oplus\cdots\oplus x_n$. Thus **the required circuit is the $n$-gate parity fan-in:**

$$
\boxed{W=\prod_{j=1}^{n}\operatorname{CNOT}_{j\to a},\qquad W|x\rangle|0\rangle=|x\rangle|f(x)\rangle.}
$$

This is [parity computation by CNOT gates](../../../coding-theory.md#parity-computation-by-cnot-gates). The circuit also satisfies $W|x\rangle|y\rangle=|x\rangle|y\oplus f(x)\rangle$ for either target value, and $W^{-1}=W$ because all these shared-target [CNOT gates](../../../quantum-theory.md#controlled-not-gate) commute and individually square to the identity. The action on general superpositions follows by [linearity](../../../vector-space.md#linearity).

<h4 id="4/b/iii">iii</h4>

↑ **Parent:** [B](#4/b)

<h5 id="4/b/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#4/b/iii)

The product of the data [Pauli Z gates](../../../quantum-theory.md#pauli-z-gate) has computational-basis [eigenvalue](../../../linear-operator-theory.md#eigenvalue)

$$
(Z^{\otimes n})|x\rangle=(-1)^{x_1+\cdots+x_n}|x\rangle=(-1)^{f(x)}|x\rangle.
$$

Use the parity circuit $W$ from part (ii), apply the target [unitary gate](../../../quantum-circuit.md#quantum-logic-gate) $R=e^{itZ}=\operatorname{diag}(e^{it},e^{-it})$, and then uncompute the parity with $W^\dagger$. For every basis input,

$$
W^\dagger(I\otimes e^{itZ})W|x\rangle|0\rangle=e^{it(-1)^{f(x)}}|x\rangle|0\rangle.
$$

This equals $e^{itZ^{\otimes n}}$ on the data, with the [ancilla qubit](../../../quantum-information-theory.md#ancilla-qubit) returned to zero. The [compute-phase-uncompute construction](../../../quantum-theory.md#compute-phase-uncompute-construction) therefore gives **an exact linear-size circuit:**

$$
\boxed{V=e^{itZ^{\otimes n}}:\quad n\ \mathrm{CNOTs},\ e^{itZ}\ \text{on the ancilla},\ n\ \mathrm{CNOTs};\qquad 2n+1\text{ gates}.}
$$

This is a [Pauli-string phase by parity computation](../../../quantum-theory.md#pauli-string-phase-by-parity-computation), an instance of [simulation of a computable diagonal Hamiltonian](../../../quantum-theory.md#simulation-of-a-computable-diagonal-hamiltonian). Part (i) also explains it by $W^\dagger(I\otimes Z)W=Z^{\otimes n}\otimes Z$, whose exponential restricts correctly to the target-$|0\rangle$ subspace. If no extra line is desired, accumulate parity into the last data [qubit](../../../quantum-mechanics.md#qubit), apply $e^{itZ}$ there, and undo the $n-1$ [CNOT gates](../../../quantum-theory.md#controlled-not-gate), for $2n-1$ gates. Both constructions implement the global phase as well as the relative phases exactly.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2013](../../2013.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
