# Paper 324

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2016/paper_324.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2016/paper_324.pdf)

**Table of contents**

- [1](#1)
  - [i](#1/i)
    - [Solution](#1/i/solution)
  - [ii](#1/ii)
    - [Solution](#1/ii/solution)
  - [iii](#1/iii)
    - [Solution](#1/iii/solution)
- [2](#2)
  - [a](#2/a)
    - [Solution](#2/a/solution)
  - [b](#2/b)
    - [Solution](#2/b/solution)
  - [c](#2/c)
    - [Solution](#2/c/solution)
- [3](#3)
  - [i](#3/i)
    - [Solution](#3/i/solution)
  - [ii](#3/ii)
    - [Solution](#3/ii/solution)
  - [iii](#3/iii)
    - [Solution](#3/iii/solution)
  - [iv](#3/iv)
    - [Solution](#3/iv/solution)
- [4](#4)
  - [i](#4/i)
    - [Solution](#4/i/solution)
  - [ii](#4/ii)
    - [Solution](#4/ii/solution)

## 1

↑ **Parent:** [Paper 324](paper-324.md)

<h3 id="1/i">i</h3>

↑ **Parent:** [1](#1)

<h4 id="1/i/solution">Solution</h4>

↑ **Parent:** [I](#1/i)

For [coprime integers](../../../number-theory.md#coprime-integers) $\alpha,N$, the [multiplicative order](../../../number-theory.md#multiplicative-order) is the smallest positive exponent

$$
\boxed{r=\operatorname{ord}_N(\alpha)=\min\{k\geq1:\alpha^k\equiv1\pmod N\}.}
$$

It exists because multiplication by $\alpha$ is an element of the finite [group of units modulo an integer](../../../algebra.md#multiplicative-group-of-integers-modulo-n). For the example, the successive residues are

$$
7^1\equiv7,\quad7^2\equiv4,\quad7^3\equiv13,\quad7^4\equiv1\pmod{15}.
$$

None of the first three is one, so **the order is four**.

The [factor extraction from an even modular order](../../../quantum-theory.md#factor-extraction-from-an-even-modular-order) uses the factorization $\alpha^r-1=(\alpha^{r/2}-1)(\alpha^{r/2}+1)$. If the [multiplicative order](../../../number-theory.md#multiplicative-order) $r$ is even, put $z=\alpha^{r/2}\bmod N$. Minimality of the [multiplicative order](../../../number-theory.md#multiplicative-order) excludes $z=1$; we also require $z\neq-1\pmod N$. Thus $z^2\equiv1\pmod N$ is a nontrivial square root of one. Neither $z-1$ nor $z+1$ is divisible by all of $N$. If either were coprime to $N$, its inverse modulo $N$, applied to $(z-1)(z+1)\equiv0$, would make the other divisible by $N$, a contradiction. Hence the [greatest common divisors](../../../number-theory.md#greatest-common-divisor)

$$
\boxed{d_-=\gcd(z-1,N),\qquad d_+=\gcd(z+1,N)}
$$

are proper nontrivial factors. For odd $N$, $(z-1)$ and $(z+1)$ have no common prime divisor of $N$, so these two divisors are complementary. If the initial $\alpha$ is not coprime to $N$, a proper $\gcd(\alpha,N)$ already supplies a factor without [quantum order finding](../../../quantum-theory.md#quantum-order-finding).

For $N=15$ and $\alpha=7$, $r=4$ and $z=7^2\bmod15=4$, which is neither $1$ nor $14$. **The factors are**

$$
\boxed{\gcd(4-1,15)=3,\qquad\gcd(4+1,15)=5.}
$$

The necessary conditions for this order-based reduction are a unit $\alpha\bmod N$, even true [multiplicative order](../../../number-theory.md#multiplicative-order), and $\alpha^{r/2}\not\equiv-1\pmod N$.

<h3 id="1/ii">ii</h3>

↑ **Parent:** [1](#1)

<h4 id="1/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#1/ii)

Let $L=\lceil\log_2N\rceil$. In the [Shor algorithm](../../../quantum-theory.md#shor-s-algorithm), first use classical arithmetic to deal with even $N$ and perfect powers, and to reject prime inputs. Perfect-power recognition and primality testing have polynomial-time classical algorithms. Factoring a perfect power $b^k$, with $b,k>1$, already gives a nontrivial factor $b$. We may therefore consider an odd composite $N$ with at least two distinct prime factors.

Choose $\alpha$ uniformly from $1<\alpha<N$ and compute its [greatest common divisor](../../../number-theory.md#greatest-common-divisor) with $N$ using the [Euclidean algorithm](../../../number-theory.md#euclidean-algorithm). A proper nontrivial divisor ends the computation. Otherwise $\alpha$ is a unit, and the remaining task is [quantum order finding](../../../quantum-theory.md#quantum-order-finding). Set

$$
N^2\leq Q=2^t<2N^2.
$$

Prepare a [uniform quantum superposition](../../../quantum-theory.md#uniform-quantum-superposition) in a $t$-[qubit](../../../quantum-mechanics.md#qubit) register and use [quantum modular exponentiation](../../../quantum-theory.md#quantum-modular-exponentiation) in a second register to obtain

$$
\frac1{\sqrt Q}\sum_{x=0}^{Q-1}|x\rangle|\alpha^x\bmod N\rangle.
$$

Repeated squaring and reversible modular multiplication implement this step with polynomially many [quantum gates](../../../quantum-circuit.md#quantum-logic-gate) in $L$. Apply the inverse [quantum Fourier transform](../../../quantum-theory.md#quantum-fourier-transform) to the first register and perform a [quantum measurement in the computational basis](../../../quantum-theory.md#quantum-measurement-in-the-computational-basis), obtaining $j$. Measuring the second register first, and Fourier-transforming the resulting periodic coset, gives the same distribution of $j$.

Here is a quantitative [quantum Fourier sampling bound for order finding](../../../quantum-theory.md#quantum-fourier-sampling-bound-for-order-finding). If $r=\operatorname{ord}_N(\alpha)$, multiplication by $\alpha$ cycles its $r$ orbit states. The Fourier eigenstates of that cycle have eigenvalues $e^{2\pi i s/r}$, and the initial state $|1\rangle$ has squared overlap $1/r$ with each, for $0\leq s<r$. Therefore

$$
\Pr(j)=\frac1r\sum_{s=0}^{r-1}\left|\frac1Q\sum_{x=0}^{Q-1}e^{2\pi i x(s/r-j/Q)}\right|^2.
$$

Conditioned on a particular eigenphase $s/r$, its nearest integer outcome $j_s$ obeys $|j_s/Q-s/r|\leq1/(2Q)$ and has probability at least $4/\pi^2$. Indeed the absolute amplitude is $|\sin(\pi Q\delta)/(Q\sin(\pi\delta))|$, where $\delta=s/r-j_s/Q$. For $|Q\delta|\leq1/2$, the numerator is at least $2Q|\delta|$ and the denominator at most $\pi Q|\delta|$; the limiting value at $\delta=0$ is one.

If $\gcd(s,r)=1$, the fraction $s/r$ is reduced, and $r<N$ gives

$$
\left|\frac{j_s}{Q}-\frac sr\right|\leq\frac1{2Q}<\frac1{2r^2}.
$$

Use [continued-fraction recovery in quantum order finding](../../../quantum-theory.md#continued-fraction-recovery-in-quantum-order-finding). The relevant approximation theorem says that reduced fractions satisfying $|a/b-p/q|<1/(2q^2)$ are [continued fraction convergents](../../../number-theory.md#continued-fraction-convergent) of $a/b$. For an input rational of $O(L)$ digits, their $O(L)$ candidates can be enumerated classically in $O(L^3)$ time, and their denominators are at most the reduced input denominator. This is the supplied continued-fraction result; discard candidate denominators exceeding $N$. A zero measurement is treated as a failed order-finding sample.

For each remaining even candidate denominator $q$, compute $z=\alpha^{q/2}\bmod N$ by [repeated squaring](../../../number-theory.md#exponentiation-by-squaring), and try $\gcd(z-1,N)$ and $\gcd(z+1,N)$. Return only a divisor $d$ with $1<d<N$; otherwise repeat the quantum sample or choose another $\alpha$. This [candidate-denominator gcd post-processing](../../../quantum-theory.md#candidate-denominator-gcd-post-processing) cannot return an incorrect factor, since its output is checked directly. When the recovered denominator is the true even [multiplicative order](../../../number-theory.md#multiplicative-order) and the square root of one is nontrivial, part (i) guarantees success. Checking $\alpha^q\equiv1\pmod N$ before trying the gcds is also a valid, more restrictive convention; the single-run distinction matters in part (iii).

Two further standard quantitative facts explain why repetitions remain efficient. First, for a uniformly chosen unit modulo an odd integer with at least two distinct prime divisors, the [probability of a useful unit in Shor factorization](../../../quantum-theory.md#probability-of-a-useful-unit-in-shor-factorization) is at least $1/2$: its true [multiplicative order](../../../number-theory.md#multiplicative-order) is even and $\alpha^{r/2}\not\equiv-1\pmod N$. To see the source of this bound, the [Chinese remainder theorem for unit groups](../../../mathematics.md#chinese-remainder-theorem-for-unit-groups) makes the prime-power components independent. Each odd-prime-power unit group is cyclic. If its 2-primary order is $2^v$, the probability of the largest possible value of $v$ is $1/2$, and the probability of any specified smaller value is at most $1/2$. Failure requires all components to have the same $v$: either all zero, making $r$ odd, or all the same positive value, making the halfway power $-1$ in every component. Conditioning on one component, the chance another component matches it is at most $1/2$, so total failure is at most $1/2$.

Second, the fraction of phase numerators coprime to $r$ is $\varphi(r)/r$, where $\varphi$ is the [Euler totient function](../../../number-theory.md#euler-totient-function). The [elementary totient-ratio lower bound](../../../number-theory.md#elementary-totient-ratio-lower-bound) suffices: if the distinct prime divisors are $p_1<\cdots<p_k$, then $p_j\geq j+1$ and $k\leq\log_2r$. The totient product formula therefore gives

$$
\frac{\varphi(r)}r=\prod_{j=1}^k\left(1-\frac1{p_j}\right)
\geq\prod_{j=1}^k\frac j{j+1}=\frac1{k+1}\geq\frac1{1+\log_2r}.
$$

Thus for a good $\alpha$, the probability of sampling a coprime phase numerator with the required accuracy is at least $(4/\pi^2)\varphi(r)/r$. This is inverse-polynomial in the input length, so polynomially many repetitions achieve any fixed success probability. The [quantum Fourier transform](../../../quantum-theory.md#quantum-fourier-transform) uses $O(t^2)$ elementary rotations and [Hadamard gates](../../../quantum-theory.md#hadamard-gate) in the ideal gate description, and the other quantum and classical stages are polynomial in $L$.

**The reduction is therefore polynomial in the bit length**:

$$
\boxed{\text{quantum order finding}\ \longrightarrow\ \text{continued-fraction candidates}\ \longrightarrow\ \text{verified nontrivial gcd factor}.}
$$

A small denominator need not itself be the true [multiplicative order](../../../number-theory.md#multiplicative-order); verification of the final factor is essential, and no guarantee is claimed for every individual sample.

<h3 id="1/iii">iii</h3>

↑ **Parent:** [1](#1)

<h4 id="1/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#1/iii)

Here the true [multiplicative order](../../../number-theory.md#multiplicative-order) is four, and it divides every power-of-two Fourier-register size $Q\geq4$, including the $Q=256$ choice from part (ii). A second-register measurement produces one of the four periodic cosets

$$
\sqrt{\frac4Q}\sum_{k=0}^{Q/4-1}|x_0+4k\rangle.
$$

Its [quantum Fourier transform](../../../quantum-theory.md#quantum-fourier-transform) has nonzero amplitudes only at $j=0,Q/4,Q/2,3Q/4$, and each has squared modulus $1/4$. The inverse transform only changes phases or permutes these four labels. Hence the measured ratios $0,1/4,1/2,3/4$ are equally likely.

For $1/4$ or $3/4$, [continued-fraction recovery in quantum order finding](../../../quantum-theory.md#continued-fraction-recovery-in-quantum-order-finding) returns denominator four. Part (i) then gives factors three and five. For $1/2$, the reduced denominator is two. Although two is not a period, the [candidate-denominator gcd post-processing](../../../quantum-theory.md#candidate-denominator-gcd-post-processing) in part (ii) still gives a factor:

$$
z=7^{2/2}=7,\qquad\gcd(7-1,15)=3,\quad\gcd(7+1,15)=1.
$$

The zero outcome produces no useful even candidate and the run fails. **For the factor-extraction procedure specified above, three of the four outcomes succeed**:

$$
\boxed{\Pr(\text{nontrivial factor in one run})=\frac34.}
$$

There is an important convention behind this answer. A version that rejects a candidate unless $7^q\equiv1\pmod{15}$ before attempting any gcd rejects $q=2$, since $7^2\equiv4$. Under that validated-period convention only the two odd-numerator phases succeed, giving

$$
\boxed{\Pr(\text{one-run success with a prior period check})=\frac12.}
$$

Thus the probability of recovering the true [multiplicative order](../../../number-theory.md#multiplicative-order) is $1/2$, whereas the probability of finding a factor with direct gcd post-processing is $3/4$. The printed question does not specify this classical post-processing detail; stating it avoids identifying these two different events.

## 2

↑ **Parent:** [Paper 324](paper-324.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

Take $|\psi\rangle$ to be normalized and let $\Pi_{\mathcal G}$ be the [orthogonal projection](../../../hilbert-space.md#orthogonal-projection) onto the good subspace. The two [reflection operators](../../../quantum-theory.md#reflection-operator) are

$$
\boxed{I_\psi=I-2|\psi\rangle\langle\psi|,\qquad I_{\mathcal G}=I-2\Pi_{\mathcal G}.}
$$

The first fixes the hyperplane orthogonal to $|\psi\rangle$ and negates its normal direction. The second fixes $\mathcal G^\perp$ and negates $\mathcal G$. Both are [Hermitian operators](../../../hilbert-space.md#hermitian-operator) and [unitary operators](../../../vector-space.md#unitary-operator), since their defining projectors square to themselves. For a non-normalized nonzero vector, divide $|\psi\rangle\langle\psi|$ by $\langle\psi|\psi\rangle$.

Put $p=\langle\psi|\Pi_{\mathcal G}|\psi\rangle=\sin^2\theta$, with $0<\theta<\pi/2$, and define normalized orthogonal good and bad vectors

$$
|g\rangle=\frac{\Pi_{\mathcal G}|\psi\rangle}{\sqrt p},\qquad
|b\rangle=\frac{(I-\Pi_{\mathcal G})|\psi\rangle}{\sqrt{1-p}}.
$$

Then $|\psi\rangle=\sin\theta|g\rangle+\cos\theta|b\rangle$. **The [amplitude amplification theorem](../../../quantum-theory.md#amplitude-amplification) states** that the iterate $Q=-I_\psi I_{\mathcal G}$ satisfies, for every nonnegative integer $m$,

$$
\boxed{Q^m|\psi\rangle=\sin((2m+1)\theta)|g\rangle+\cos((2m+1)\theta)|b\rangle,\qquad
p_m=\sin^2((2m+1)\theta).}
$$

To prove it, the span of $|g\rangle,|b\rangle$ is invariant under both [reflection operators](../../../quantum-theory.md#reflection-operator). In that ordered orthonormal basis,

$$
I_{\mathcal G}=\begin{pmatrix}-1&0\\0&1\end{pmatrix},\qquad
Q=\begin{pmatrix}\cos2\theta&\sin2\theta\\-\sin2\theta&\cos2\theta\end{pmatrix}.
$$

Multiplying the second matrix into $(\sin\theta,\cos\theta)^T$ advances the angle by $2\theta$. Induction proves the formula, and projecting onto $\mathcal G$ gives $p_m$. The minus sign in $Q$ is just a global phase choice, but it makes the displayed state formula exact.

If $p$ is known, choose $m$ nearest to $\pi/(4\theta)-1/2$, with $m\geq0$. The final angle is within $\theta$ of $\pi/2$, so $p_m\geq\cos^2\theta=1-p$. For $p\leq1/2$, this is at least $1/2$ after $O(1/\sqrt p)$ iterations, and is close to one when $p$ is small. For $p>1/2$, measuring the initial state already has success above $1/2$. Repeated independent attempts with a success test give any fixed desired success probability. This is the quadratic improvement of [amplitude amplification](../../../quantum-theory.md#amplitude-amplification) over repeated sampling, which takes $O(1/p)$ attempts. At $p=0$ there is no good component to amplify, and at $p=1$ the initial state is already entirely good; these endpoint cases do not require the undefined normalized component vectors.

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/solution">Solution</h4>

↑ **Parent:** [B](#2/b)

Prepare an ancillary [qubit](../../../quantum-mechanics.md#qubit) in

$$
|-\rangle=\frac{|0\rangle-|1\rangle}{\sqrt2},\qquad X|-\rangle=-|-\rangle.
$$

It can be prepared from $|0\rangle$ by an $X$ operation followed by a [Hadamard gate](../../../quantum-theory.md#hadamard-gate), independently of $g$. One call to the [Boolean quantum oracle](../../../quantum-theory.md#boolean-quantum-oracle) then gives [quantum phase kickback](../../../quantum-theory.md#phase-kickback):

$$
U_g|x\rangle|-\rangle=(-1)^{g(x)}|x\rangle|-\rangle.
$$

The data state receives a minus sign precisely on the basis vectors spanning $\mathcal G$, while the ancilla remains unchanged and unentangled. **One oracle call realizes the reflection**. By linearity it is the [marked-state phase oracle](../../../quantum-theory.md#marked-state-phase-oracle)

$$
\boxed{I_{\mathcal G}=\sum_x(-1)^{g(x)}|x\rangle\langle x|=I-2\Pi_{\mathcal G}}
$$

with one oracle call. The ancillary preparation and its optional inverse use only fixed operations, so no additional knowledge of $g$ is needed.

<h3 id="2/c">c</h3>

↑ **Parent:** [2](#2)

<h4 id="2/c/solution">Solution</h4>

↑ **Parent:** [C](#2/c)

Follow the printed examples by counting positive squares, so zero is not marked. For $N\geq2$, the marked output set is

$$
S=\{k^2:1\leq k\leq\lfloor\sqrt{N-1}\rfloor\},\qquad K=|S|=\lfloor\sqrt{N-1}\rfloor.
$$

A one-to-one map from the finite set $[N]$ to itself is a [permutation](../../../combinatorics.md#permutation), so exactly $K$ inputs have outputs in $S$. In the [uniform quantum superposition](../../../quantum-theory.md#uniform-quantum-superposition) $|s\rangle=N^{-1/2}\sum_x|x\rangle$, the initial good probability is therefore $p=K/N$. For [permutation-preimage quantum search](../../../quantum-theory.md#permutation-preimage-quantum-search), this known [marked density under a permutation](../../../quantum-theory.md#marked-density-under-a-permutation) is $\Theta(N^{-1/2})$.

Define the efficiently computable predicate $h(y)$ to be one if and only if $y$ is a positive square. The assumed [Boolean quantum oracle](../../../quantum-theory.md#boolean-quantum-oracle) for $h$, acting on $y$ and a $|-\rangle$ ancilla, implements its diagonal sign operation $D_h|y\rangle=(-1)^{h(y)}|y\rangle$. Compute the [modular-addition quantum oracle](../../../quantum-theory.md#modular-addition-quantum-oracle) into a zero output register, apply this sign operation, and uncompute:

$$
|x\rangle|0\rangle\xrightarrow{U_f}|x\rangle|f(x)\rangle
\xrightarrow{D_h}(-1)^{h(f(x))}|x\rangle|f(x)\rangle
\xrightarrow{U_f^\dagger}(-1)^{h(f(x))}|x\rangle|0\rangle.
$$

This implements $I_{\mathcal G}$ for $\mathcal G=\operatorname{span}\{|x\rangle:f(x)\in S\}$, with the work registers clean. Only forward calls to $U_f$ were promised, but its inverse costs one such call: if $J|y\rangle=|-y\bmod N\rangle$ on the second register, then

$$
\boxed{U_f^\dagger=(I\otimes J)U_f(I\otimes J).}
$$

Indeed the output addition is changed into subtraction. Thus each marked reflection costs exactly two queries to $U_f$; all other operations used here are independent of the unknown $f$.

Use the [amplitude amplification theorem](../../../quantum-theory.md#amplitude-amplification) with $|\psi\rangle=|s\rangle$, whose reflection is allowed by the assumptions. With $\theta=\arcsin\sqrt{K/N}$, choose $m$ nearest to $\pi/(4\theta)-1/2$. Here $p\leq1/2$ for every $N\geq2$, so a trial succeeds with probability at least $1/2$. Also

$$
m=O(\sqrt{N/K})=O(N^{1/4}).
$$

Measure $x$ and use one additional $U_f$ query to evaluate and check $f(x)$. On failure, restart with fresh registers. Four independent trials have failure probability at most $2^{-4}$, so **the required confidence and query bound are**

$$
\boxed{\Pr(\text{success})\geq\frac{15}{16}>0.9,\qquad
\#U_f\text{ queries}\leq4(2m+1)=O(N^{1/4}).}
$$

This is an upper bound on [quantum query complexity](../../../computer-science.md#quantum-query-complexity), not a claim that arbitrary reflections or every classical gate have constant cost. Including zero as a square would change $K$ to $K+1$ without changing the asymptotic bound. With the printed positive-square interpretation, $N=1$ has no valid output and no algorithm can satisfy the success requirement; the intended asymptotic task necessarily has $N\geq2$.

## 3

↑ **Parent:** [Paper 324](paper-324.md)

<h3 id="3/i">i</h3>

↑ **Parent:** [3](#3)

<h4 id="3/i/solution">Solution</h4>

↑ **Parent:** [I](#3/i)

Store a tensor-product element of the [Pauli group](../../../quantum-circuit.md#pauli-group) as

$$
P=i^s\bigotimes_{j=1}^nX^{a_j}Z^{b_j},\qquad s\in\mathbb Z/4\mathbb Z,\quad a_j,b_j\in\{0,1\}.
$$

The phases of the original single-[qubit](../../../quantum-mechanics.md#qubit) factors can all be accumulated into $i^s$. This [binary phase representation of a Pauli string](../../../quantum-circuit.md#binary-phase-representation-of-a-pauli-string) uses $2n+2$ bits. It retains phases, which must not be dropped when computing probabilities later.

For the conjugation convention $U^\dagger P U$ in the question, direct multiplication of the two-by-two matrices gives

$$
H^\dagger XH=Z,\quad H^\dagger ZH=X,\quad H^\dagger XZH=-XZ,
$$

and

$$
S^\dagger XS=-iXZ,\quad S^\dagger ZS=Z,\quad S^\dagger XZS=-iX.
$$

These [backward Pauli updates for Hadamard and phase gates](../../../quantum-circuit.md#backward-pauli-updates-for-hadamard-and-phase-gates) use $S^\dagger P S$, not $SPS^\dagger$. On the affected line $j$, the updates are

$$
\begin{aligned}
H_j:&\quad(a_j,b_j)\mapsto(b_j,a_j),\quad s\mapsto s+2a_jb_j,\\
S_j:&\quad(a_j,b_j)\mapsto(a_j,b_j\oplus a_j),\quad s\mapsto s-a_j.
\end{aligned}
$$

All phases are reduced modulo four and the updates use the old bits.

For a [Controlled-Z gate](../../../quantum-theory.md#controlled-z-gate) on lines $j,k$, its diagonal action gives

$$
CZ\,X_j\,CZ=X_jZ_k,\quad CZ\,X_k\,CZ=Z_jX_k,\quad
CZ\,Z_j\,CZ=Z_j,\quad CZ\,Z_k\,CZ=Z_k.
$$

For the [controlled-Z update in the binary phase representation](../../../quantum-circuit.md#controlled-z-update-in-the-binary-phase-representation), conjugation respects products, so these determine the rule for every [Pauli operator](../../../quantum-circuit.md#pauli-operator) on those lines. In the chosen ordered $XZ$ convention it is

$$
\boxed{b_j\mapsto b_j\oplus a_k,\quad b_k\mapsto b_k\oplus a_j,\quad
s\mapsto s+2a_ja_k,\quad a_j,a_k\text{ unchanged}.}
$$

The phase arises when a newly introduced $Z_k$ is moved past $X_k$. For instance $X_jX_k$ becomes $-X_jZ_jX_kZ_k$, so this sign matters.

The untouched factors are unchanged. Each [Clifford operation](../../../quantum-circuit.md#clifford-gate) therefore needs only a fixed number of local bit updates; reconstructing the requested full list takes $O(n)$ time. Put the final phase into the first factor, which is permitted because the single-[qubit](../../../quantum-mechanics.md#qubit) [Pauli group](../../../quantum-circuit.md#pauli-group) includes all multiples by $\pm1,\pm i$. **The classical cost is polynomial**, despite the exponentially large matrix of the operation on the full state space.

<h3 id="3/ii">ii</h3>

↑ **Parent:** [3](#3)

<h4 id="3/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#3/ii)

The computational-basis projectors on the first [qubit](../../../quantum-mechanics.md#qubit) are

$$
\Pi_0=|0\rangle\langle0|\otimes I^{\otimes(n-1)},\qquad
\Pi_1=|1\rangle\langle1|\otimes I^{\otimes(n-1)}.
$$

The [Pauli Z gate](../../../quantum-theory.md#pauli-z-gate) acts as $+1$ on the first subspace and $-1$ on the second, so $Z_1=\Pi_0-\Pi_1$. By the [Born rule](../../../quantum-mechanics.md#born-rule), $p_b=\langle\psi|\Pi_b|\psi\rangle$. Therefore **the expectation determines the output probabilities**:

$$
\boxed{\langle\psi|Z_1|\psi\rangle=p_0-p_1,\qquad
p_0=\frac{1+\langle Z_1\rangle}{2},\quad p_1=\frac{1-\langle Z_1\rangle}{2}.}
$$

The normalization supplies $p_0+p_1=1$; no product-state assumption is needed for this identity.

<h3 id="3/iii">iii</h3>

↑ **Parent:** [3](#3)

<h4 id="3/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#3/iii)

Write $|a\rangle=\bigotimes_j|a_j\rangle$. Instead of storing the output vector, use [Heisenberg propagation of a Pauli observable through a Clifford circuit](../../../quantum-circuit.md#heisenberg-propagation-of-a-pauli-observable-through-a-clifford-circuit):

$$
\langle Z_1\rangle_{\rm out}=\langle a|C^\dagger Z_1C|a\rangle.
$$

Initialize the compact [Pauli group](../../../quantum-circuit.md#pauli-group) representation at $Z_1$ and conjugate successively by $U_N,U_{N-1},\ldots,U_1$, in that order, using $P\mapsto U_j^\dagger P U_j$. This gives

$$
P=C^\dagger Z_1C=U_1^\dagger\cdots U_N^\dagger Z_1U_N\cdots U_1
$$

with $O(N+n)$ local-update work and $O(n)$ storage. The resulting [Pauli operator](../../../quantum-circuit.md#pauli-operator) is Hermitian, so we can express it as $P=\eta\bigotimes_j\sigma_j$, where $\eta\in\{+1,-1\}$ and each $\sigma_j$ is $I,X,Y$ or $Z$. Any factors $XZ$ in the representation from part (i) are converted using $XZ=-iY$, with their phases absorbed into $\eta$.

The [product state](../../../bell-state.md#product-state) input now makes the expectation factorize:

$$
\boxed{e=\langle a|P|a\rangle=\eta\prod_{j=1}^n\langle a_j|\sigma_j|a_j\rangle,\qquad
p_0=\frac{1+e}{2},\quad p_1=\frac{1-e}{2}.}
$$

Each factor is a two-by-two matrix calculation. More explicitly, for $|a_j\rangle=\alpha_j|0\rangle+\beta_j|1\rangle$, the three nontrivial expectations are $2\operatorname{Re}(\overline\alpha_j\beta_j)$, $2\operatorname{Im}(\overline\alpha_j\beta_j)$, and $|\alpha_j|^2-|\beta_j|^2$ for $X,Y,Z$, respectively.

Thus **this single-output process has a [strong classical simulation](../../../quantum-circuit.md#strong-classical-simulation-of-a-quantum-circuit) in [polynomial time](../../../computer-science.md#polynomial-time)**, even when the individual input states are not stabilizer states. As usual, the given state identities must provide efficiently computable amplitudes. With finite-precision inputs, each factor can be evaluated to error $\delta/n$ and its approximation clipped to $[-1,1]$ to obtain the final expectation to error at most $\delta$, because all factors lie in $[-1,1]$. The required extra precision is only $O(\log(n/\delta))$ bits. Exact evaluation applies when the input descriptions support exact arithmetic. This avoids silently assigning a finite exact-computation cost to arbitrary unspecified real numbers.

Once the probabilities are known, a classical randomized computation can reproduce this measured bit. The argument concerns the specified one-[qubit](../../../quantum-mechanics.md#qubit) output; it does not assert that every joint measurement distribution for arbitrary product inputs can be simulated by this same single-observable calculation.

<h3 id="3/iv">iv</h3>

↑ **Parent:** [3](#3)

<h4 id="3/iv/solution">Solution</h4>

↑ **Parent:** [Iv](#3/iv)

Use [GHZ preparation with Hadamard and controlled-Z gates](../../../quantum-theory.md#ghz-preparation-with-hadamard-and-controlled-z-gates) for $n\geq2$. Apply a [Hadamard gate](../../../quantum-theory.md#hadamard-gate) to the first [qubit](../../../quantum-mechanics.md#qubit), then a [controlled-NOT gate](../../../quantum-theory.md#controlled-not-gate) from that [qubit](../../../quantum-mechanics.md#qubit) to each of the other $n-1$ [qubits](../../../quantum-mechanics.md#qubit). Every controlled-NOT can be written in the allowed gate set as

$$
\operatorname{CNOT}_{1\to j}=H_j\,CZ_{1j}\,H_j.
$$

Indeed conjugating the target $Z$ by $H$ makes the controlled phase into a controlled $X$. The rightmost gate acts first. Consequently the [Clifford circuit](../../../quantum-circuit.md#clifford-circuit) uses $1+3(n-1)$ allowed gates and gives

$$
\boxed{|\psi\rangle=\frac{|0\rangle^{\otimes n}+|1\rangle^{\otimes n}}{\sqrt2}.}
$$

For every chosen [qubit](../../../quantum-mechanics.md#qubit) $j$, tracing out the other [qubits](../../../quantum-mechanics.md#qubit) yields $\rho_j=\tfrac12(|0\rangle\langle0|+|1\rangle\langle1|)=I/2$. Equivalently, across that [qubit](../../../quantum-mechanics.md#qubit) versus the rest, the displayed state is a [Schmidt decomposition](../../../von-neumann-entropy.md#schmidt-decomposition) with two nonzero coefficients $1/\sqrt2$. It is therefore [entangled](../../../bell-state.md#entangled-state) across every such bipartition.

**[Entanglement](../../../bell-state.md#entangled-state) does not prevent the polynomial single-output simulation from part (iii).** The simulation follows the measured observable rather than claiming that the intermediate states remain [product states](../../../bell-state.md#product-state). When $n=1$, there is no remaining subsystem and the requested [entanglement](../../../bell-state.md#entangled-state) is impossible; the construction and claim require $n\geq2$.

## 4

↑ **Parent:** [Paper 324](paper-324.md)

<h3 id="4/i">i</h3>

↑ **Parent:** [4](#4)

<h4 id="4/i/solution">Solution</h4>

↑ **Parent:** [I](#4/i)

**The [spectral norm](../../../continuous-dual-space.md#matrix-2-norm) is the induced Euclidean [operator norm](../../../continuous-dual-space.md#operator-norm)**:

$$
\boxed{\|A\|=\sup_{\|v\|_2=1}\|Av\|_2
=\sqrt{\lambda_{\max}(A^\dagger A)}.}
$$

It is the largest [singular value](../../../linear-algebra.md#singular-value). From the definition, multiplying on either side by a [unitary operator](../../../vector-space.md#unitary-operator) leaves the norm unchanged: right multiplication permutes the unit sphere of possible inputs, and left multiplication preserves output lengths. In particular every [unitary operator](../../../vector-space.md#unitary-operator) has norm one.

For [unitary product telescoping](../../../continuous-dual-space.md#unitary-product-telescoping), replace the factors one at a time. With empty products interpreted as the identity,

$$
U_m\cdots U_1-V_m\cdots V_1
=\sum_{j=1}^m U_m\cdots U_{j+1}(U_j-V_j)V_{j-1}\cdots V_1.
$$

All cross terms cancel. By the triangle inequality and unitary invariance of the [spectral norm](../../../continuous-dual-space.md#matrix-2-norm),

$$
\boxed{\|U_m\cdots U_1-V_m\cdots V_1\|
\leq\sum_{j=1}^m\|U_j-V_j\|<m\epsilon.}
$$

This bound is independent of the dimension and does not assume that any of the factors commute.

<h3 id="4/ii">ii</h3>

↑ **Parent:** [4](#4)

<h4 id="4/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#4/ii)

For [first-order two-local Hamiltonian simulation](../../../quantum-theory.md#first-order-two-local-hamiltonian-simulation), regard each term $H_k$ as a [Hermitian operator](../../../hilbert-space.md#hermitian-operator), as is standard for a local-Hamiltonian decomposition. The [Lie-Trotter product formula](../../../numerical-analysis.md#lie-product-formula) for bounded operators states

$$
e^{\sum_k A_k}=\lim_{r\to\infty}\left(e^{A_M/r}\cdots e^{A_1/r}\right)^r
$$

in [operator norm](../../../continuous-dual-space.md#operator-norm); the reversed factor ordering is just as valid as the displayed one. Take $A_k=-iH_k$ and use the circuit

$$
V_r=\left(e^{-iH_M/r}\cdots e^{-iH_1/r}\right)^r.
$$

Each factor is a [unitary operator](../../../vector-space.md#unitary-operator) on at most two [qubits](../../../quantum-mechanics.md#qubit) and hence is one allowed two-[qubit](../../../quantum-mechanics.md#qubit) gate, with a spectator identity for a one-[qubit](../../../quantum-mechanics.md#qubit) term. The factors in the rightmost part of each written product act first. Merely quoting the limit would not establish the requested rate, so we give a quantitative error bound.

For two [Hermitian operators](../../../hilbert-space.md#hermitian-operator) $A,B$ and $t\geq0$, differentiating

$$
F(s)=e^{-i(t-s)(A+B)}e^{-isA}e^{-isB},\qquad0\leq s\leq t,
$$

gives $F'(s)=i e^{-i(t-s)(A+B)}[B,e^{-isA}]e^{-isB}$. The [commutator](../../../lie-algebra.md#commutator) identity obtained by differentiating $e^{iuA}Be^{-iuA}$ implies $\|[B,e^{-isA}]\|\leq s\|[A,B]\|$. Since the surrounding factors are unitary, integration yields the [first-order unitary product-formula error bound](../../../numerical-analysis.md#first-order-unitary-product-formula-error-bound)

$$
\|e^{-it(A+B)}-e^{-itA}e^{-itB}\|\leq\frac{t^2}{2}\|[A,B]\|.
$$

Splitting the terms successively and using the triangle inequality therefore gives the one-step estimate

$$
\left\|e^{-iH/r}-e^{-iH_M/r}\cdots e^{-iH_1/r}\right\|
\leq\frac1{2r^2}\sum_{k<\ell}\|[H_k,H_\ell]\|
<\frac{M(M-1)}{2r^2},
$$

for $M>1$. Here [submultiplicativity of the operator norm](../../../continuous-dual-space.md#submultiplicativity-of-the-operator-norm) gives $\|[H_k,H_\ell]\|\leq2\|H_k\|\|H_\ell\|<2$. The ordering chosen for the products changes the sign of local commutators, not this norm bound. Applying part (i) to the $r$ steps gives

$$
\boxed{\|e^{-iH}-V_r\|\leq\frac1{2r}\sum_{k<\ell}\|[H_k,H_\ell]\|
<\frac{M(M-1)}{2r}.}
$$

Choose $r=\max(1,\lceil M(M-1)/(2\epsilon)\rceil)$. For $M>1$ the error is strictly below $\epsilon$; $M=1$ is exact already with $r=1$. The [quantum circuit](../../../quantum-circuit.md) contains $Mr$ two-[qubit](../../../quantum-mechanics.md#qubit) gates. **A sufficient gate count is**

$$
\boxed{Mr=O\!\left(M+\frac{M^3}{\epsilon}\right)
=O\!\left(\frac{n^6}{\epsilon}\right),\qquad0<\epsilon\leq1.}
$$

Thus the worst-case polynomial degree in this first-order bound is six. Terms with disjoint supports commute and may improve the count in particular decompositions, but the stated assumptions alone suffice for this bound, without a further sparsity or bounded-degree condition. The requested gate model allows arbitrary two-[qubit](../../../quantum-mechanics.md#qubit) unitaries, so no additional compilation error is incurred here.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2016](../../2016.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
