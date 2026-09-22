# Paper 324

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2025/III_Paper_324.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2025/III_Paper_324.pdf)

**Table of contents**

- [1](#1)
  - [a](#1/a)
    - [i](#1/a/i)
      - [Solution](#1/a/i/solution)
    - [ii](#1/a/ii)
      - [Solution](#1/a/ii/solution)
  - [b](#1/b)
    - [i](#1/b/i)
      - [Solution](#1/b/i/solution)
    - [ii](#1/b/ii)
      - [Solution](#1/b/ii/solution)
    - [iii](#1/b/iii)
      - [Solution](#1/b/iii/solution)
    - [iv](#1/b/iv)
      - [Solution](#1/b/iv/solution)
- [2](#2)
  - [i](#2/i)
    - [Solution](#2/i/solution)
  - [ii](#2/ii)
    - [Solution](#2/ii/solution)
  - [iii](#2/iii)
    - [Solution](#2/iii/solution)
  - [iv](#2/iv)
    - [Solution](#2/iv/solution)
- [3](#3)
  - [a](#3/a)
    - [i](#3/a/i)
      - [Solution](#3/a/i/solution)
    - [ii](#3/a/ii)
      - [Solution](#3/a/ii/solution)
    - [iii](#3/a/iii)
      - [Solution](#3/a/iii/solution)
    - [iv](#3/a/iv)
      - [Solution](#3/a/iv/solution)
  - [b](#3/b)
    - [Solution](#3/b/solution)
  - [c](#3/c)
    - [Solution](#3/c/solution)
- [4](#4)
  - [a](#4/a)
    - [i](#4/a/i)
      - [Solution](#4/a/i/solution)
    - [ii](#4/a/ii)
      - [Solution](#4/a/ii/solution)
  - [b](#4/b)
    - [Solution](#4/b/solution)

## 1

↑ **Parent:** [Paper 324](paper-324.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/i">i</h4>

↑ **Parent:** [A](#1/a)

<h5 id="1/a/i/solution">Solution</h5>

↑ **Parent:** [I](#1/a/i)

Let $H=\operatorname{Stab}_F(x)$. The identity belongs to $H$ because $F(e,x)=x$. If $g,h\in H$, the [group action](../../../group-theory.md#group-action) law gives

$$
F(gh,x)=F(g,F(h,x))=F(g,x)=x,
$$

so $gh\in H$. Finally, if $g\in H$, then

$$
x=F(e,x)=F(g^{-1}g,x)=F(g^{-1},F(g,x))=F(g^{-1},x),
$$

so $g^{-1}\in H$. The [subgroup](../../../group.md#subgroup) criterion therefore proves that $\operatorname{Stab}_F(x)$ is the [stabilizer subgroup](../../../group-theory.md#stabilizer-subgroup) of $x$.

<h4 id="1/a/ii">ii</h4>

↑ **Parent:** [A](#1/a)

<h5 id="1/a/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#1/a/ii)

Put $H=\operatorname{Stab}_F(x)$. For $g,h\in G$,

$$
\begin{aligned}
f_x(g)=f_x(h)
&\iff F(g,x)=F(h,x)\\
&\iff F(h^{-1}g,x)=x\\
&\iff h^{-1}g\in H\\
&\iff g\in hH.
\end{aligned}
$$

**Thus $f_x$ is constant on every left [coset](../../../group-theory.md#coset) of $H$ and takes different values on different cosets. Its oracle is therefore an oracle for the [hidden subgroup problem](../../../quantum-theory.md#hidden-subgroup-problem), and the hidden subgroup is precisely the [stabilizer subgroup](../../../group-theory.md#stabilizer-subgroup) $H$.**

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/i">i</h4>

↑ **Parent:** [B](#1/b)

<h5 id="1/b/i/solution">Solution</h5>

↑ **Parent:** [I](#1/b/i)

Since $\gcd(x,N)=1$, multiplication by $x$ modulo $N$ is a [bijection](../../../function.md#bijection) of $\mathbb Z_N$, with inverse multiplication by the [modular inverse](../../../number-theory.md#modular-multiplicative-inverse) $x^{-1}$. Hence $U_x$ permutes the standard orthonormal basis. It preserves all inner products and satisfies

$$
U_x^\dagger=U_{x^{-1}},
\qquad
U_x^\dagger U_x=I,
$$

so $U_x$ is a [unitary operator](../../../vector-space.md#unitary-operator).

<h4 id="1/b/ii">ii</h4>

↑ **Parent:** [B](#1/b)

<h5 id="1/b/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#1/b/ii)

The [multiplicative order](../../../number-theory.md#multiplicative-order) $r$ makes the states $|a^k\bmod N\rangle$, $0\leq k<r$, distinct and cyclic under $U_a$. Therefore

$$
\begin{aligned}
U_a|\psi_s\rangle
&=\frac1{\sqrt r}\sum_{k=0}^{r-1}
e^{-2\pi isk/r}|a^{k+1}\bmod N\rangle\\
&=e^{2\pi is/r}\frac1{\sqrt r}\sum_{j=0}^{r-1}
e^{-2\pi isj/r}|a^j\bmod N\rangle.
\end{aligned}
$$

Thus each $|\psi_s\rangle$ is an [eigenvector](../../../linear-operator-theory.md#eigenvector) with

$$
\boxed{U_a|\psi_s\rangle=e^{2\pi is/r}|\psi_s\rangle}.
$$

These are the Fourier eigenvectors of the cyclic modular-multiplication orbit.

<h4 id="1/b/iii">iii</h4>

↑ **Parent:** [B](#1/b)

<h5 id="1/b/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#1/b/iii)

Summing the eigenvectors and reversing the finite sums gives

$$
\frac1{\sqrt r}\sum_{s=0}^{r-1}|\psi_s\rangle
=\frac1r\sum_{k=0}^{r-1}
\left(\sum_{s=0}^{r-1}e^{-2\pi isk/r}\right)
|a^k\bmod N\rangle.
$$

The [root-of-unity filter](../../../algebra.md#root-of-unity-filter) makes the inner sum equal to $r$ for $k=0$ and zero otherwise. Since $a^0=1$,

$$
\boxed{\frac1{\sqrt r}\sum_{s=0}^{r-1}|\psi_s\rangle=|1\rangle}.
$$

<h4 id="1/b/iv">iv</h4>

↑ **Parent:** [B](#1/b)

<h5 id="1/b/iv/solution">Solution</h5>

↑ **Parent:** [Iv](#1/b/iv)

Use $|1\rangle$ as the target register for [quantum phase estimation](../../../quantum-theory.md#quantum-phase-estimation) of $U_a$. By part (iii), it is the equal superposition $r^{-1/2}\sum_s|\psi_s\rangle$ of eigenvectors with phases $s/r$. Controlled modular multiplications implement the required powers $U_a^{2^j}$ efficiently. The phase-estimation circuit produces

$$
\frac1{\sqrt r}\sum_{s=0}^{r-1}
|\widetilde{s/r}\rangle|\psi_s\rangle,
$$

where the first register contains an $m$-bit approximation with constant success probability. A [quantum measurement in the computational basis](../../../quantum-theory.md#quantum-measurement-in-the-computational-basis) therefore outputs an approximation to $s/r$, with $s$ uniformly distributed over $\{0,\ldots,r-1\}$.

## 2

↑ **Parent:** [Paper 324](paper-324.md)

<h3 id="2/i">i</h3>

↑ **Parent:** [2](#2)

<h4 id="2/i/solution">Solution</h4>

↑ **Parent:** [I](#2/i)

For the [HHL algorithm](../../../quantum-theory.md#hhl-algorithm) to have runtime polynomial in $\log N$, the Hermitian matrix $A$ must be invertible, have a [condition number](../../../linear-algebra.md#condition-number) $\kappa$ bounded by $\operatorname{poly}(\log N)$, and be a [sparse matrix](../../../vector-space.md#sparse-matrix) with its nonzero entries efficiently accessible by an oracle. The normalized state $|b\rangle$ must also be preparable in $\operatorname{poly}(\log N)$ time. With precision costs suppressed, these assumptions let HHL prepare, with high probability,

$$
\boxed{|\xi\rangle=\frac{A^{-1}|b\rangle}
{\|A^{-1}|b\rangle\|}}.
$$

<h3 id="2/ii">ii</h3>

↑ **Parent:** [2](#2)

<h4 id="2/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#2/ii)

Normalization gives $p^2+q^2=1$. Write $p=\sin\theta$, $q=\cos\theta$ with $0<\theta<\pi/2$, and set $|u\rangle=U|b\rangle$. Define the two [Householder reflections](../../../linear-algebra.md#householder-transformation)

$$
R_u=2|u\rangle\langle u|-I
=U(2|b\rangle\langle b|-I)U^\dagger,
\qquad
R_\xi=I-2|\xi\rangle\langle\xi|.
$$

The [amplitude amplification](../../../quantum-theory.md#amplitude-amplification) iterate $G=R_uR_\xi$ preserves $\operatorname{span}\{|\xi\rangle,|\phi\rangle\}$ and rotates that plane through $2\theta$. Consequently

$$
\boxed{
G^kU|b\rangle
=\sin((2k+1)\theta)|\xi\rangle
+\cos((2k+1)\theta)|\phi\rangle}.
$$

In particular, $O(1/p)$ iterations raise the success probability to a constant close to one.

<h3 id="2/iii">iii</h3>

↑ **Parent:** [2](#2)

<h4 id="2/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#2/iii)

Choose an integer $k$ large enough that

$$
\theta'=\frac{\pi}{4k+2}\leq\arcsin p,
\qquad
c=\frac{\sin\theta'}p\leq1.
$$

Prepare an ancillary qubit in $\sqrt{1-c^2}|0\rangle+c|1\rangle$ and declare only $|\xi\rangle|1\rangle$ to be good. The initial good amplitude of

$$
U|b\rangle\otimes
\left(\sqrt{1-c^2}|0\rangle+c|1\rangle\right)
$$

is $pc=\sin\theta'$. Applying $k$ [amplitude amplification](../../../quantum-theory.md#amplitude-amplification) iterations gives good amplitude

$$
\sin((2k+1)\theta')=\sin(\pi/2)=1.
$$

The final state is therefore $|\xi\rangle|1\rangle$ up to a global phase. Discarding the ancilla prepares $|\xi\rangle$ exactly; this is [exact amplitude amplification](../../../quantum-theory.md#exact-amplitude-amplification).

<h3 id="2/iv">iv</h3>

↑ **Parent:** [2](#2)

<h4 id="2/iv/solution">Solution</h4>

↑ **Parent:** [Iv](#2/iv)

Let $t=e^{iz}$ and $|u\rangle=U|b\rangle=p|\xi\rangle+q|\phi\rangle$. The first factor in $G$ is

$$
(1-t)|u\rangle\langle u|-I.
$$

Since $R(\xi,z)|u\rangle=pt|\xi\rangle+q|\phi\rangle$, the coefficient of $|\phi\rangle$ in $G|u\rangle$ is

$$
q\left[(1-t)(p^2t+q^2)-1\right].
$$

It vanishes when

$$
(1-t)(p^2t+q^2)=1,
$$

or, using $p^2+q^2=1$,

$$
t+t^{-1}=\frac{p^2-q^2}{p^2}.
$$

A unit-modulus solution $t=e^{iz}$ exists exactly when the right-hand side lies in $[-2,2]$. The upper bound is automatic, while the lower bound is

$$
q^2\leq3p^2.
$$

Thus exact preparation by one application of $G$ is possible precisely when

$$
\boxed{p\geq\frac12}
\qquad\text{or equivalently}\qquad
\boxed{q\leq\sqrt3\,p}.
$$

One may choose $z$ so that $\cos z=(p^2-q^2)/(2p^2)$. Then $G|u\rangle$ has no $|\phi\rangle$ component and, by unitarity, equals $|\xi\rangle$ up to phase. This is a [phase-matched amplitude amplification](../../../quantum-theory.md#phase-matched-amplitude-amplification) step.

## 3

↑ **Parent:** [Paper 324](paper-324.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/i">i</h4>

↑ **Parent:** [A](#3/a)

<h5 id="3/a/i/solution">Solution</h5>

↑ **Parent:** [I](#3/a/i)

With $\omega=e^{2\pi i/Q}$, the [quantum Fourier transform](../../../quantum-theory.md#quantum-fourier-transform) over the additive group $\mathbb Z_Q$ is

$$
\boxed{
\operatorname{QFT}_Q|a\rangle
=\frac1{\sqrt Q}\sum_{b=0}^{Q-1}\omega^{ab}|b\rangle}.
$$

<h4 id="3/a/ii">ii</h4>

↑ **Parent:** [A](#3/a)

<h5 id="3/a/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#3/a/ii)

Apply [Hadamard gates](../../../quantum-theory.md#hadamard-gate) to $|0^m\rangle$ to prepare

$$
2^{-m/2}\sum_{x=0}^{2^m-1}|x\rangle.
$$

Reversibly compute the efficiently decidable predicate $[x<Q]$ into an ancillary qubit and measure it. The success probability is $Q/2^m>1/2$, and conditioned on success the first register is exactly

$$
|\xi\rangle=\frac1{\sqrt Q}\sum_{b=0}^{Q-1}|b\rangle.
$$

Restart after a failed measurement. After $L=\lceil\log_2(1/\delta)\rceil$ attempts, the probability that all attempts fail is below $\delta$, so the state is prepared with probability at least $1-\delta$ using a number of gates polynomial in $m$ and $\log(1/\delta)$.

<h4 id="3/a/iii">iii</h4>

↑ **Parent:** [A](#3/a)

<h5 id="3/a/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#3/a/iii)

Write $b=\sum_{j=0}^{m-1}2^jb_j$. Applying the [phase gate](../../../quantum-theory.md#phase-gate)

$$
P\left(\frac{2\pi2^j}{Q}\right)
$$

to qubit $b_j$ contributes $\exp(2\pi i2^jb_j/Q)$. The product of these $m$ gates is therefore

$$
\boxed{U|b\rangle=\omega^b|b\rangle}.
$$

Similarly, for $a=\sum_ja_j2^j$ and $b=\sum_kb_k2^k$, apply a [controlled phase gate](../../../quantum-theory.md#controlled-phase-gate)

$$
CP\left(\frac{2\pi2^{j+k}}Q\right)
$$

between every pair $(a_j,b_k)$. The accumulated phase is

$$
\prod_{j,k}\exp\left(\frac{2\pi i}{Q}a_jb_k2^{j+k}\right)
=\omega^{ab}.
$$

The $m^2$ controlled phase gates implement

$$
\boxed{V|a\rangle|b\rangle=\omega^{ab}|a\rangle|b\rangle}.
$$

<h4 id="3/a/iv">iv</h4>

↑ **Parent:** [A](#3/a)

<h5 id="3/a/iv/solution">Solution</h5>

↑ **Parent:** [Iv](#3/a/iv)

Prepare $|\xi\rangle=Q^{-1/2}\sum_b|b\rangle$ in the second register by part (ii), while preserving the first register $|a\rangle$. Applying the diagonal unitary $V$ from part (iii) gives

$$
V|a\rangle|\xi\rangle
=|a\rangle\frac1{\sqrt Q}\sum_{b=0}^{Q-1}\omega^{ab}|b\rangle
=\boxed{|a\rangle\operatorname{QFT}_Q|a\rangle}.
$$

The preparation can be made coherent using [amplitude amplification](../../../quantum-theory.md#amplitude-amplification) in place of postselection when this map is needed as a subroutine.

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

The shift $S|x\rangle=|x-1\bmod Q\rangle$ acts on a Fourier state as

$$
\begin{aligned}
S\operatorname{QFT}_Q|a\rangle
&=\frac1{\sqrt Q}\sum_x\omega^{ax}|x-1\rangle\\
&=\omega^a\operatorname{QFT}_Q|a\rangle.
\end{aligned}
$$

Thus $\operatorname{QFT}_Q|a\rangle$ is an [eigenvector](../../../linear-operator-theory.md#eigenvector) of $S$ with eigenphase $a/Q$. Apply the unitary part of [exact quantum phase estimation](../../../quantum-theory.md#exact-quantum-phase-estimation) for $S$ to a zeroed control register and this Fourier state. It writes the eigenphase label coherently:

$$
\boxed{
|0^m\rangle\operatorname{QFT}_Q|a\rangle
\longmapsto
|a\rangle\operatorname{QFT}_Q|a\rangle}.
$$

<h3 id="3/c">c</h3>

↑ **Parent:** [3](#3)

<h4 id="3/c/solution">Solution</h4>

↑ **Parent:** [C](#3/c)

Start with $(|a\rangle+|b\rangle)/\sqrt2$ and a zeroed second register. Apply the coherent construction from part (a)(iv) to obtain

$$
\frac1{\sqrt2}\left(
|a\rangle\operatorname{QFT}_Q|a\rangle
+|b\rangle\operatorname{QFT}_Q|b\rangle\right).
$$

Now run the inverse of the phase-estimation map from part (b) on the two registers. It erases the first label in both branches:

$$
|0^m\rangle\frac{
\operatorname{QFT}_Q|a\rangle+
\operatorname{QFT}_Q|b\rangle}{\sqrt2}
=|0^m\rangle\operatorname{QFT}_Q
\frac{|a\rangle+|b\rangle}{\sqrt2}.
$$

Discarding the zeroed register leaves the required [quantum Fourier transform](../../../quantum-theory.md#quantum-fourier-transform) of the superposition. The coherent use of a computed label followed by its inverse is an [uncomputation](../../../quantum-theory.md#uncomputation).

## 4

↑ **Parent:** [Paper 324](paper-324.md)

<h3 id="4/a">a</h3>

↑ **Parent:** [4](#4)

<h4 id="4/a/i">i</h4>

↑ **Parent:** [A](#4/a)

<h5 id="4/a/i/solution">Solution</h5>

↑ **Parent:** [I](#4/a/i)

The process admits a [strong classical simulation of a quantum circuit](../../../quantum-circuit.md#strong-classical-simulation-of-a-quantum-circuit) if a classical algorithm, given its circuit and input descriptions, computes either output probability to the requested polynomial precision in time polynomial in the input size and precision parameter. This asks for the probabilities themselves, rather than only efficient samples from their distribution.

<h4 id="4/a/ii">ii</h4>

↑ **Parent:** [A](#4/a)

<h5 id="4/a/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#4/a/ii)

Suppose output qubit $j$ is measured. Its probability of outcome zero is

$$
p_0=\frac12\left(1+
\langle\psi|C^\dagger Z_jC|\psi\rangle\right).
$$

Because $C$ is a [Clifford operation](../../../quantum-circuit.md#clifford-gate), the [Pauli group](../../../quantum-circuit.md#pauli-group) is preserved under conjugation. Propagating $Z_j$ backward through the $N=\operatorname{poly}(n)$ gates therefore produces, including its sign, a tensor-product Pauli

$$
C^\dagger Z_jC=\eta\,P_1\otimes\cdots\otimes P_n.
$$

The input is a [product state](../../../bell-state.md#product-state), so the expectation factors:

$$
\langle\psi|C^\dagger Z_jC|\psi\rangle
=\eta\prod_{k=1}^n\langle\alpha_k|P_k|\alpha_k\rangle.
$$

Each one-qubit factor follows directly from the classical description of $|\alpha_k\rangle$, and conjugating a Pauli through each Clifford gate takes constant classical work. Hence $p_0$, and $p_1=1-p_0$, are computable in polynomial time. This is [Heisenberg propagation of a Pauli observable through a Clifford circuit](../../../quantum-circuit.md#heisenberg-propagation-of-a-pauli-observable-through-a-clifford-circuit).

<h3 id="4/b">b</h3>

↑ **Parent:** [4](#4)

<h4 id="4/b/solution">Solution</h4>

↑ **Parent:** [B](#4/b)

Write $|\psi\rangle=\alpha|0\rangle+\beta|1\rangle$ and $t=e^{i\theta}$. Before measurement, the three [controlled-NOT gates](../../../quantum-theory.md#controlled-not-gate) map a computational-basis component $|x,y,0\rangle$ to

$$
|x,y\mathbin\oplus x,y\mathbin\oplus x\rangle.
$$

The measured bit is therefore $b=y\mathbin\oplus x$. For $b=0$, the unnormalized state of the first qubit is

$$
\frac1{\sqrt2}(\alpha|0\rangle+t\beta|1\rangle)
=\frac1{\sqrt2}P(\theta)|\psi\rangle.
$$

For $b=1$, it is

$$
\frac1{\sqrt2}(t\alpha|0\rangle+\beta|1\rangle)
=\frac t{\sqrt2}P(-\theta)|\psi\rangle.
$$

Each branch has probability $1/2$; after normalization and removal of the irrelevant global phase $t$, the two outputs are

$$
\boxed{P(\theta)|\psi\rangle\quad\text{and}\quad
P(-\theta)|\psi\rangle}
$$

with equal probability. This is [probabilistic phase-gate injection](../../../quantum-theory.md#probabilistic-phase-gate-injection).

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2025](../../2025.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
