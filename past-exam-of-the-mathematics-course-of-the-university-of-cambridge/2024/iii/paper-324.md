# Paper 324

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2024/Paper_324.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2024/Paper_324.pdf)

**Table of contents**

- [1](#1)
  - [a](#1/a)
    - [Solution](#1/a/solution)
  - [b](#1/b)
    - [Solution](#1/b/solution)
  - [c](#1/c)
    - [i](#1/c/i)
      - [Solution](#1/c/i/solution)
    - [ii](#1/c/ii)
      - [Solution](#1/c/ii/solution)
    - [iii](#1/c/iii)
      - [Solution](#1/c/iii/solution)
    - [iv](#1/c/iv)
      - [Solution](#1/c/iv/solution)
- [2](#2)
  - [a](#2/a)
    - [Solution](#2/a/solution)
  - [b](#2/b)
    - [i](#2/b/i)
      - [Solution](#2/b/i/solution)
    - [ii](#2/b/ii)
      - [Solution](#2/b/ii/solution)
    - [iii](#2/b/iii)
      - [Solution](#2/b/iii/solution)
    - [iv](#2/b/iv)
      - [Solution](#2/b/iv/solution)
- [3](#3)
  - [a](#3/a)
    - [Solution](#3/a/solution)
  - [b](#3/b)
    - [Solution](#3/b/solution)
  - [c](#3/c)
    - [Solution](#3/c/solution)
- [4](#4)
  - [a](#4/a)
    - [Solution](#4/a/solution)
  - [b](#4/b)
    - [Solution](#4/b/solution)
  - [c](#4/c)
    - [Solution](#4/c/solution)

## 1

↑ **Parent:** [Paper 324](paper-324.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

The [hidden subgroup problem](../../../quantum-theory.md#hidden-subgroup-problem) for a [group](../../../group.md) $G$ is specified by an oracle $f:G\to S$ that hides an unknown [subgroup](../../../group.md#subgroup) $H\leq G$: it is constant on each left [coset](../../../group-theory.md#coset) of $H$ and takes distinct values on distinct cosets. The task is to determine $H$, usually by finding a [generating set](../../../set.md#generating-set) for it.

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

A shift-invariant basis is a common [eigenbasis](../../../linear-operator-theory.md#eigenbasis) of all [cyclic shift operators](../../../quantum-theory.md#cyclic-shift-operator) $U(\gamma)$. For the displayed Fourier states, [orthonormality](../../../linear-algebra.md#orthonormal-set) follows from the [root-of-unity filter](../../../algebra.md#root-of-unity-filter):

$$
\langle\xi_\alpha|\xi_{\alpha'}\rangle
=\frac1N\sum_{\beta\in\mathbb Z_N}
\omega^{(\alpha-\alpha')\beta}
=\delta_{\alpha,\alpha'}.
$$

There are $N$ vectors in this [orthonormal set](../../../linear-algebra.md#orthonormal-set) in the $N$-dimensional [Hilbert space](../../../hilbert-space.md), so they form a [basis](../../../vector-space.md#basis). Reindexing the finite sum gives

$$
\begin{aligned}
U(\gamma)|\xi_\alpha\rangle
&=\frac1{\sqrt N}\sum_\beta
\omega^{-\alpha\beta}|\beta+\gamma\rangle\\
&=\omega^{\alpha\gamma}|\xi_\alpha\rangle.
\end{aligned}
$$

**Thus every $|\xi_\alpha\rangle$ is simultaneously an [eigenvector](../../../linear-operator-theory.md#eigenvector) of every shift, with [eigenvalue](../../../linear-operator-theory.md#eigenvalue) $\omega^{\alpha\gamma}$ for $U(\gamma)$.**

<h3 id="1/c">c</h3>

↑ **Parent:** [1](#1)

<h4 id="1/c/i">i</h4>

↑ **Parent:** [C](#1/c)

<h5 id="1/c/i/solution">Solution</h5>

↑ **Parent:** [I](#1/c/i)

For each fixed $\alpha$, right multiplication by $x^{-\alpha}$ is a [bijection](../../../function.md#bijection) of $G$, whose inverse is right multiplication by $x^\alpha$. Therefore $D_x$ permutes the displayed [orthonormal basis](../../../linear-algebra.md#orthonormal-basis) of the [tensor-product space](../../../linear-algebra.md#tensor-product). It is consequently a [unitary operator](../../../vector-space.md#unitary-operator), with

$$
\boxed{D_x^\dagger|\alpha\rangle|y\rangle
=|\alpha\rangle|yx^\alpha\rangle.}
$$

<h4 id="1/c/ii">ii</h4>

↑ **Parent:** [C](#1/c)

<h5 id="1/c/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#1/c/ii)

Write $x=g^\eta$. Applying $D_x$ and then changing the summation variable from $k$ to $\ell=k-\alpha\eta$ gives

$$
\begin{aligned}
D_x|\alpha\rangle|\chi_\beta\rangle
&=\frac1{\sqrt N}\sum_k
\omega^{\beta k}|\alpha\rangle|g^{k-\alpha\eta}\rangle\\
&=\omega^{\alpha\beta\eta}
|\alpha\rangle|\chi_\beta\rangle.
\end{aligned}
$$

Hence this state is an [eigenvector](../../../linear-operator-theory.md#eigenvector) of $D_x$ with [eigenvalue](../../../linear-operator-theory.md#eigenvalue) $\boxed{\omega^{\alpha\beta\eta}}$.

<h4 id="1/c/iii">iii</h4>

↑ **Parent:** [C](#1/c)

<h5 id="1/c/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#1/c/iii)

Using the convention

$$
F_N|\alpha\rangle=\frac1{\sqrt N}
\sum_j\omega^{\alpha j}|j\rangle,
$$

part (ii) applies the extra [phase](../../../quantum-mechanics.md#quantum-phase) $\omega^{j\beta\eta}$ to term $j$. The resulting first register is the [quantum Fourier transform](../../../quantum-theory.md#quantum-fourier-transform) of $|\alpha+\beta\eta\bmod N\rangle$. Applying its inverse therefore produces

$$
\boxed{|\alpha+\beta\eta\bmod N\rangle
|\chi_\beta\rangle}.
$$

<h4 id="1/c/iv">iv</h4>

↑ **Parent:** [C](#1/c)

<h5 id="1/c/iv/solution">Solution</h5>

↑ **Parent:** [Iv](#1/c/iv)

Choose $\alpha=0$ and prepare $|\chi_1\rangle$. The circuit from part (iii) returns

$$
|\eta\rangle|\chi_1\rangle,
$$

so a [quantum measurement in the computational basis](../../../quantum-theory.md#quantum-measurement-in-the-computational-basis) of the first register reveals the [discrete logarithm](../../../coding-theory.md#discrete-logarithm-problem) $\eta$ exactly. More generally, any $\beta$ that is [invertible modulo $N$](../../../algebra.md#multiplicative-group-of-integers-modulo-n) returns $\beta\eta\bmod N$, from which $\eta$ follows by multiplication by the [modular inverse](../../../number-theory.md#modular-multiplicative-inverse) of $\beta$.

## 2

↑ **Parent:** [Paper 324](paper-324.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

Let $\Pi_{\mathcal G}$ be the [orthogonal projection](../../../hilbert-space.md#orthogonal-projection) onto the good [linear subspace](../../../vector-space.md#vector-subspace) and write

$$
|\psi\rangle
=\sin\theta\,|\psi_G\rangle
+\cos\theta\,|\psi_B\rangle,
\qquad
\sin^2\theta=\langle\psi|\Pi_{\mathcal G}|\psi\rangle,
$$

where the two displayed states are normalized projections into $\mathcal G$ and $\mathcal G^\perp$. Define the [reflections](../../../linear-algebra.md#reflection-in-a-hyperplane)

$$
R_G=I-2\Pi_{\mathcal G},
\qquad
R_\psi=2|\psi\rangle\langle\psi|-I.
$$

The [amplitude amplification](../../../quantum-theory.md#amplitude-amplification) iterate $Q=R_\psi R_G$ preserves the good-bad plane, and its $k$th iterate satisfies

$$
Q^k|\psi\rangle
=\sin((2k+1)\theta)|\psi_G\rangle
+\cos((2k+1)\theta)|\psi_B\rangle.
$$

**Thus repeated reflections rotate amplitude toward the good subspace, reaching constant success probability after $O(1/\sin\theta)$ iterations.**

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/i">i</h4>

↑ **Parent:** [B](#2/b)

<h5 id="2/b/i/solution">Solution</h5>

↑ **Parent:** [I](#2/b/i)

In the ordered [orthonormal basis](../../../linear-algebra.md#orthonormal-basis)

$$
|b\rangle=|\psi_0\rangle|0\rangle,
\qquad
|g\rangle=|\psi_1\rangle|1\rangle
$$

of $\mathcal S$, the [Pauli Z gate](../../../quantum-theory.md#pauli-z-gate) acts as

$$
I_{m-1}\otimes Z
=\begin{pmatrix}1&0\\0&-1\end{pmatrix}
=I_{\mathcal S}-2|g\rangle\langle g|.
$$

It fixes the line $|g\rangle^\perp\cap\mathcal S$ and negates $|g\rangle$, so it is the [reflection in a hyperplane](../../../linear-algebra.md#reflection-in-a-hyperplane) orthogonal to the good state.

<h4 id="2/b/ii">ii</h4>

↑ **Parent:** [B](#2/b)

<h5 id="2/b/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#2/b/ii)

Set $|\Psi\rangle=U|0^m\rangle$. [Unitary conjugation](../../../vector-space.md#unitary-conjugation) gives

$$
UR_0U^\dagger
=U(I-2|0^m\rangle\langle0^m|)U^\dagger
=I-2|\Psi\rangle\langle\Psi|.
$$

The operator negates $|\Psi\rangle$ and fixes every vector in $\mathcal S$ [orthogonal](../../../linear-algebra.md#orthogonal-vectors) to it. It is therefore the [reflection in a hyperplane](../../../linear-algebra.md#reflection-in-a-hyperplane) whose normal is $|\Psi\rangle$.

<h4 id="2/b/iii">iii</h4>

↑ **Parent:** [B](#2/b)

<h5 id="2/b/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#2/b/iii)

Put $\sqrt p=\sin\theta$ and $\sqrt{1-p}=\cos\theta$, where $0<\theta<\pi/2$. In the ordered basis $(|b\rangle,|g\rangle)$, the product of the two reflections is

$$
(UR_0U^\dagger)(I_{m-1}\otimes Z)
=-\begin{pmatrix}
\cos2\theta&-\sin2\theta\\
\sin2\theta&\cos2\theta
\end{pmatrix}.
$$

The leading minus sign is a physically irrelevant [global phase](../../../quantum-mechanics.md#global-phase). The remaining [rotation matrix](../../../linear-algebra.md#rotation-matrix) rotates the good-bad plane through $2\theta$, where

$$
\boxed{\sin^2\theta=p}.
$$

Equivalently, one iterate changes the initial angle $\theta$ to $3\theta$.

<h4 id="2/b/iv">iv</h4>

↑ **Parent:** [B](#2/b)

<h5 id="2/b/iv/solution">Solution</h5>

↑ **Parent:** [Iv](#2/b/iv)

Attach a [quantum ancilla](../../../quantum-information-theory.md#quantum-ancilla) prepared with amplitude

$$
c=\frac1{2\sqrt p}
$$

on $|1\rangle$; this is possible because $p>1/4$. Mark a state as good only when both the original success qubit and this ancilla equal one. The enlarged state's good probability is $pc^2=1/4$, so its good amplitude is $1/2=\sin(\pi/6)$. One [amplitude amplification](../../../quantum-theory.md#amplitude-amplification) iteration rotates the angle from $\pi/6$ to $3\pi/6=\pi/2$. It therefore prepares $|\psi_1\rangle$ exactly, after which the flag and ancillary qubits may be discarded. This is an instance of [exact amplitude amplification](../../../quantum-theory.md#exact-amplitude-amplification).

## 3

↑ **Parent:** [Paper 324](paper-324.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

The [spectral norm](../../../continuous-dual-space.md#matrix-2-norm) of an operator $O$ is the induced [operator norm](../../../continuous-dual-space.md#operator-norm)

$$
\|O\|=\sup_{\|\psi\|=1}\|O\psi\|.
$$

Every [Pauli X gate](../../../quantum-theory.md#pauli-x-gate) $X_i$ is [unitary](../../../vector-space.md#unitary-operator), so $\|X_i\|=1$. The [triangle inequality](../../../topological-analysis.md#triangle-inequality) for the norm therefore gives

$$
\boxed{\|J_X\|
\leq\sum_{i=1}^n\|X_i\|=n}.
$$

In fact equality holds, as the product of $+1$ [eigenvectors](../../../linear-operator-theory.md#eigenvector) of the $X_i$ has eigenvalue $n$ under $J_X$.

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

The operators $X_i$ act on different [qubits](../../../quantum-mechanics.md#qubit) and therefore [commute](../../../vector-space.md#commuting-operators), so

$$
e^{-itJ_X}=\prod_{i=1}^ne^{-itX_i}.
$$

Since $X=HZH$,

$$
e^{-itX}=H e^{-itZ}H
=e^{-it}H\operatorname{diag}(1,e^{2it})H.
$$

The scalar $e^{-it}$ is a [global phase](../../../quantum-mechanics.md#global-phase). Thus each factor uses two [Hadamard gates](../../../quantum-theory.md#hadamard-gate) and one [phase gate](../../../quantum-theory.md#phase-gate), and applying the factors in parallel or sequentially gives an exact [quantum circuit](../../../quantum-circuit.md) of $\boxed{3n}$ elementary gates.

<h3 id="3/c">c</h3>

↑ **Parent:** [3](#3)

<h4 id="3/c/solution">Solution</h4>

↑ **Parent:** [C](#3/c)

Each summand of $J_X$ acts on one [qubit](../../../quantum-mechanics.md#qubit), while each summand $Z_iZ_j$ of $J_Z$ acts on two. Therefore $J=J_X+J_Z$ is a [2-local Hamiltonian](../../../quantum-theory.md#k-local-hamiltonian). We have

$$
\|J_X\|=O(n),
\qquad
\|J_Z\|\leq\binom n2=O(n^2).
$$

Split $t$ into $r$ steps of length $\delta=t/r$ and use the [second-order product formula](../../../quantum-theory.md#second-order-product-formula)

$$
S_2(\delta)=
e^{-i\delta J_X/2}e^{-i\delta J_Z}e^{-i\delta J_X/2}.
$$

For one step, $\Lambda=O(\delta n^2)$ in the stated estimate, so the [spectral-norm error](../../../continuous-dual-space.md#matrix-2-norm) is $O(\delta^3n^6)$. The error bound for a product of [unitary operators](../../../vector-space.md#unitary-operator) makes the total error

$$
O(r\delta^3n^6)=O\left(\frac{n^6t^3}{r^2}\right).
$$

It is therefore enough to choose

$$
r=O\left(\frac{n^3t^{3/2}}{\sqrt\epsilon}\right),
$$

with $r$ also large enough that the small-step estimate applies.

All $Z_iZ_j$ terms [commute](../../../vector-space.md#commuting-operators). A factor $e^{-i\delta Z_iZ_j}$ uses a constant-size circuit of two [controlled-NOT gates](../../../quantum-theory.md#controlled-not-gate) and one [phase gate](../../../quantum-theory.md#phase-gate), up to a [global phase](../../../quantum-mechanics.md#global-phase), so one product-formula step costs $O(n^2)$ gates. The complete [Hamiltonian simulation](../../../quantum-theory.md#hamiltonian-simulation) consequently has size

$$
\boxed{O\left(\frac{n^5t^{3/2}}{\sqrt\epsilon}\right)}.
$$

## 4

↑ **Parent:** [Paper 324](paper-324.md)

<h3 id="4/a">a</h3>

↑ **Parent:** [4](#4)

<h4 id="4/a/solution">Solution</h4>

↑ **Parent:** [A](#4/a)

First construct a [controlled unitary gate](../../../quantum-theory.md#controlled-unitary-gate) from the uncontrolled oracle. Keep the supplied $|v_0\rangle$ in a reference register. Controlled on an extra qubit, swap the data and reference registers, query $U$ on the register that contains $|v_0\rangle$ in one branch, and swap back. Because $U|v_0\rangle=|v_0\rangle$, that branch is unchanged, while the other branch acquires $U$ on the data. Reversing the control convention with [Pauli X gates](../../../quantum-theory.md#pauli-x-gate) gives controlled-$U$. The reference state is returned unchanged, and each use costs one query to $U$ and $O(n)$ [controlled-SWAP gates](../../../quantum-theory.md#fredkin-gate).

Expand $|b\rangle=\sum_jb_j|v_j\rangle$ in an [eigenbasis](../../../linear-operator-theory.md#eigenbasis) of $U$. [Exact quantum phase estimation](../../../quantum-theory.md#exact-quantum-phase-estimation) with an $m$-qubit phase register produces

$$
\sum_jb_j|c_j\rangle|v_j\rangle,
\qquad
U|v_j\rangle=e^{2\pi ic_j/2^m}|v_j\rangle.
$$

Apply the available [phase gates](../../../quantum-theory.md#phase-gate), controlled by the corresponding bits of $c_j$, to multiply branch $j$ by

$$
e^{-2\pi ic_j/2^m}=\lambda_j^{-1}.
$$

Then reverse phase estimation. Although no $U^\dagger$ oracle was supplied, every eigenvalue obeys $\lambda_j^{2^m}=1$, so $U^{-q}=U^{2^m-q}$. The inverse controlled powers can therefore be implemented with forward calls to $U$. Since $2^m=\operatorname{poly}(n)$, phase estimation and its inverse use only $\operatorname{poly}(n)$ queries. The phase register returns to $|0^m\rangle$, while the data register is

$$
\sum_jb_j\lambda_j^{-1}|v_j\rangle
=\boxed{U^\dagger|b\rangle}.
$$

As a direct check, the same spectral promise implies $U^\dagger=U^{2^m-1}$.

<h3 id="4/b">b</h3>

↑ **Parent:** [4](#4)

<h4 id="4/b/solution">Solution</h4>

↑ **Parent:** [B](#4/b)

The [HHL algorithm](../../../quantum-theory.md#hhl-algorithm) requires coherent, efficient and repeatable preparation of the normalized state $|b\rangle$, normally through a known preparation circuit and its inverse; possession of a single unknown physical specimen does not supply that access. The component of $b$ on any discarded or unresolved small-eigenvalue subspace must also be negligible. Here $U$ is a [unitary operator](../../../vector-space.md#unitary-operator), so it is invertible and all its [singular values](../../../linear-algebra.md#singular-value) equal one, giving [condition number](../../../linear-algebra.md#condition-number) $\kappa=1$.

Standard HHL is stated for a [Hermitian matrix](../../../hilbert-space.md#hermitian-operator) with an efficient sparse-access or [block encoding](../../../quantum-theory.md#block-encoding) oracle. A non-Hermitian $U$ can be embedded in the Hermitian block matrix

$$
\begin{pmatrix}0&U\\U^\dagger&0\end{pmatrix};
$$

part (a) supplies efficient access to $U^\dagger$. With inverse-polynomial target precision, $m=O(\log n)$ phase bits, and an efficient preparation oracle for $|b\rangle$, the runtime is $\operatorname{poly}(n)$. The output is the normalized [quantum state](../../../quantum-mechanics.md#quantum-state) proportional to the solution $x$, rather than a classical list of all its amplitudes.

<h3 id="4/c">c</h3>

↑ **Parent:** [4](#4)

<h4 id="4/c/solution">Solution</h4>

↑ **Parent:** [C](#4/c)

Implement the assumed efficient classical algorithm for $x\mapsto\theta_x$ as a [reversible circuit](../../../computer-science.md#reversible-circuit). On input $|x\rangle|0^s\rangle$, it computes an $O(m)$-bit [binary expansion](../../../arithmetic.md#binary-expansion) of the angle in a work register using $\operatorname{poly}(m)$ [Toffoli gates](../../../quantum-theory.md#toffoli-gate) and elementary reversible gates. Write the computed angle as a sum of binary-weighted angles. For each angle bit, apply the corresponding controlled single-qubit $R_y$ rotation to the target. These rotations have the same axis, so their angles add and produce

$$
|x\rangle|\widetilde\theta_x\rangle
(\cos\theta_x|0\rangle+\sin\theta_x|1\rangle).
$$

Finally apply [uncomputation](../../../quantum-theory.md#uncomputation) to erase the work register. Each [Toffoli gate](../../../quantum-theory.md#toffoli-gate) and controlled rotation has a constant-size decomposition into one- and two-qubit gates when arbitrary one-qubit rotations are available. Ignoring the stipulated precision costs, the resulting circuit has size $\operatorname{poly}(m)$ and returns every [quantum ancilla](../../../quantum-information-theory.md#quantum-ancilla) to zero.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2024](../../2024.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
