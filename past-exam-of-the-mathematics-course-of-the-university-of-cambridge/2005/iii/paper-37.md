# Paper 37

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2005/Paper37.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2005/Paper37.pdf)

**Table of contents**

- [1](#1)
  - [a](#1/a)
    - [Solution](#1/a/solution)
  - [b](#1/b)
    - [Solution](#1/b/solution)
- [2](#2)
  - [a](#2/a)
    - [Solution](#2/a/solution)
  - [b](#2/b)
    - [i](#2/b/i)
      - [Solution](#2/b/i/solution)
    - [ii](#2/b/ii)
      - [Solution](#2/b/ii/solution)
- [3](#3)
  - [a](#3/a)
    - [Solution](#3/a/solution)
  - [b](#3/b)
    - [Solution](#3/b/solution)
- [4](#4)
  - [a](#4/a)
    - [Solution](#4/a/solution)
  - [b](#4/b)
    - [Solution](#4/b/solution)
- [5](#5)
  - [a](#5/a)
    - [Solution](#5/a/solution)
  - [b](#5/b)
    - [Solution](#5/b/solution)

## 1

↑ **Parent:** [Paper 37](paper-37.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

Use base-two logarithms for [Von Neumann entropy](../../../von-neumann-entropy.md), so the units are [bits](../../../information-theory.md#bit), and adopt $0\log_2 0=0$. All systems here may be taken finite-dimensional; the entropy arguments also apply when the displayed [Von Neumann entropies](../../../von-neumann-entropy.md) are finite. The [density operator](../../../quantum-theory.md#density-matrix) of the joint [pure state](../../../quantum-theory.md#pure-state) is $\rho_{AB}=|\Psi_{AB}\rangle\langle\Psi_{AB}|$. It is a rank-one [orthogonal projector](../../../hilbert-space.md#orthogonal-projection), whose only nonzero [eigenvalue](../../../linear-operator-theory.md#eigenvalue) is one. Consequently

$$
\boxed{S(A,B)=-\operatorname{Tr}(\rho_{AB}\log_2\rho_{AB})=0.}
$$

The [reduced density matrices](../../../bell-state.md#reduced-density-matrix) are $\rho_A=\operatorname{Tr}_B\rho_{AB}$ and $\rho_B=\operatorname{Tr}_A\rho_{AB}$. The [quantum conditional entropy](../../../von-neumann-entropy.md#quantum-conditional-entropy) is defined by the entropy difference

$$
S(B|A):=S(\rho_{AB})-S(\rho_A).
$$

For the [pure state](../../../quantum-theory.md#pure-state) under consideration this becomes $S(B|A)=-S(\rho_A)$. To determine when it is negative, write the [Schmidt decomposition](../../../von-neumann-entropy.md#schmidt-decomposition)

$$
|\Psi_{AB}\rangle=\sum_{j=1}^r\sqrt{\lambda_j}|a_j\rangle|b_j\rangle,
\qquad \lambda_j>0,\qquad\sum_j\lambda_j=1.
$$

The [eigenvalues](../../../linear-operator-theory.md#eigenvalue) of $\rho_A$ are the $\lambda_j$, together with possible zeros. Each contribution $-\lambda_j\log_2\lambda_j$ is nonnegative, and their sum vanishes exactly when one [eigenvalue](../../../linear-operator-theory.md#eigenvalue) equals one. Equivalently the [Schmidt rank](../../../von-neumann-entropy.md#schmidt-rank) is one and $|\Psi_{AB}\rangle$ is a [product state](../../../bell-state.md#product-state). If the [pure state](../../../quantum-theory.md#pure-state) is [entangled](../../../bell-state.md#entangled-state), then $r\geq2$, every nonzero [eigenvalue](../../../linear-operator-theory.md#eigenvalue) is strictly below one, and the [Von Neumann entropy](../../../von-neumann-entropy.md) is strictly positive. Thus the [pure-state negative conditional entropy criterion](../../../von-neumann-entropy.md#pure-state-negative-conditional-entropy-criterion) gives

$$
\boxed{S(B|A)<0\quad\Longleftrightarrow\quad|\Psi_{AB}\rangle\text{ is entangled}.}
$$

The purity assumption matters: for mixed [density operators](../../../quantum-theory.md#density-matrix), negative [quantum conditional entropy](../../../von-neumann-entropy.md#quantum-conditional-entropy) is not necessary for [entanglement](../../../bell-state.md#entangled-state).

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

Let a [density operator](../../../quantum-theory.md#density-matrix) on a [Hilbert space](../../../hilbert-space.md) $\mathcal H_S$ have the [spectral decomposition](../../../linear-operator-theory.md#spectral-decomposition)

$$
\rho_S=\sum_{j=1}^r\lambda_j|j\rangle_S\langle j|,
\qquad\lambda_j>0,\qquad\sum_j\lambda_j=1.
$$

Introduce an auxiliary [Hilbert space](../../../hilbert-space.md) $\mathcal H_R$ with an [orthonormal basis](../../../linear-algebra.md#orthonormal-basis) containing $r$ vectors $|j\rangle_R$, and set

$$
|\Omega\rangle_{SR}=\sum_{j=1}^r\sqrt{\lambda_j}|j\rangle_S|j\rangle_R.
$$

This vector has norm one. Its [partial trace](../../../quantum-theory.md#partial-trace) is

$$
\operatorname{Tr}_R|\Omega\rangle\langle\Omega|
=\sum_{j,k}\sqrt{\lambda_j\lambda_k}|j\rangle_S\langle k|\langle k|j\rangle_R
=\rho_S.
$$

This explicitly constructs a [purification of a density operator](../../../quantum-theory.md#purification-of-a-density-operator). The same construction works for an arbitrary trace-class [density operator](../../../quantum-theory.md#density-matrix): its nonzero [eigenvalues](../../../linear-operator-theory.md#eigenvalue) form a finite or countable summable family, and the displayed vector converges in the [Hilbert space](../../../hilbert-space.md) norm. The entropy inequality below is understood with finite [Von Neumann entropies](../../../von-neumann-entropy.md), avoiding undefined differences of infinities.

Apply this construction with $S=AB$ to obtain a joint [pure state](../../../quantum-theory.md#pure-state) on $ABC$. The [Schmidt decomposition](../../../von-neumann-entropy.md#schmidt-decomposition) across $AB:C$, $A:BC$ and $B:AC$ respectively gives

$$
S(AB)=S(C),\qquad S(A)=S(BC),\qquad S(B)=S(AC).
$$

Now apply [Subadditivity of Von Neumann entropy](../../../von-neumann-entropy.md#subadditivity-of-von-neumann-entropy) to the [reduced density matrices](../../../bell-state.md#reduced-density-matrix) on $BC$ and $AC$:

$$
S(A)=S(BC)\leq S(B)+S(C),\qquad
S(B)=S(AC)\leq S(A)+S(C).
$$

These inequalities say $S(A)-S(B)\leq S(C)$ and $S(B)-S(A)\leq S(C)$. Replacing $S(C)$ by $S(AB)$ proves the [Araki–Lieb inequality](../../../von-neumann-entropy.md#araki-lieb-inequality):

$$
\boxed{|S(A)-S(B)|\leq S(A,B).}
$$

The subadditivity used here concerns the actual reduced [density operators](../../../quantum-theory.md#density-matrix), rather than statistical independence. In particular it follows from [nonnegativity of quantum relative entropy](../../../von-neumann-entropy.md#nonnegativity-of-quantum-relative-entropy), since

$$
D(\rho_{BC}\Vert\rho_B\otimes\rho_C)
=S(\rho_B)+S(\rho_C)-S(\rho_{BC})\geq0,
$$

and similarly for $AC$. Thus no independence assumption on the [purification of a density operator](../../../quantum-theory.md#purification-of-a-density-operator) is needed.

## 2

↑ **Parent:** [Paper 37](paper-37.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

Diagonalize the [reduced density matrix](../../../bell-state.md#reduced-density-matrix) on Alice's [Hilbert space](../../../hilbert-space.md):

$$
\rho_A=\sum_{j=1}^r\lambda_j|a_j\rangle\langle a_j|,
\qquad\lambda_j>0.
$$

For every positive [eigenvalue](../../../linear-operator-theory.md#eigenvalue), define a vector on Bob's [Hilbert space](../../../hilbert-space.md) by

$$
|b_j\rangle=\lambda_j^{-1/2}(\langle a_j|\otimes I_B)|\Psi_{AB}\rangle.
$$

The definition of the [partial trace](../../../quantum-theory.md#partial-trace) gives

$$
\langle b_i|b_j\rangle
=\frac{\langle a_j|\rho_A|a_i\rangle}{\sqrt{\lambda_i\lambda_j}}
=\delta_{ij}.
$$

Thus the $|b_j\rangle$ are [orthonormal](../../../linear-algebra.md#orthonormal-set). Extend the $|a_j\rangle$ to an [orthonormal basis](../../../linear-algebra.md#orthonormal-basis) of Alice's [Hilbert space](../../../hilbert-space.md). If $|a\rangle$ lies in the zero-[eigenvalue](../../../linear-operator-theory.md#eigenvalue) subspace of $\rho_A$, then

$$
\| (\langle a|\otimes I_B)|\Psi_{AB}\rangle\|^2
=\langle a|\rho_A|a\rangle=0.
$$

There is therefore no component of $|\Psi_{AB}\rangle$ in those additional basis directions. Expansion in Alice's [orthonormal basis](../../../linear-algebra.md#orthonormal-basis) yields the [Schmidt decomposition](../../../von-neumann-entropy.md#schmidt-decomposition)

$$
\boxed{|\Psi_{AB}\rangle=\sum_{j=1}^r\sqrt{\lambda_j}|a_j\rangle|b_j\rangle,
\quad\sum_j\lambda_j=1.}
$$

Its positive [Schmidt coefficients](../../../von-neumann-entropy.md#schmidt-coefficient) are $s_j=\sqrt{\lambda_j}$ and its [Schmidt rank](../../../von-neumann-entropy.md#schmidt-rank) is $r$. Taking the two [partial traces](../../../quantum-theory.md#partial-trace) and using the [orthonormality](../../../linear-algebra.md#orthonormal-set) of both families gives

$$
\rho_A=\sum_j\lambda_j|a_j\rangle\langle a_j|,
\qquad
\rho_B=\sum_j\lambda_j|b_j\rangle\langle b_j|.
$$

Hence **the two reduced density matrices have exactly the same nonzero eigenvalues, including multiplicities**. Their numbers of zero [eigenvalues](../../../linear-operator-theory.md#eigenvalue) may differ when the local [Hilbert spaces](../../../hilbert-space.md) have different dimensions. In particular their [Von Neumann entropies](../../../von-neumann-entropy.md) agree.

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/i">i</h4>

↑ **Parent:** [B](#2/b)

<h5 id="2/b/i/solution">Solution</h5>

↑ **Parent:** [I](#2/b/i)

The coefficient [matrix](../../../vector-space.md#matrix) in the computational [orthonormal bases](../../../linear-algebra.md#orthonormal-basis), with Alice's index labelling rows, is

$$
C=\frac1{\sqrt3}\begin{pmatrix}0&-1\\1&1\end{pmatrix}.
$$

Since the entries are real, the [reduced density matrices](../../../bell-state.md#reduced-density-matrix) are

$$
\rho_A=CC^\dagger=\frac13\begin{pmatrix}1&-1\\-1&2\end{pmatrix},
\qquad
\rho_B=C^{\mathsf T}\overline C=\frac13\begin{pmatrix}1&1\\1&2\end{pmatrix}.
$$

Both have [trace](../../../linear-algebra.md#matrix-trace) one and [determinant](../../../linear-algebra.md#determinant) $1/9$. Their characteristic [polynomial](../../../polynomial.md) is $\lambda^2-\lambda+1/9$, so the nonzero [eigenvalues](../../../linear-operator-theory.md#eigenvalue) are

$$
\lambda_\pm=\frac{3\pm\sqrt5}{6}.
$$

Both are positive. Thus the [Schmidt rank](../../../von-neumann-entropy.md#schmidt-rank), or the [Schmidt number](../../../von-neumann-entropy.md#schmidt-number) of this [pure state](../../../quantum-theory.md#pure-state), is

$$
\boxed{r=2.}
$$

If “Schmidt numbers” denotes the individual positive [Schmidt coefficients](../../../von-neumann-entropy.md#schmidt-coefficient) instead, those are

$$
\boxed{s_+=\frac{\sqrt5+1}{2\sqrt3},\qquad s_-=\frac{\sqrt5-1}{2\sqrt3}.}
$$

Their squares are $\lambda_\pm$; giving both the [Schmidt rank](../../../von-neumann-entropy.md#schmidt-rank) and the [Schmidt coefficients](../../../von-neumann-entropy.md#schmidt-coefficient) removes this terminology ambiguity. The [pure state](../../../quantum-theory.md#pure-state) is [entangled](../../../bell-state.md#entangled-state) because its [Schmidt rank](../../../von-neumann-entropy.md#schmidt-rank) exceeds one.

<h4 id="2/b/ii">ii</h4>

↑ **Parent:** [B](#2/b)

<h5 id="2/b/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#2/b/ii)

Factor the coefficients into a [tensor product](../../../linear-algebra.md#tensor-product):

$$
|\Psi\rangle
=\left(\frac{|0\rangle-|1\rangle}{\sqrt2}\right)_A
\otimes\left(\frac{|0\rangle-|1\rangle}{\sqrt2}\right)_B.
$$

This is already a [Schmidt decomposition](../../../von-neumann-entropy.md#schmidt-decomposition) with one term. Consequently

$$
\boxed{r=1,\qquad s_1=1,\qquad\lambda_1=1.}
$$

Each [reduced density matrix](../../../bell-state.md#reduced-density-matrix) is the rank-one [orthogonal projector](../../../hilbert-space.md#orthogonal-projection) onto $(|0\rangle-|1\rangle)/\sqrt2$, so its other [eigenvalue](../../../linear-operator-theory.md#eigenvalue) is zero. The joint [pure state](../../../quantum-theory.md#pure-state) is a [product state](../../../bell-state.md#product-state), with no [entanglement](../../../bell-state.md#entangled-state).

## 3

↑ **Parent:** [Paper 37](paper-37.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

**Yes: a deterministic LOCC protocol exists for every allowed value of the parameter.** Here is an explicit implementation, so existence does not depend on merely quoting a pure-state conversion theorem.

First convert the input [Bell state](../../../bell-state.md) to $|\Phi^+\rangle=(|00\rangle+|11\rangle)/\sqrt2$ by [local unitary operations](../../../bell-state.md#local-unitary-operation):

$$
(Z_A\otimes X_B)|\Psi^-\rangle=|\Phi^+\rangle.
$$

Write $c=\cos\phi$ and $s=\sin\phi$. Alice performs the two-outcome [measurement in quantum mechanics](../../../quantum-measurement.md) with [Kraus operators](../../../quantum-information-theory.md#kraus-operator)

$$
M_0=\begin{pmatrix}c&0\\0&s\end{pmatrix},\qquad
M_1=\begin{pmatrix}s&0\\0&c\end{pmatrix}.
$$

They define a physical [measurement in quantum mechanics](../../../quantum-measurement.md) because

$$
M_0^\dagger M_0+M_1^\dagger M_1=(c^2+s^2)I=I.
$$

Acting on $|\Phi^+\rangle$, the unnormalized branch vectors are

$$
(M_0\otimes I)|\Phi^+\rangle=\frac{c|00\rangle+s|11\rangle}{\sqrt2},\qquad
(M_1\otimes I)|\Phi^+\rangle=\frac{s|00\rangle+c|11\rangle}{\sqrt2}.
$$

Both branches have [probability](../../../probability-theory.md#probability) $1/2$. Alice communicates the outcome to Bob. If it is one, both apply the [Pauli X gate](../../../quantum-theory.md#pauli-x-gate); this turns the normalized second branch into $c|00\rangle+s|11\rangle$. If it is zero, neither applies this correction. Finally Bob applies a [Pauli X gate](../../../quantum-theory.md#pauli-x-gate) in either branch, obtaining

$$
\boxed{c|01\rangle+s|10\rangle.}
$$

Every outcome produces the same target [pure state](../../../quantum-theory.md#pure-state), so this is deterministic [local operations and classical communication](../../../bell-state.md#local-operations-and-classical-communication), not a successful branch selected by [postselection](../../../quantum-measurement.md#postselection). This [two-outcome LOCC dilution of a Bell pair](../../../bell-state.md#two-outcome-locc-dilution-of-a-bell-pair) remains valid at $\phi=0$, where the output is a [product state](../../../bell-state.md#product-state), and at $\phi=\pi/4$, where it is another [Bell state](../../../bell-state.md).

The target [Schmidt coefficients](../../../von-neumann-entropy.md#schmidt-coefficient) are $c,s$, while those of the input are both $1/\sqrt2$. For an interior value $0<\phi<\pi/4$, [local unitary operations](../../../bell-state.md#local-unitary-operation) alone could not change these [Schmidt coefficients](../../../von-neumann-entropy.md#schmidt-coefficient); the local [measurement in quantum mechanics](../../../quantum-measurement.md) is the step that reduces the [entanglement](../../../bell-state.md#entangled-state).

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

Expand an initial bipartite [pure state](../../../quantum-theory.md#pure-state) in local [orthonormal bases](../../../linear-algebra.md#orthonormal-basis) as

$$
|\psi\rangle=\sum_{i,j}C_{ij}|i\rangle_A|j\rangle_B.
$$

By the [Schmidt decomposition](../../../von-neumann-entropy.md#schmidt-decomposition), or equivalently the [singular value decomposition](../../../linear-algebra.md#singular-value-decomposition) of $C$, its [Schmidt rank](../../../von-neumann-entropy.md#schmidt-rank) is $\operatorname{rank}C$. In a specified local measurement branch, the product [Kraus operator](../../../quantum-information-theory.md#kraus-operator) $A\otimes B$ changes the coefficient [matrix](../../../vector-space.md#matrix) to

$$
C'=ACB^{\mathsf T}.
$$

Indeed the coefficient of $|k\rangle|l\rangle$ is $\sum_{i,j}A_{ki}C_{ij}B_{lj}$. The elementary [matrix rank](../../../vector-space.md#matrix-rank) inequality gives

$$
\operatorname{rank}(ACB^{\mathsf T})\leq\operatorname{rank}C.
$$

Normalizing a nonzero branch multiplies $C'$ by a scalar and therefore leaves its [matrix rank](../../../vector-space.md#matrix-rank) unchanged.

Now refine a complete [LOCC](../../../bell-state.md#local-operations-and-classical-communication) transcript to record every individual [Kraus operator](../../../quantum-information-theory.md#kraus-operator). Although later choices depend on the earlier classical outcomes, fixing a transcript fixes all those choices. Composing the local operations therefore gives a single product [Kraus operator](../../../quantum-information-theory.md#kraus-operator) $A_\tau\otimes B_\tau$ in that branch. Each nonzero branch obeys the same [Schmidt-rank contraction under product operators](../../../von-neumann-entropy.md#schmidt-rank-contraction-under-product-operators). Local auxiliary systems prepared independently are included by local isometries and do not add [entanglement](../../../bell-state.md#entangled-state). Discarding a local auxiliary system is included by resolving its [partial trace](../../../quantum-theory.md#partial-trace) in an [orthonormal basis](../../../linear-algebra.md#orthonormal-basis); this again yields refined product [Kraus operators](../../../quantum-information-theory.md#kraus-operator).

If the protocol produces a specified [pure state](../../../quantum-theory.md#pure-state) deterministically, its output [density operator](../../../quantum-theory.md#density-matrix) is a sum of positive rank-one branch [density operators](../../../quantum-theory.md#density-matrix). Every nonzero branch vector must be proportional to that output vector: its squared overlap with any vector orthogonal to the output sums to zero, so each such overlap is separately zero. Thus the output [Schmidt rank](../../../von-neumann-entropy.md#schmidt-rank) equals that of each surviving branch, and

$$
\boxed{r_{\mathrm{out}}\leq r_{\mathrm{in}}.}
$$

This proves [monotonicity of Schmidt rank under LOCC](../../../von-neumann-entropy.md#monotonicity-of-schmidt-rank-under-locc), even for a nonzero branch selected by [postselection](../../../quantum-measurement.md#postselection). If the classical transcript is instead discarded and the result is mixed, the refined branch vectors supply an ensemble with [Schmidt ranks](../../../von-neumann-entropy.md#schmidt-rank) at most $r_{\mathrm{in}}$; by definition its [Schmidt number](../../../von-neumann-entropy.md#schmidt-number) is at most $r_{\mathrm{in}}$. This is the correct mixed-state extension, rather than a bound on the ranks of its [reduced density matrices](../../../bell-state.md#reduced-density-matrix). In finite dimensions, any limiting exact protocol obeys the same pure-state bound because the set of coefficient [matrices](../../../vector-space.md#matrix) of rank at most $r_{\mathrm{in}}$ is closed, being defined by vanishing minors.

## 4

↑ **Parent:** [Paper 37](paper-37.md)

<h3 id="4/a">a</h3>

↑ **Parent:** [4](#4)

<h4 id="4/a/solution">Solution</h4>

↑ **Parent:** [A](#4/a)

A [discrete memoryless channel](../../../coding-theory.md#discrete-memoryless-channel) is specified by discrete input and output [alphabets](../../../information-theory.md#alphabet) and a transition [probability](../../../probability-theory.md#probability) $W(y|x)$, with $W(y|x)\geq0$ and $\sum_yW(y|x)=1$. Its successive outputs are conditionally independent given the inputs, with the same transition rule at every use:

$$
\Pr(Y_1=y_1,\ldots,Y_n=y_n\mid X_1=x_1,\ldots,X_n=x_n)
=\prod_{j=1}^nW(y_j|x_j).
$$

Operationally, its [channel capacity](../../../information-theory.md#channel-capacity) is the supremum of communication rates in [bits](../../../information-theory.md#bit) per use attainable by increasingly long block codes with decoding error [probability](../../../probability-theory.md#probability) tending to zero. For finite [alphabets](../../../information-theory.md#alphabet), the equivalent Shannon characterization is

$$
C=\max_{P_X}I(X;Y),\qquad
I(X;Y)=H(Y)-H(Y|X),
$$

where $H$ is [Shannon entropy](../../../information-theory.md#information-entropy), $H(Y|X)$ is classical [conditional entropy](../../../information-theory.md#conditional-entropy), and the maximization is over the input [probability distribution](../../../probability-theory.md#probability-distribution).

For the channel in question, the transition [matrix](../../../vector-space.md#matrix), with input symbols indexing rows, is

$$
W=\begin{pmatrix}
2/3&1/3&0\\
0&2/3&1/3\\
1/3&0&2/3
\end{pmatrix}.
$$

Every row has the same [Shannon entropy](../../../information-theory.md#information-entropy), namely the [binary entropy](../../../information-theory.md#binary-entropy) $h_2(1/3)$. Consequently $H(Y|X)=h_2(1/3)$ for every input [probability distribution](../../../probability-theory.md#probability-distribution). Since the output has three symbols, the [maximum entropy on a finite alphabet](../../../information-theory.md#maximum-entropy-on-a-finite-alphabet) gives

$$
I(X;Y)\leq\log_2 3-h_2(1/3).
$$

Choose a uniform input. Each column of $W$ sums to one, so $P_Y(y)=1/3$ for every output symbol and the upper bound is attained. Finally

$$
h_2(1/3)=-\frac13\log_2\frac13-\frac23\log_2\frac23
=\log_2 3-\frac23.
$$

Thus the [cyclic ternary channel capacity](../../../information-theory.md#cyclic-ternary-channel-capacity) is

$$
\boxed{C=\frac23\text{ bits per channel use},}
$$

achieved by a uniform input [probability distribution](../../../probability-theory.md#probability-distribution). This is a [weakly symmetric channel capacity](../../../information-theory.md#weakly-symmetric-channel-capacity) calculation: the [matrix](../../../vector-space.md#matrix) rows are permutations and the column sums agree. The channel is not the usual ternary symmetric-error channel, since an error has only one possible changed output for each input.

<h3 id="4/b">b</h3>

↑ **Parent:** [4](#4)

<h4 id="4/b/solution">Solution</h4>

↑ **Parent:** [B](#4/b)

There is a normalization error in the original PDF: the first term contains $I$ rather than $\rho$. For a normalized [qubit](../../../quantum-mechanics.md#qubit) [density operator](../../../quantum-theory.md#density-matrix), that printed expression has [trace](../../../linear-algebra.md#matrix-trace) $2(1-p)+p=2-p$, so it is not a [quantum channel](../../../quantum-information-theory.md#quantum-channel) except at $p=1$. The intended [depolarizing channel](../../../quantum-information-theory.md#quantum-depolarizing-channel) is the [Pauli channel](../../../quantum-information-theory.md#pauli-channel) that leaves the input unchanged with [probability](../../../probability-theory.md#probability) $1-p$ and applies each nonidentity [Pauli matrix](../../../algebra.md#pauli-matrices) with [probability](../../../probability-theory.md#probability) $p/3$, for $0\leq p\leq1$. Its [Kraus operators](../../../quantum-information-theory.md#kraus-operator) are

$$
K_0=\sqrt{1-p}\,I,\qquad K_k=\sqrt{p/3}\,\sigma_k\quad(k=1,2,3),
$$

and $\sum_{k=0}^3K_k^\dagger K_k=I$, proving that it is trace-preserving and a [completely positive map](../../../quantum-information-theory.md#completely-positive-map).

Write the input in its [Bloch vector](../../../quantum-theory.md#bloch-vector) representation,

$$
\rho=\frac12(I+\mathbf r\cdot\boldsymbol\sigma),\qquad |\mathbf r|\leq1.
$$

Conjugation by a [Pauli matrix](../../../algebra.md#pauli-matrices) keeps its own [Bloch vector](../../../quantum-theory.md#bloch-vector) component and reverses the other two. More explicitly, $\sigma_k\sigma_j\sigma_k=\sigma_j$ for $j=k$ and $-\sigma_j$ for $j\ne k$. Hence

$$
\sum_{k=1}^3\sigma_k\rho\sigma_k
=\frac12(3I-\mathbf r\cdot\boldsymbol\sigma)
=2I-\rho.
$$

The corrected [quantum channel](../../../quantum-information-theory.md#quantum-channel) therefore gives

$$
\Phi_p(\rho)=(1-p)\rho+\frac p3(2I-\rho)
=\frac12\left[I+\left(1-\frac{4p}{3}\right)\mathbf r\cdot\boldsymbol\sigma\right].
$$

Thus its action is

$$
\boxed{\mathbf r\longmapsto\left(1-\frac{4p}{3}\right)\mathbf r.}
$$

The [Bloch sphere](../../../quantum-theory.md#bloch-sphere) is sent to a sphere of radius $|1-4p/3|$ about the origin of the [Bloch ball](../../../quantum-theory.md#bloch-ball). At $p=0$ the action is the identity. For $0<p<3/4$ the [Bloch vector](../../../quantum-theory.md#bloch-vector) shrinks without changing direction. At $p=3/4$ every input becomes the maximally mixed [density operator](../../../quantum-theory.md#density-matrix) $I/2$. For $3/4<p\leq1$, the [Bloch vector](../../../quantum-theory.md#bloch-vector) reverses direction and shrinks, reaching factor $-1/3$ at $p=1$. The reversal is compatible with complete positivity because this remains a probabilistic mixture of [Pauli matrices](../../../algebra.md#pauli-matrices). The parameter here is the total nonidentity-error [probability](../../../probability-theory.md#probability), not the retention parameter used in some definitions of the [quantum depolarizing channel](../../../quantum-information-theory.md#quantum-depolarizing-channel).

For completeness, retain the PDF literally and call its output $F_p(\rho)$. The same calculation gives

$$
F_p(\rho)=\left(1-\frac p2\right)I-\frac p6\mathbf r\cdot\boldsymbol\sigma,
\qquad\operatorname{Tr}F_p(\rho)=2-p.
$$

This has no normalized-output [Bloch ball](../../../quantum-theory.md#bloch-ball) interpretation as printed. If it is manually normalized, then

$$
\frac{F_p(\rho)}{2-p}
=\frac12\left[I-\frac{p}{3(2-p)}\mathbf r\cdot\boldsymbol\sigma\right].
$$

That different transformation sends $p=0$ to $I/2$, rather than to the input, and agrees with the intended answer only at $p=1$. The literal and corrected conventions therefore cannot be silently identified.

## 5

↑ **Parent:** [Paper 37](paper-37.md)

<h3 id="5/a">a</h3>

↑ **Parent:** [5](#5)

<h4 id="5/a/solution">Solution</h4>

↑ **Parent:** [A](#5/a)

Under the intended assumption that one use of the [quantum channel](../../../quantum-information-theory.md#quantum-channel) transmits one [qubit](../../../quantum-mechanics.md#qubit) without noise, Alice can communicate two [classical bits](../../../information-theory.md#bit) with certainty if she and Bob already share a [Bell pair](../../../bell-state.md#bell-pair). She uses **superdense coding**. The prior distribution of the [Bell pair](../../../bell-state.md#bell-pair) must be a resource available before the permitted channel use; distributing it through that same channel would consume another use.

Take the shared [Bell state](../../../bell-state.md) to be $|\Phi^+\rangle=(|00\rangle+|11\rangle)/\sqrt2$, with Alice holding the first [qubit](../../../quantum-mechanics.md#qubit). For a two-[bit](../../../information-theory.md#bit) message $(a,b)\in\{0,1\}^2$, Alice applies the [local unitary operation](../../../bell-state.md#local-unitary-operation) $U_{ab}=X^aZ^b$ to her [qubit](../../../quantum-mechanics.md#qubit). The four encoded [pure states](../../../quantum-theory.md#pure-state) are, up to irrelevant [global phases](../../../quantum-mechanics.md#global-phase),

$$
\begin{array}{c|c|c}
(a,b)&U_{ab}&(U_{ab}\otimes I)|\Phi^+\rangle\\\hline
(0,0)&I&|\Phi^+\rangle\\
(0,1)&Z&|\Phi^-\rangle\\
(1,0)&X&|\Psi^+\rangle\\
(1,1)&XZ&-|\Psi^-\rangle
\end{array}
$$

They are [orthogonal](../../../linear-algebra.md#orthogonal-vectors): for any [matrix](../../../vector-space.md#matrix) $V$ on the first [qubit](../../../quantum-mechanics.md#qubit), $\langle\Phi^+|(V\otimes I)|\Phi^+\rangle=\operatorname{Tr}V/2$, and the four [Pauli operators](../../../quantum-circuit.md#pauli-operator) are [orthogonal](../../../linear-algebra.md#orthogonal-vectors) in the [trace inner product](../../../linear-algebra.md#frobenius-inner-product). Explicitly,

$$
\langle\Phi^+|(U_{ab}^\dagger U_{a'b'}\otimes I)|\Phi^+\rangle
=\delta_{aa'}\delta_{bb'}.
$$

Alice sends her [qubit](../../../quantum-mechanics.md#qubit) through the [quantum channel](../../../quantum-information-theory.md#quantum-channel) once. Bob now holds both [qubits](../../../quantum-mechanics.md#qubit) and performs a [Bell-basis measurement](../../../bell-state.md#bell-basis-measurement). Its four [orthogonal projectors](../../../hilbert-space.md#orthogonal-projection) identify $(a,b)$ with certainty, giving

$$
\boxed{\text{one shared Bell pair + one noiseless qubit transmission}
\ \Longrightarrow\ \text{two classical bits}.}
$$

Before the transmission, Bob's [reduced density matrix](../../../bell-state.md#reduced-density-matrix) is $I/2$ for every message, so shared [entanglement](../../../bell-state.md#entangled-state) alone does not convey the message.

Without shared [entanglement](../../../bell-state.md#entangled-state), a noiseless single-[qubit](../../../quantum-mechanics.md#qubit) transmission cannot perfectly distinguish four messages: perfect discrimination requires [orthogonal](../../../linear-algebra.md#orthogonal-vectors) state supports, and its two-dimensional [Hilbert space](../../../hilbert-space.md) has room for at most two nonzero mutually [orthogonal](../../../linear-algebra.md#orthogonal-vectors) supports. The [Holevo bound](../../../quantum-information-theory.md#holevo-s-theorem) also limits its accessible classical information to one [bit](../../../information-theory.md#bit). For the usual protocol starting with a shared two-[qubit](../../../quantum-mechanics.md#qubit) [pure state](../../../quantum-theory.md#pure-state) and using local unitary encodings, exact two-[bit](../../../information-theory.md#bit) transmission requires a maximally mixed Bob marginal. Indeed all encoded joint states are pure and have the same $\rho_B$, while [Subadditivity of Von Neumann entropy](../../../von-neumann-entropy.md#subadditivity-of-von-neumann-entropy) gives their average entropy at most $1+S(\rho_B)$. Four equally likely perfectly distinguishable messages have average [Von Neumann entropy](../../../von-neumann-entropy.md) two, forcing $S(\rho_B)=1$ and hence a [maximally entangled state](../../../quantum-theory.md#maximally-entangled-state).

The specification “quantum channel” alone does not determine its dimension or noise, so the one-[qubit](../../../quantum-mechanics.md#qubit), noiseless interpretation is needed for this particular conclusion. A noiseless four-dimensional channel could send four [orthogonal](../../../linear-algebra.md#orthogonal-vectors) states without any shared [entanglement](../../../bell-state.md#entangled-state); a completely depolarizing [qubit](../../../quantum-mechanics.md#qubit) channel cannot transmit the message even with a shared [Bell pair](../../../bell-state.md#bell-pair), since its output is independent of Alice's encoding. Shared [entanglement](../../../bell-state.md#entangled-state) is therefore the extra resource for the intended single-[qubit](../../../quantum-mechanics.md#qubit) channel, not a guarantee for every unspecified [quantum channel](../../../quantum-information-theory.md#quantum-channel).

<h3 id="5/b">b</h3>

↑ **Parent:** [5](#5)

<h4 id="5/b/solution">Solution</h4>

↑ **Parent:** [B](#5/b)

Let $D=\mathcal C_{\mathrm{ev}}$, and write $\mathcal C_{\mathrm{odd}}=t+D$ for any odd-weight word $t\in\mathcal C_H$. The parity functional on the four-dimensional binary [linear code](../../../coding-theory.md#linear-code) $\mathcal C_H$ is nonzero, so its kernel $D$ has dimension three and its other fibre is the coset $t+D$. For example $t=(1,\ldots,1)$ belongs to the standard length-seven [Hamming code](../../../coding-theory.md#hamming-code) and has odd [Hamming weight](../../../coding-theory.md#hamming-weight). Denote the two logical basis states by $|\psi_0\rangle$ and $|\psi_1\rangle$, corresponding to these two cosets. The eight computational [orthonormal basis](../../../linear-algebra.md#orthonormal-basis) vectors in each sum are distinct, so both logical states have norm one; their disjoint supports make them [orthogonal](../../../linear-algebra.md#orthogonal-vectors).

For a binary vector $w\in\mathbb F_2^7$, define the product of [Pauli Z gates](../../../quantum-theory.md#pauli-z-gate)

$$
Z(w)=\bigotimes_{j=1}^7 Z_j^{w_j},\qquad
Z(w)|x\rangle=(-1)^{w\cdot x}|x\rangle,
$$

where the dot product is computed modulo two. The key diagonal overlap, with $t_0=0$ and $t_1=t$, is

$$
\langle\psi_a|Z(w)|\psi_a\rangle
=\frac{(-1)^{w\cdot t_a}}8\sum_{x\in D}(-1)^{w\cdot x}.
$$

If $w\in D^\perp$, every summand is one. If $w\notin D^\perp$, choose $x_0\in D$ with $w\cdot x_0=1$. Translation $x\mapsto x+x_0$ permutes $D$ and negates every summand. The sum must then be zero. Thus

$$
\sum_{x\in D}(-1)^{w\cdot x}
=\begin{cases}8,&w\in D^\perp,\\0,&w\notin D^\perp.\end{cases}
$$

Off-diagonal logical overlaps vanish for every $w$:

$$
\langle\psi_0|Z(w)|\psi_1\rangle=0,
$$

because a diagonal [Pauli operator](../../../quantum-circuit.md#pauli-operator) cannot move a computational basis word from one coset to the disjoint other coset.

The possible errors are $E_0=I$ and $E_j=Z(e_j)$ for $j=1,\ldots,7$. Set $e_0=0$. Each [phase flip](../../../quantum-theory.md#pauli-z-gate) is its own adjoint and inverse, so

$$
E_i^\dagger E_j=Z(e_i+e_j).
$$

If $i\ne j$, the vector $e_i+e_j$ is nonzero and has [Hamming weight](../../../coding-theory.md#hamming-weight) one or two. By the given [dual code](../../../coding-theory.md#dual-code) identity $D^\perp=\mathcal C_H$ and the minimum [Hamming distance](../../../coding-theory.md#hamming-distance) three of the [Hamming code](../../../coding-theory.md#hamming-code), it cannot belong to $D^\perp$. Hence all its diagonal logical overlaps vanish. If $i=j$, the product is the identity and its logical overlaps are $\delta_{ab}$. Combining both cases gives

$$
\boxed{\langle\psi_a|E_i^\dagger E_j|\psi_b\rangle
=\delta_{ij}\delta_{ab}\quad(a,b\in\{0,1\},\ i,j\in\{0,\ldots,7\}).}
$$

This proves the [Knill--Laflamme condition](../../../quantum-error-correction.md#knill-laflamme-condition) with an identity error-overlap [matrix](../../../vector-space.md#matrix), not merely a possibly degenerate scalar [matrix](../../../vector-space.md#matrix). In particular the eight two-dimensional error subspaces $E_i\mathcal X_{\mathrm{Steane}}$ are mutually [orthogonal](../../../linear-algebra.md#orthogonal-vectors). This is precisely [nondegenerate phase-flip correction in the Steane code](../../../quantum-error-correction.md#nondegenerate-phase-flip-correction-in-the-steane-code).

To exhibit recovery rather than only the criterion, let $P$ be the [orthogonal projector](../../../hilbert-space.md#orthogonal-projection) onto the code and $P_i=E_iPE_i^\dagger$. The [projective measurement](../../../quantum-measurement.md#projective-measurement) consisting of these eight mutually [orthogonal projectors](../../../hilbert-space.md#orthogonal-projection), completed by $I-\sum_iP_i$, determines which error occurred. For an arbitrary encoded [pure state](../../../quantum-theory.md#pure-state) $|\chi\rangle=\alpha|\psi_0\rangle+\beta|\psi_1\rangle$ affected by $E_j$, outcome $j$ occurs with certainty and leaves $E_j|\chi\rangle$ unchanged. Applying $E_j$ again recovers $|\chi\rangle$. The outcome gives the [error syndrome](../../../quantum-error-correction.md#error-syndrome) and does not reveal $\alpha$ or $\beta$, so recovery preserves logical [quantum superpositions](../../../quantum-mechanics.md#quantum-superposition).

An equivalent explicit [error syndrome](../../../quantum-error-correction.md#error-syndrome) uses three commuting X-type [stabilizer generators](../../../quantum-circuit.md#stabilizer-generator). Choose a [parity-check matrix](../../../coding-theory.md#parity-check-matrix) for $\mathcal C_H$ with the seven different nonzero binary columns:

$$
H=\begin{pmatrix}
1&0&1&0&1&0&1\\
0&1&1&0&0&1&1\\
0&0&0&1&1&1&1
\end{pmatrix}.
$$

Its rows span $\mathcal C_H^\perp=D$. For a row $h_l$, the operator $X(h_l)=\bigotimes_jX_j^{(h_l)_j}$ permutes each of $D$ and $t+D$, and therefore has eigenvalue $+1$ on both logical states. A [phase flip](../../../quantum-theory.md#pauli-z-gate) at position $j$ changes its eigenvalue to $(-1)^{H_{lj}}$, since $X(h_l)Z_j=(-1)^{H_{lj}}Z_jX(h_l)$. Measuring the three commuting [stabilizer generators](../../../quantum-circuit.md#stabilizer-generator) gives the $j$th column of $H$ as a binary [syndrome](../../../coding-theory.md#syndrome); no error gives the zero column. All eight outcomes are different, and applying the identified $Z_j$ restores the code state. Measuring these [stabilizer generators](../../../quantum-circuit.md#stabilizer-generator) never distinguishes the two logical states.

Finally, if a noise [Kraus operator](../../../quantum-information-theory.md#kraus-operator) is a coherent linear combination $F=\sum_jc_jE_j$, the same syndrome measurement separates its mutually [orthogonal](../../../linear-algebra.md#orthogonal-vectors) components $c_jE_j|\chi\rangle$. Conditional recovery returns $|\chi\rangle$ in every nonzero branch. Linearity then also corrects any [quantum channel](../../../quantum-information-theory.md#quantum-channel) whose [Kraus operators](../../../quantum-information-theory.md#kraus-operator) lie in this span. The argument therefore corrects arbitrary unknown single-site [phase flips](../../../quantum-theory.md#pauli-z-gate) nondegenerately, including coherent phase-error amplitudes, rather than only a known error on a basis codeword.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2005](../../2005.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
