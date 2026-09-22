# Paper 49

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2010/Paper49.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2010/Paper49.pdf)

**Table of contents**

- [1](#1)
  - [a](#1/a)
    - [Solution](#1/a/solution)
  - [b](#1/b)
    - [Solution](#1/b/solution)
  - [c](#1/c)
    - [Solution](#1/c/solution)
- [2](#2)
  - [a](#2/a)
    - [Solution](#2/a/solution)
  - [b](#2/b)
    - [Solution](#2/b/solution)
  - [c](#2/c)
    - [Solution](#2/c/solution)
  - [d](#2/d)
    - [Solution](#2/d/solution)
- [3](#3)
  - [a](#3/a)
    - [Solution](#3/a/solution)
  - [b](#3/b)
    - [Solution](#3/b/solution)
  - [c](#3/c)
    - [Solution](#3/c/solution)
  - [d](#3/d)
    - [Solution](#3/d/solution)
- [4](#4)
  - [a](#4/a)
    - [Solution](#4/a/solution)
  - [b](#4/b)
    - [Solution](#4/b/solution)
  - [c](#4/c)
    - [Solution](#4/c/solution)
  - [d](#4/d)
    - [Solution](#4/d/solution)

## 1

↑ **Parent:** [Paper 49](paper-49.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

Write $N=2^n$ and $|s\rangle=N^{-1/2}\sum_{x=0}^{N-1}|x\rangle$. The initial [Hadamard gates](../../../quantum-theory.md#hadamard-gate) prepare $|s\rangle$ in the search register and $|-\rangle$ in the final [quantum ancilla](../../../quantum-information-theory.md#quantum-ancilla). Since the [Pauli X gate](../../../quantum-theory.md#pauli-x-gate) satisfies $X|-\rangle=-|-\rangle$, the [Boolean quantum oracle](../../../quantum-theory.md#boolean-quantum-oracle) acts by [quantum phase kickback](../../../quantum-theory.md#phase-kickback):

$$
U_f(|x\rangle|-\rangle)=(-1)^{f(x)}|x\rangle|-\rangle.
$$

For a single marked entry this is the [marked-state phase oracle](../../../quantum-theory.md#marked-state-phase-oracle) $O_a=I-2|a\rangle\langle a|$ on the search register. The ancilla stays separate and unchanged throughout.

The [Grover diffusion operator](../../../quantum-theory.md#grover-diffusion-operator) is $V=2|s\rangle\langle s|-I$, because $H^{\otimes n}|0^n\rangle=|s\rangle$. The PDF circuit places one diffusion after each oracle call, so the state before measurement is

$$
(VO_a)^k|s\rangle\otimes|-\rangle.
$$

In the supplied [amplitude amplification theorem](../../../quantum-theory.md#amplitude-amplification), take $|\psi\rangle=|s\rangle$ and $|\phi\rangle=|a\rangle$. Their overlap has modulus $1/\sqrt N$, so the [Grover rotation angle](../../../quantum-theory.md#grover-rotation-angle) is $\theta=\arcsin(N^{-1/2})$. A [quantum measurement in the computational basis](../../../quantum-theory.md#quantum-measurement-in-the-computational-basis) therefore gives

$$
\boxed{\mathbb P(\text{output }a)=\sin^2((2k+1)\theta).}
$$

The inverse sine here is applied to the overlap of the two different states. The converted TeX's self-overlap in the angle definition is a transcription error; the original PDF has $|\langle\phi|\psi\rangle|$.

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

If there is no marked entry, the [Boolean quantum oracle](../../../quantum-theory.md#boolean-quantum-oracle) is the identity. The [uniform superposition state](../../../quantum-circuit.md#uniform-superposition-state) is a positive eigenstate of the [Grover diffusion operator](../../../quantum-theory.md#grover-diffusion-operator):

$$
V|s\rangle=(2|s\rangle\langle s|-I)|s\rangle=|s\rangle.
$$

Thus every iteration leaves the full state $|s\rangle\otimes|-\rangle$ unchanged. The measured search bits have the [uniform distribution](../../../continuous-probability-distribution.md#continuous-uniform-distribution)

$$
\boxed{\mathbb P(\text{output }x)=\frac1N\quad(0\leq x<N).}
$$

Only the first $n$ qubits are measured in the printed circuit. If the untouched ancilla were also measured in the computational basis, its bit would be an independent fair bit, giving probability $1/(2N)$ for each joint outcome.

<h3 id="1/c">c</h3>

↑ **Parent:** [1](#1)

<h4 id="1/c/solution">Solution</h4>

↑ **Parent:** [C](#1/c)

Use a [verified Grover promise test](../../../quantum-theory.md#verified-grover-promise-test). Since $n>1$, $N\geq4$. Choose

$$
k=\left\lfloor\frac\pi{4\theta}\right\rfloor,\qquad \theta=\arcsin(N^{-1/2}).
$$

This is a nearest integer to $\pi/(4\theta)-1/2$, so $|(2k+1)\theta-\pi/2|\leq\theta$. Run the [Grover search algorithm](../../../quantum-theory.md#grover-s-algorithm) for $k$ iterations and measure the candidate $x$. Make one further oracle query with input $|x\rangle|0\rangle$ and measure the answer bit $f(x)$. Declare that a marked entry exists exactly when this bit is one.

In the zero case the verification always returns zero, so the decision is correct with certainty. In the single-marked-entry case, verification returns one exactly when the candidate is $a$, and

$$
\mathbb P(\text{correct decision})
=\sin^2((2k+1)\theta)
\geq\cos^2\theta=1-\frac1N\geq\frac34.
$$

Finally, $\arcsin u\geq u$ on $[0,1]$ gives $k\leq\pi\sqrt N/4$. Hence

$$
\boxed{\text{success probability}\geq\frac34,\qquad\text{oracle calls}=k+1=O(\sqrt{2^n}).}
$$

The verification query is necessary for this decision rule: an unverified search-register label does not itself say whether it is marked.

## 2

↑ **Parent:** [Paper 49](paper-49.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

The [Pauli Z gate](../../../quantum-theory.md#pauli-z-gate) exchanges the two [Hadamard basis](../../../quantum-theory.md#hadamard-basis) states: $Z|+\rangle=|-\rangle$ and $Z|-\rangle=|+\rangle$. Multiplying the displayed gate by the [Pauli X gate](../../../quantum-theory.md#pauli-x-gate) gives

$$
U(\theta)X=|+\rangle\langle1|+e^{-i\theta}|-\rangle\langle0|.
$$

On the other hand,

$$
e^{-i\theta}ZU(-\theta)
=e^{-i\theta}Z\left(|+\rangle\langle0|+e^{i\theta}|-\rangle\langle1|\right)
=e^{-i\theta}|-\rangle\langle0|+|+\rangle\langle1|.
$$

The two operators agree, proving

$$
\boxed{U(\theta)X=e^{-i\theta}ZU(-\theta).}
$$

Also $U(\theta)=H\operatorname{diag}(1,e^{-i\theta})=J(-\theta)$ in the [J gate](../../../bell-state.md#j-gate-in-measurement-based-quantum-computation) convention. Keeping this angle sign explicit avoids confusing the two conventions for [equatorial qubit measurements](../../../quantum-measurement.md#equatorial-qubit-measurement).

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/solution">Solution</h4>

↑ **Parent:** [B](#2/b)

Prepare the [three-vertex graph-state wire](../../../quantum-circuit.md#three-vertex-graph-state-wire): start all three [qubits](../../../quantum-mechanics.md#qubit) in $|+\rangle$ and apply [Controlled-Z gates](../../../quantum-theory.md#controlled-z-gate) on edges $1-2$ and $2-3$. In this paper's [equatorial qubit measurement](../../../quantum-measurement.md#equatorial-qubit-measurement) convention the basis vectors can be chosen as

$$
|v_r(\theta)\rangle=\frac{|0\rangle+(-1)^re^{i\theta}|1\rangle}{\sqrt2}.
$$

The given identity means that measuring an input qubit at angle $\theta$, with outcome $r$, teleports its state to the next qubit as $X^rU(\theta)|\psi\rangle$. Each outcome has probability $1/2$, since $X^rU(\theta)$ is unitary. This is [one-bit teleportation](../../../bell-state.md#one-bit-teleportation) with a known [Pauli frame](../../../quantum-circuit.md#pauli-frame).

Measure vertex 1 at angle $\alpha$ and record $r$. Then measure vertex 2 at angle $\gamma=(-1)^r\beta$, taken modulo $2\pi$, and record $s$. The controlled-Z on edge $2-3$ commutes with the first measurement, so the two teleportation steps can be applied successively. The remaining normalized state is

$$
X^sU(\gamma)X^rU(\alpha)|+\rangle.
$$

For $r=0$ this is $X^sU(\beta)U(\alpha)|+\rangle$. For $r=1$, the relation proved above gives $U(-\beta)X=e^{i\beta}ZU(\beta)$. Thus in every branch the remaining state is

$$
e^{ir\beta}X^sZ^rU(\beta)U(\alpha)|+\rangle.
$$

The scalar is a [global phase](../../../quantum-mechanics.md#global-phase) and has no effect on probabilities.

Finally measure vertex 3 in the [computational basis](../../../quantum-theory.md#computational-basis), obtaining $z$, and report

$$
\boxed{k=z\oplus s.}
$$

The $Z^r$ byproduct changes only computational-basis phases; $X^s$ changes the output label by $s$. Hence the corrected bit has exactly the ideal circuit's [probability distribution](../../../probability-theory.md#probability-distribution) in every branch, not merely on average. The procedure uses only single-qubit measurements after preparing the graph state, adaptive classical angle selection, and deterministic classical output processing.

<h3 id="2/c">c</h3>

↑ **Parent:** [2](#2)

<h4 id="2/c/solution">Solution</h4>

↑ **Parent:** [C](#2/c)

First expand the result of the first gate in the [computational basis](../../../quantum-theory.md#computational-basis):

$$
U(\alpha)|+\rangle
=\frac{|+\rangle+e^{-i\alpha}|-\rangle}{\sqrt2}
=\frac{1+e^{-i\alpha}}2|0\rangle+\frac{1-e^{-i\alpha}}2|1\rangle.
$$

Using $1+e^{-i\alpha}=2e^{-i\alpha/2}\cos(\alpha/2)$ and $1-e^{-i\alpha}=2ie^{-i\alpha/2}\sin(\alpha/2)$, this becomes

$$
e^{-i\alpha/2}\left(\cos(\alpha/2)|0\rangle+i\sin(\alpha/2)|1\rangle\right).
$$

Apply $U(\beta)|0\rangle=|+\rangle$ and $U(\beta)|1\rangle=e^{-i\beta}|-\rangle$ to obtain

$$
\boxed{U(\beta)U(\alpha)|+\rangle
=e^{-i\alpha/2}\left(\cos(\alpha/2)|+\rangle+i e^{-i\beta}\sin(\alpha/2)|-\rangle\right).}
$$

For example, its [quantum measurement in the computational basis](../../../quantum-theory.md#quantum-measurement-in-the-computational-basis) has probabilities $\mathbb P(k=0)=(1+\sin\alpha\sin\beta)/2$ and $\mathbb P(k=1)=(1-\sin\alpha\sin\beta)/2$, obtained by squaring the two basis amplitudes.

<h3 id="2/d">d</h3>

↑ **Parent:** [2](#2)

<h4 id="2/d/solution">Solution</h4>

↑ **Parent:** [D](#2/d)

Use [two-bit remote state preparation on a graph-state path](../../../quantum-information-theory.md#two-bit-remote-state-preparation-on-a-graph-state-path). Alice performs the first two measurements from the preceding [measurement-based quantum computation](../../../quantum-circuit.md#measurement-based-quantum-computation): angle $\alpha$ on her first qubit, giving $r$, then angle $(-1)^r\beta$ on her second, giving $s$. She sends the pair $(r,s)$ to Bob, using exactly two [classical communication](../../../quantum-information-theory.md#classical-communication) bits.

The branch calculation already gives Bob's state as $e^{ir\beta}X^sZ^r|\chi\rangle$, where $|\chi\rangle=U(\beta)U(\alpha)|+\rangle$. Bob applies $X^s$ first and $Z^r$ second, so his correction operator is $Z^rX^s$. Since $X^2=Z^2=I$,

$$
(Z^rX^s)(X^sZ^r)|\chi\rangle=|\chi\rangle.
$$

Thus

$$
\boxed{\text{Alice sends }(r,s);\qquad\text{Bob applies }Z^rX^s.}
$$

The final state is exactly the desired state up to the irrelevant global phase. No postselection is used: all four measurement branches have probability $1/4$ and are corrected. Bob does not need the angles themselves; Alice uses them in her measurement choices, while the two bits specify his Pauli correction.

## 3

↑ **Parent:** [Paper 49](paper-49.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

Number the wires from top to bottom as $1,\ldots,5$. The first two [controlled-NOT gates](../../../quantum-theory.md#controlled-not-gate) encode $|\psi\rangle=u|0\rangle+v|1\rangle$ into the [bit-flip repetition code](../../../quantum-error-correction.md#bit-flip-repetition-code)

$$
u|000\rangle+v|111\rangle
$$

on data wires $1,2,3$. The lower two zero ancillas store an [error syndrome](../../../quantum-error-correction.md#error-syndrome). Reading the PDF's four detection CNOTs gives

$$
s_4=b_2\oplus b_3,\qquad s_5=b_1\oplus b_3.
$$

The syndrome and the data qubit to be flipped are therefore

$$
\begin{array}{c|c|c}
\text{physical error}&(s_4,s_5)&\text{recovery target}\\\hline
I&00&\text{none}\\
X_1&01&1\\
X_2&10&2\\
X_3&11&3
\end{array}
$$

This is [coherent syndrome extraction for the three-qubit repetition code](../../../quantum-error-correction.md#coherent-syndrome-extraction-for-the-three-qubit-repetition-code). The recovery [Toffoli gates](../../../quantum-theory.md#toffoli-gate) implement these conditions; the intervening [Pauli X gates](../../../quantum-theory.md#pauli-x-gate) temporarily turn zero-valued controls into one-valued controls and then restore the syndrome wires. Finally, inverse encoding returns the logical state to the top wire and resets data wires 2 and 3 to zero.

For the specified error $X_1$, the encoded data becomes $u|100\rangle+v|011\rangle$. Both terms have syndrome $01$, so detection factors out $|01\rangle_{45}$ without revealing the logical amplitudes. Recovery flips data wire 1, restoring $u|000\rangle+v|111\rangle$, and decoding yields

$$
\boxed{|\psi\rangle_1\otimes|0\rangle_2\otimes|0\rangle_3\otimes|0\rangle_4\otimes|1\rangle_5.}
$$

The lower four wires need not all return to zero: their syndrome record is independent of the logical state, which is what the correction requirement needs.

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

Use the [Hadamard gate](../../../quantum-theory.md#hadamard-gate) identity $H=(X+Z)/\sqrt2$ on the first data wire. The $X_1$ branch is corrected as above and has syndrome $01$. The $Z_1$ branch changes the encoded state to $\alpha|000\rangle-\beta|111\rangle$, with syndrome $00$. No bit-flip recovery is triggered, and decoding leaves $Z|\psi\rangle$ on the top wire.

By linearity of the full [quantum circuit](../../../quantum-circuit.md), its output for $H_1$ is therefore

$$
\frac1{\sqrt2}\left(|\psi\rangle\otimes|0001\rangle+Z|\psi\rangle\otimes|0000\rangle\right),
$$

where the four-bit strings are ordered as wires $2,3,4,5$. The two syndrome states are orthogonal. Taking their [partial trace](../../../quantum-theory.md#partial-trace) removes the cross terms, so the [reduced density matrix](../../../bell-state.md#reduced-density-matrix) is

$$
\rho=\frac12\left(|\psi\rangle\langle\psi|+Z|\psi\rangle\langle\psi|Z\right)
=\boxed{\begin{pmatrix}|\alpha|^2&0\\0&|\beta|^2\end{pmatrix}.}
$$

The top output undergoes a [completely dephasing channel](../../../quantum-measurement.md#rank-one-dephasing) in the computational basis. The bit-flip component is corrected, but the undetected phase component destroys logical coherence after the syndrome is ignored.

<h3 id="3/c">c</h3>

↑ **Parent:** [3](#3)

<h4 id="3/c/solution">Solution</h4>

↑ **Parent:** [C](#3/c)

The point needing proof is that a corrected error's residual state cannot retain dependence on the logical input. Let $W_j$ denote the complete linear map from the logical input to all five output wires for error $E_j$. Protection gives $W_j|0\rangle=|0\rangle|\eta_{j,0}\rangle$ and $W_j|1\rangle=|1\rangle|\eta_{j,1}\rangle$. Applying protection to $|+\rangle$ and comparing its two top-qubit components yields

$$
\frac{|0\rangle|\eta_{j,0}\rangle+|1\rangle|\eta_{j,1}\rangle}{\sqrt2}
=|+\rangle|\eta_{j,+}\rangle,
$$

so $|\eta_{j,0}\rangle=|\eta_{j,1}\rangle=|\eta_{j,+}\rangle$. Denote the common vector by $|\eta_j\rangle$. Linearity then gives $W_j|\psi\rangle=|\psi\rangle|\eta_j\rangle$ for every input.

The encoding and all operations surrounding the error are fixed. Replacing the error by $E=\alpha E_1+\beta E_2$ consequently replaces the overall map by $\alpha W_1+\beta W_2$, giving

$$
\boxed{W_E|\psi\rangle=|\psi\rangle\otimes\left(\alpha|\eta_1\rangle+\beta|\eta_2\rangle\right).}
$$

Because $E$ and the surrounding circuit are unitary, the output is normalized for every normalized input; the residual vector in parentheses thus has norm one. This proves [linearity of coherent quantum error correction](../../../quantum-error-correction.md#linearity-of-coherent-quantum-error-correction) and hence protection against $E$. Orthogonality of $|\eta_1\rangle$ and $|\eta_2\rangle$ is not required for this proof.

<h3 id="3/d">d</h3>

↑ **Parent:** [3](#3)

<h4 id="3/d/solution">Solution</h4>

↑ **Parent:** [D](#3/d)

Use [phase-flip protection by Hadamard conjugation](../../../quantum-error-correction.md#phase-flip-protection-by-hadamard-conjugation). Insert a [Hadamard gate](../../../quantum-theory.md#hadamard-gate) on each of the three data wires immediately after the two encoding CNOTs and before the physical error. Insert another Hadamard on each data wire immediately after the error and before syndrome detection. Leave the two syndrome ancillas and every detection, recovery and decoding gate unchanged.

The first layer changes the encoded state to $\alpha|+++\rangle+\beta|---\rangle$, the three-qubit [phase-flip repetition code](../../../quantum-error-correction.md#phase-flip-repetition-code). The two layers surrounding the error turn the effective error seen by the old circuit into

$$
E'=H^{\otimes3}EH^{\otimes3}.
$$

Since $H^2=I$ and $HZH=X$, the four physical cases become respectively $I,X_1,X_2,X_3$. The original coherent syndrome and recovery circuit corrects all four, as its syndrome table shows. Thus **two Hadamard layers on the three data wires, straddling the error, give the required phase-flip protection**. The final top wire is the original $|\psi\rangle$, not $H|\psi\rangle$, because the second layer returns the data to the original coding basis before recovery and decoding.

## 4

↑ **Parent:** [Paper 49](paper-49.md)

<h3 id="4/a">a</h3>

↑ **Parent:** [4](#4)

<h4 id="4/a/solution">Solution</h4>

↑ **Parent:** [A](#4/a)

Put $N=2^n$ and label the binary digits of $x$ by $x_{n-1},\ldots,x_0$, with $x=\sum_{j=0}^{n-1}2^jx_j$. The [Walsh-Hadamard transform](../../../quantum-theory.md#walsh-hadamard-transform) prepares the [uniform quantum superposition](../../../quantum-theory.md#uniform-quantum-superposition) $N^{-1/2}\sum_x|x\rangle$. Applying the [phase gate](../../../quantum-theory.md#phase-gate) $R_a^{2^j}$ to the qubit for digit $x_j$ multiplies its basis amplitude by $\exp(2\pi ia2^jx_j/N)$. Taking their product gives

$$
\prod_{j=0}^{n-1}e^{2\pi ia2^jx_j/N}=e^{2\pi iax/N}.
$$

With the most significant qubit written first, this proves

$$
\boxed{\left(R_a^{2^{n-1}}\otimes R_a^{2^{n-2}}\otimes\cdots\otimes R_a\right)H^{\otimes n}|0^n\rangle
=\frac1{\sqrt N}\sum_{x=0}^{N-1}e^{2\pi iax/N}|x\rangle.}
$$

Each power is implemented by repeated uses of the supplied gate. The total is $\sum_{j=0}^{n-1}2^j=N-1$ uses. This realizes [dyadic phase-gate identification](../../../quantum-theory.md#dyadic-phase-gate-identification) without needing an unknown controlled gate or asserting a gate-call cost polynomial in $n$.

<h3 id="4/b">b</h3>

↑ **Parent:** [4](#4)

<h4 id="4/b/solution">Solution</h4>

↑ **Parent:** [B](#4/b)

The inverse [quantum Fourier transform](../../../quantum-theory.md#quantum-fourier-transform) in the original PDF has matrix elements $N^{-1/2}e^{-2\pi iky/N}$ multiplying $|y\rangle\langle k|$. The converted TeX incorrectly repeats $y$ in the bra; using the actual PDF operator,

$$
F^\dagger|\psi\rangle
=\frac1N\sum_{y=0}^{N-1}\left(\sum_{x=0}^{N-1}e^{2\pi i(a-y)x/N}\right)|y\rangle.
$$

If $y=a$, every summand of the inner sum is one, so it equals $N$. If $y\ne a$, let $q=e^{2\pi i(a-y)/N}$. Then $q\ne1$ and $q^N=1$, and the finite [geometric series](../../../real-analysis.md#geometric-series) gives $\sum_{x=0}^{N-1}q^x=(1-q^N)/(1-q)=0$. This is [orthogonality of roots of unity](../../../algebra.md#orthogonality-of-roots-of-unity). Hence

$$
\boxed{F^\dagger|\psi\rangle=|a\rangle.}
$$

A [quantum measurement in the computational basis](../../../quantum-theory.md#quantum-measurement-in-the-computational-basis) consequently returns the integer $a$ with probability one.

<h3 id="4/c">c</h3>

↑ **Parent:** [4](#4)

<h4 id="4/c/solution">Solution</h4>

↑ **Parent:** [C](#4/c)

The eigenvalue on $|0\rangle$ of every power is one, and its eigenvalue on $|1\rangle$ is $e^{2\pi iak/N}$. Thus

$$
R_a^k=R_a^l\quad\Longleftrightarrow\quad e^{2\pi ia(k-l)/N}=1
\quad\Longleftrightarrow\quad N\mid a(k-l).
$$

If $a$ is odd, its [greatest common divisor](../../../number-theory.md#greatest-common-divisor) with $N=2^n$ is one. Divisibility can therefore be cancelled, giving

$$
\boxed{R_a^k=R_a^l\iff k\equiv l\pmod{2^n}.}
$$

In particular, the $N$ powers with $0\leq k<N$ are distinct. Each is the phase gate $R_m$ with $m\equiv ak\pmod N$, and multiplication by $a$ is a permutation of these residue classes. Equivalently, for any desired $m$, choose $k\equiv a^{-1}m\pmod N$, where $a^{-1}$ is the [modular inverse](../../../number-theory.md#modular-multiplicative-inverse). Then $R_a^k=R_m$, using the representative $0\leq k<N$ and repeated forward applications only. Thus the powers generate the entire set. Once the preceding identification procedure has found $a$, these powers can also be labelled and selected classically.

<h3 id="4/d">d</h3>

↑ **Parent:** [4](#4)

<h4 id="4/d/solution">Solution</h4>

↑ **Parent:** [D](#4/d)

Write the normalized [qubit](../../../quantum-mechanics.md#qubit) as $|\phi\rangle=c_0|0\rangle+c_1|1\rangle$, with $|c_0|^2+|c_1|^2=1$. Only the $|1\rangle$ amplitude changes between the two [phase gates](../../../quantum-theory.md#phase-gate), so

$$
\bigl(R(\theta+\delta)-R(\theta)\bigr)|\phi\rangle
=c_1e^{i\theta}(e^{i\delta}-1)|1\rangle.
$$

Since $|e^{i\delta}-1|=2|\sin(\delta/2)|\leq|\delta|$,

$$
\boxed{\|R_m|\phi\rangle-R(\theta)|\phi\rangle\|
=2|c_1||\sin(\delta/2)|\leq|\delta|.}
$$

The [phase-gate discretization error](../../../quantum-theory.md#phase-gate-discretization-error) is uniform over all input states; its exact [operator norm](../../../continuous-dual-space.md#operator-norm) is $2|\sin(\delta/2)|$. To choose an approximating gate, round $N\theta/(2\pi)$ to the nearest integer and reduce it modulo $N$. Taking the shortest circular angle difference gives $|\delta|\leq\pi/N$, and hence a uniform state-vector error at most $\pi/2^n$. The circular choice handles the identified endpoints $0$ and $2\pi$ correctly.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2010](../../2010.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
