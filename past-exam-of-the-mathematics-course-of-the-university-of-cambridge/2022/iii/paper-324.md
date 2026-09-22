# Paper 324

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2022/paper_324.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2022/paper_324.pdf)

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
  - [c](#1/c)
    - [i](#1/c/i)
      - [Solution](#1/c/i/solution)
    - [ii](#1/c/ii)
      - [Solution](#1/c/ii/solution)
- [2](#2)
  - [i](#2/i)
    - [Solution](#2/i/solution)
  - [ii](#2/ii)
    - [Solution](#2/ii/solution)
  - [iii](#2/iii)
    - [Solution](#2/iii/solution)
  - [iv](#2/iv)
    - [Solution](#2/iv/solution)
  - [v](#2/v)
    - [Solution](#2/v/solution)
- [3](#3)
  - [a](#3/a)
    - [i](#3/a/i)
      - [Solution](#3/a/i/solution)
    - [ii](#3/a/ii)
      - [Solution](#3/a/ii/solution)
    - [iii](#3/a/iii)
      - [Solution](#3/a/iii/solution)
  - [b](#3/b)
    - [i](#3/b/i)
      - [Solution](#3/b/i/solution)
    - [ii](#3/b/ii)
      - [Solution](#3/b/ii/solution)
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

↑ **Parent:** [Paper 324](paper-324.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/i">i</h4>

↑ **Parent:** [A](#1/a)

<h5 id="1/a/i/solution">Solution</h5>

↑ **Parent:** [I](#1/a/i)

A $Z$ measurement is a [quantum measurement in the computational basis](../../../quantum-theory.md#quantum-measurement-in-the-computational-basis). To measure $X$, apply a [Hadamard gate](../../../quantum-theory.md#hadamard-gate), measure $Z$, and apply another [Hadamard gate](../../../quantum-theory.md#hadamard-gate) to the measured qubit. Since $HXH=Z$, this gives the $X$ outcome and leaves the qubit in the corresponding $X$ [eigenstate](../../../quantum-mechanics.md#eigenstate).

<h4 id="1/a/ii">ii</h4>

↑ **Parent:** [A](#1/a)

<h5 id="1/a/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#1/a/ii)

Prepare an [ancilla qubit](../../../quantum-information-theory.md#ancilla-qubit) in $|0\rangle$. To measure $X\otimes X$, apply a [Hadamard gate](../../../quantum-theory.md#hadamard-gate) to each data qubit, apply a [controlled-NOT gate](../../../quantum-theory.md#controlled-not-gate) from each data qubit to the ancilla, measure the ancilla in the [computational basis](../../../quantum-theory.md#computational-basis), and apply a Hadamard gate to each data qubit again. The ancilla records the parity of the two rotated computational-basis bits, so outcome $0$ corresponds to eigenvalue $+1$ and outcome $1$ to eigenvalue $-1$. The data register is projected by $[I+(-1)^sX\otimes X]/2$, so its complete [post-measurement state](../../../quantum-measurement.md#post-measurement-state) is retained. For $Z\otimes X$, perform the same [ancilla-assisted Pauli measurement](../../../quantum-theory.md#ancilla-assisted-pauli-measurement) but apply the basis-changing Hadamard gates only to the second data qubit.

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/i">i</h4>

↑ **Parent:** [B](#1/b)

<h5 id="1/b/i/solution">Solution</h5>

↑ **Parent:** [I](#1/b/i)

Since $P|\psi\rangle=\lambda_P|\psi\rangle$, $P^2=I$, and $P$ [anticommutes](../../../vector-space.md#anticommutator) with $Q$,

$$
\langle\psi|Q|\psi\rangle
=\langle\psi|PQP|\psi\rangle
=-\langle\psi|Q|\psi\rangle,
$$

so the [expectation value](../../../quantum-mechanics.md#expectation-value) of $Q$ is zero. The two [spectral projectors](../../../hilbert-space.md#spectral-projector) of the Hermitian [Pauli operator](../../../quantum-circuit.md#pauli-operator) $Q$ are $(I\mathbin\pm Q)/2$, and hence the [Born rule](../../../quantum-mechanics.md#born-rule) gives

$$
\boxed{\Pr(\lambda_Q=\pm1)
=\left\langle\psi\middle|\frac{I\pm Q}{2}\middle|\psi\right\rangle
=\frac12.}
$$

<h4 id="1/b/ii">ii</h4>

↑ **Parent:** [B](#1/b)

<h5 id="1/b/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#1/b/ii)

Put $a=\lambda_P$ and $b=\lambda_Q$. The [Pauli operators](../../../quantum-circuit.md#pauli-operator) are Hermitian and satisfy $P^2=Q^2=I$ and $PQ+QP=0$, so

$$
V^\dagger=V,
\qquad
V^2=\frac12(aP+bQ)^2=I.
$$

Thus $V$ is a [unitary operator](../../../vector-space.md#unitary-operator). For every Pauli operator $R$, according as $R$ commutes or anticommutes with $P$ and $Q$, expansion of $VRV$ gives one of $\pm R$ or $\pm RPQ$, up to the phase that makes it Hermitian. It is therefore another Pauli operator, so $V$ normalizes the [Pauli group](../../../quantum-circuit.md#pauli-group) and is a [Clifford operation](../../../quantum-circuit.md#clifford-gate). Finally,

$$
V|\psi\rangle
=\frac{1}{\sqrt2}(I+bQ)|\psi\rangle,
$$

which is the normalized projection onto the eigenvalue-$b$ [eigenspace](../../../linear-operator-theory.md#eigenspace) of $Q$. Hence $V$ maps the eigenvalue-$\lambda_P$ eigenspace of $P$ onto the eigenvalue-$\lambda_Q$ eigenspace of $Q$.

<h3 id="1/c">c</h3>

↑ **Parent:** [1](#1)

<h4 id="1/c/i">i</h4>

↑ **Parent:** [C](#1/c)

<h5 id="1/c/i/solution">Solution</h5>

↑ **Parent:** [I](#1/c/i)

A [Pauli-based computation](../../../quantum-theory.md#pauli-based-computation) starts with the supplied nonstabilizer resource state $|\alpha\rangle$ and performs an adaptive sequence of mutually commuting [Measurements of Pauli observables](../../../quantum-theory.md#measurement-of-a-pauli-observable). Each outcome is recorded classically and may determine the next Pauli observable and the final classical output. When a proposed observable anticommutes with a previously fixed Pauli constraint, its outcome is uniformly random by part b(i); one samples that outcome and uses the [Clifford operation](../../../quantum-circuit.md#clifford-gate) $V(\lambda_P,\lambda_Q)$ from part b(ii) to update the [Clifford frame](../../../quantum-circuit.md#clifford-frame). This replaces the old constraint by the newly measured one while preserving the distribution and the [post-measurement state](../../../quantum-measurement.md#post-measurement-state) represented by the computation.

<h4 id="1/c/ii">ii</h4>

↑ **Parent:** [C](#1/c)

<h5 id="1/c/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#1/c/ii)

Propagate each output observable backwards through the [Clifford circuit](../../../quantum-circuit.md#clifford-circuit) and write

$$
Q_i=C^\dagger Z_iC.
$$

The $Q_i$ are mutually commuting [Pauli operators](../../../quantum-circuit.md#pauli-operator), and measuring them on $|0\rangle^{\otimes n}\otimes|\phi\rangle$ has exactly the required joint output distribution. Initially the first $n$ qubits are constrained by the [stabilizer generators](../../../quantum-circuit.md#stabilizer-generator) $Z_1,\ldots,Z_n$. Process the $Q_i$ in order. If $Q_i$ anticommutes with a current generator, part b gives a uniform outcome and a [Clifford operation](../../../quantum-circuit.md#clifford-gate) that replaces that generator by $Q_i$; this step needs no measurement on $|\phi\rangle$. If $Q_i$ commutes with every current generator, multiply it by known generators to remove its action on the first register. What remains is a Pauli observable $P_j$ on the $t$ resource qubits and is measured there. The nontrivial $P_j$ are independent and mutually commuting. An independent commuting family of [Pauli operators](../../../quantum-circuit.md#pauli-operator) on $t$ qubits has at most $t$ members, so $s\leq t$. All effective observables are fixed by the original commuting family; the sampled outcomes merely update the classical Clifford frame. The resulting nonadaptive [Pauli-based computation](../../../quantum-theory.md#pauli-based-computation), followed by the stated $Z_1,\ldots,Z_n$ outputs, is therefore a [weak classical simulation of a quantum circuit](../../../quantum-circuit.md#weak-classical-simulation-of-a-quantum-circuit) with the same joint distribution.

## 2

↑ **Parent:** [Paper 324](paper-324.md)

<h3 id="2/i">i</h3>

↑ **Parent:** [2](#2)

<h4 id="2/i/solution">Solution</h4>

↑ **Parent:** [I](#2/i)

An $n$-qubit [stabilizer state](../../../quantum-circuit.md#stabilizer-state) is the unique simultaneous $+1$ [eigenstate](../../../quantum-mechanics.md#eigenstate) of an [abelian group](../../../group.md#abelian-group) $G$ of [Pauli operators](../../../quantum-circuit.md#pauli-operator) having $2^n$ elements and not containing $-I$. The group $G$ is the state's [stabilizer group](../../../quantum-circuit.md#stabilizer-group); equivalently, it is generated by $n$ independent commuting Hermitian Pauli operators.

<h3 id="2/ii">ii</h3>

↑ **Parent:** [2](#2)

<h4 id="2/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#2/ii)

The state $|001\rangle$ has independent [stabilizer generators](../../../quantum-circuit.md#stabilizer-generator) $ZII$, $IZI$, and $-IIZ$. Its complete [stabilizer group](../../../quantum-circuit.md#stabilizer-group) is

$$
\{III,ZII,IZI,-IIZ,ZZI,-ZIZ,-IZZ,-ZZZ\}.
$$

For $|\Phi^+\rangle\otimes|+\rangle$, take the generators $XXI$, $ZZI$, and $IIX$. Their products give

$$
\{III,XXI,ZZI,-YYI,IIX,XXX,ZZX,-YYX\}.
$$

In particular $(XX)(ZZ)=-YY$, which accounts for the two minus signs.

<h3 id="2/iii">iii</h3>

↑ **Parent:** [2](#2)

<h4 id="2/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#2/iii)

The [Gottesman--Knill theorem](../../../quantum-circuit.md#gottesman-knill-theorem) states that [stabilizer-state preparation](../../../quantum-circuit.md#stabilizer-state-preparation), [Clifford circuits](../../../quantum-circuit.md#clifford-circuit), and adaptive [Measurements of Pauli observables](../../../quantum-theory.md#measurement-of-a-pauli-observable) can be simulated in classical polynomial time. For $|\Psi_{\rm in}\rangle=|+\rangle^{\otimes3}$, choose generators $XII$, $IXI$, and $IIX$. With each row written as $[x_1x_2x_3\mid z_1z_2z_3]$, its sign-free [stabilizer tableau](../../../quantum-circuit.md#stabilizer-tableau) is

$$
\begin{pmatrix}
1&0&0&\mid&0&0&0\\
0&1&0&\mid&0&0&0\\
0&0&1&\mid&0&0&0
\end{pmatrix}.
$$

Conjugating these generators successively by $\operatorname{CNOT}_{21}$, $H_2\otimes H_3$, and $\operatorname{CNOT}_{13}$ gives $XIX$, $XZX$, and $ZIZ$. Hence the output tableau, again ignoring signs, is

$$
\begin{pmatrix}
1&0&1&\mid&0&0&0\\
1&0&1&\mid&0&1&0\\
0&0&0&\mid&1&0&1
\end{pmatrix}.
$$

<h3 id="2/iv">iv</h3>

↑ **Parent:** [2](#2)

<h4 id="2/iv/solution">Solution</h4>

↑ **Parent:** [Iv](#2/iv)

At each qubit, two matrices from $\{I,X,Y,Z\}$ either commute or anticommute. Moving every $Q_i$ past the corresponding $P_i$ therefore gives

$$
PQ=(-1)^rQP,
$$

where $r$ is the number of positions containing distinct nonidentity Pauli matrices. Thus two Pauli strings always commute or anticommute. If they anticommute and a vector $|\psi\rangle$ were stabilized by both, then $PQ|\psi\rangle=|\psi\rangle$ and $QP|\psi\rangle=|\psi\rangle$, contradicting $PQ=-QP$. Their common [stabilizer subspace](../../../quantum-circuit.md#stabilizer-subspace) is consequently the zero subspace $\{0\}$.

<h3 id="2/v">v</h3>

↑ **Parent:** [2](#2)

<h4 id="2/v/solution">Solution</h4>

↑ **Parent:** [V](#2/v)

The group average

$$
\Pi_G=\frac1{|G|}\sum_{P\in G}P
$$

is Hermitian. In its square, every $R\in G$ occurs exactly $|G|$ times among products $PQ$, and therefore $\Pi_G^2=\Pi_G$. Moreover $g\Pi_G=\Pi_G$ for every $g\in G$, so its image lies in the [stabilizer subspace](../../../quantum-circuit.md#stabilizer-subspace) $V_G$, while $\Pi_G|\psi\rangle=|\psi\rangle$ for every $|\psi\rangle\in V_G$. Thus $\Pi_G$ is the [orthogonal projector](../../../hilbert-space.md#orthogonal-projection) onto $V_G$. If $g_1,\ldots,g_l$ are independent generators, expanding the product chooses each element of $G$ exactly once and gives the [stabilizer-projector formula](../../../quantum-circuit.md#stabilizer-projector-formula)

$$
\boxed{\Pi_G=\prod_{i=1}^l\frac{I+g_i}{2}}.
$$

## 3

↑ **Parent:** [Paper 324](paper-324.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/i">i</h4>

↑ **Parent:** [A](#3/a)

<h5 id="3/a/i/solution">Solution</h5>

↑ **Parent:** [I](#3/a/i)

Write the [local Hamiltonian](../../../quantum-theory.md#local-hamiltonian) as $H=\sum_{j=1}^mh_j$. Since its terms commute, their [matrix exponentials](../../../linear-operator-theory.md#matrix-exponential) factor exactly:

$$
e^{-iHt}=\prod_{j=1}^me^{-ih_jt}.
$$

Each factor acts on at most two qubits and can be compiled over a fixed [universal quantum gate set](../../../quantum-circuit.md#universal-quantum-gate-set) to [operator norm](../../../continuous-dual-space.md#operator-norm) error at most $\varepsilon/m$. The [telescoping bound for products of operators](../../../continuous-dual-space.md#telescoping-bound-for-products-of-operators) then bounds the total error by the sum of the factor errors, at most $\varepsilon$. Because $m$ is polynomial in $n$ and the [Solovay--Kitaev theorem](../../../quantum-circuit.md#solovay-kitaev-theorem) gives gate count polynomial in $\log(m/\varepsilon)$ for each fixed-dimensional factor, this is an efficient [commuting local Hamiltonian simulation](../../../quantum-theory.md#commuting-local-hamiltonian-simulation). Finally, the [eigenvalue equation](../../../linear-operator-theory.md#eigenvalue-equation) $H|\Psi\rangle=\lambda|\Psi\rangle$ implies

$$
U(t)|\Psi\rangle=e^{-i\lambda t}|\Psi\rangle,
$$

so $|\Psi\rangle$ remains an [eigenstate](../../../quantum-mechanics.md#eigenstate) and its eigenvalue is $e^{-i\lambda t}$.

<h4 id="3/a/ii">ii</h4>

↑ **Parent:** [A](#3/a)

<h5 id="3/a/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#3/a/ii)

Apply [exact quantum phase estimation](../../../quantum-theory.md#exact-quantum-phase-estimation) to $U(t)$ with the supplied [eigenstate](../../../quantum-mechanics.md#eigenstate) $|\Psi\rangle$. Since

$$
U(t)|\Psi\rangle=e^{2\pi i\phi}|\Psi\rangle,
\qquad
\phi=-\frac{\lambda t}{2\pi}\pmod1,
$$

the promise that the phase has an $N$-bit representation makes an $N$-qubit control register recover $\phi$ exactly. Multiplying by $-2\pi$ modulo $2\pi$ gives $\lambda t\bmod2\pi$. Equivalently, phase estimation may be run on $U(t)^\dagger$, whose eigenphase is $\lambda t/(2\pi)$ modulo one.

<h4 id="3/a/iii">iii</h4>

↑ **Parent:** [A](#3/a)

<h5 id="3/a/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#3/a/iii)

Let $A=X\otimes X\otimes I$ and $B=Z\otimes I\otimes Z$. The two [Pauli operators](../../../quantum-circuit.md#pauli-operator) anticommute because their local factors anticommute at exactly one qubit. Since $A^2=B^2=I$, the mixed terms cancel and

$$
H^2=(5A-4B)^2=25I+16I=41I,
\qquad
H^4=1681I.
$$

This is a scalar, or $0$-local, Hamiltonian, so the smallest value is $\boxed{k=0}$.

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/i">i</h4>

↑ **Parent:** [B](#3/b)

<h5 id="3/b/i/solution">Solution</h5>

↑ **Parent:** [I](#3/b/i)

The vertices $v_2,v_3,v_5$ form a [triangle in a graph](../../../graph.md#triangle-in-a-graph), so every [cut of a graph](../../../graph-theory.md#cut-graph-theory) leaves at least one of their three edges uncut. Hence the cut size is at most four. Take

$$
S_1=\{v_2,v_5\},
\qquad
S_2=\{v_1,v_3,v_4\}.
$$

The crossing edges are $(1,5),(2,3),(3,5),(4,5)$, so $C=4$. The upper bound is attained and this is a [maximum cut](../../../graph-theory.md#maximum-cut).

<h4 id="3/b/ii">ii</h4>

↑ **Parent:** [B](#3/b)

<h5 id="3/b/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#3/b/ii)

Since $\hat x_i=P_{1,i}$ and $I-\hat x_i=P_{0,i}$, the [diagonal Hamiltonian](../../../quantum-theory.md#diagonal-hamiltonian) is

$$
H=-\sum_{(i,j)\in E}\left(P_{1,i}P_{0,j}+P_{0,i}P_{1,j}\right),
$$

with the identity on every unlisted qubit. Each [computational-basis state](../../../quantum-theory.md#computational-basis-state) is an [eigenstate](../../../quantum-mechanics.md#eigenstate), and its eigenvalue is minus the cost of the corresponding cut. Part i supplies cost four, while the assumed bound $|\lambda_{\min}|\leq4$ rules out a lower energy. Thus the [ground-state energy](../../../quantum-mechanics.md#ground-state-energy) is $-4$. For the assignment $(x_1,x_2,x_3,x_4,x_5)=(0,1,0,0,1)$, one [ground state](../../../quantum-mechanics.md#ground-state) is

$$
\boxed{|\psi\rangle=|01001\rangle}.
$$

Its bitwise complement $|10110\rangle$ is another ground state, as are the basis states corresponding to the other maximum cuts.

## 4

↑ **Parent:** [Paper 324](paper-324.md)

<h3 id="4/a">a</h3>

↑ **Parent:** [4](#4)

<h4 id="4/a/i">i</h4>

↑ **Parent:** [A](#4/a)

<h5 id="4/a/i/solution">Solution</h5>

↑ **Parent:** [I](#4/a/i)

For a [finite abelian group](../../../group.md#finite-abelian-group) $G$ and its [character group of a finite abelian group](../../../group.md#character-group-of-a-finite-abelian-group) $\widehat G$, the [quantum Fourier transform over a finite abelian group](../../../quantum-theory.md#quantum-fourier-transform-over-a-finite-abelian-group) is

$$
\operatorname{QFT}_G|g\rangle
=\frac1{\sqrt{|G|}}\sum_{\chi\in\widehat G}\chi(g)|\chi\rangle.
$$

Replacing $\chi(g)$ by its complex conjugate gives the equally common inverse-transform convention.

<h4 id="4/a/ii">ii</h4>

↑ **Parent:** [A](#4/a)

<h5 id="4/a/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#4/a/ii)

The relation $z^{2^n}=1$ makes $z$ a [root of unity](../../../algebra.md#root-of-unity), so $|z|=1$ and normalization gives $T=2^{n/2}$. Write the [binary expansion](../../../arithmetic.md#binary-expansion) $y=\sum_{j=0}^{n-1}2^jy_j$. Then $z^y=\prod_j(z^{2^j})^{y_j}$, and hence

$$
|\phi\rangle
=\bigotimes_{j=0}^{n-1}
\frac{|0\rangle+z^{2^j}|1\rangle}{\sqrt2},
$$

up to the convention for ordering the binary digits. This explicit [tensor product](../../../linear-algebra.md#tensor-product) of one-qubit states proves that $|\phi\rangle$ is a [product state](../../../bell-state.md#product-state).

<h3 id="4/b">b</h3>

↑ **Parent:** [4](#4)

<h4 id="4/b/i">i</h4>

↑ **Parent:** [B](#4/b)

<h5 id="4/b/i/solution">Solution</h5>

↑ **Parent:** [I](#4/b/i)

In the [hidden subgroup problem](../../../quantum-theory.md#hidden-subgroup-problem), an oracle gives a function $f:G\to X$ that is constant on every left [coset](../../../group-theory.md#coset) of an unknown subgroup $H\leq G$ and takes distinct values on distinct cosets. The task is to determine $H$.

<h4 id="4/b/ii">ii</h4>

↑ **Parent:** [B](#4/b)

<h5 id="4/b/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#4/b/ii)

Regard bit strings as the [elementary abelian group](../../../group.md#elementary-abelian-group) $G=(\mathbb Z_2)^n$ under [bitwise exclusive or](../../../computer-science.md#exclusive-or). The promise says

$$
f(x)=f(y)
\quad\Longleftrightarrow\quad
x\mathbin\oplus y\in H,
\qquad
H=\{0^n,p\}.
$$

**Thus $f$ is constant exactly on the cosets of $H$ and distinct between them. Determining the hidden subgroup determines its nonzero element $p$, so this is [Simon's problem](../../../quantum-theory.md#simon-s-problem) as an instance of the [hidden subgroup problem](../../../quantum-theory.md#hidden-subgroup-problem).**

<h4 id="4/b/iii">iii</h4>

↑ **Parent:** [B](#4/b)

<h5 id="4/b/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#4/b/iii)

Prepare $2^{-n/2}\sum_x|x\rangle|0^n\rangle$, query the oracle, and measure or discard the output register. For $p\ne0$, the input register becomes the [coset state](../../../quantum-theory.md#coset-state)

$$
\frac{|x\rangle+|x\mathbin\oplus p\rangle}{\sqrt2}.
$$

Apply $H^{\otimes n}$, the [quantum Fourier transform](../../../quantum-theory.md#quantum-fourier-transform) over $(\mathbb Z_2)^n$. The two amplitudes interfere destructively unless the [binary inner product](../../../linear-algebra.md#binary-inner-product) satisfies

$$
y\mathbin\cdot p=0\pmod2,
$$

and every vector in this orthogonal subspace is sampled uniformly. Repeat until $n-1$ independent equations have been collected, then use [Gaussian elimination](../../../numerical-analysis.md#gaussian-elimination) over $\mathbb F_2$ to find their one-dimensional [null space](../../../linear-algebra.md#kernel-of-a-linear-map); its nonzero vector is $p$. This is [Simon's algorithm](../../../quantum-theory.md#simon-s-algorithm). It uses $O(n)$ oracle queries with high probability and polynomial classical work. When $p=0^n$, the function is injective and the samples eventually span all of $(\mathbb F_2)^n$, which distinguishes that case with arbitrarily high probability.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2022](../../2022.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
