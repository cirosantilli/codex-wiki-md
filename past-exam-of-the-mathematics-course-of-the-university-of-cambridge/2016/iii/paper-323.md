# Paper 323

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2016/paper_323.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2016/paper_323.pdf)

**Table of contents**

- [1](#1)
  - [i](#1/i)
    - [Solution](#1/i/solution)
  - [ii](#1/ii)
    - [Solution](#1/ii/solution)
- [2](#2)
  - [i](#2/i)
    - [Solution](#2/i/solution)
  - [ii](#2/ii)
    - [Solution](#2/ii/solution)
- [3](#3)
  - [i](#3/i)
    - [Solution](#3/i/solution)
  - [ii](#3/ii)
    - [Solution](#3/ii/solution)
  - [iii](#3/iii)
    - [a](#3/iii/a)
      - [Solution](#3/iii/a/solution)
    - [b](#3/iii/b)
      - [Solution](#3/iii/b/solution)
    - [c](#3/iii/c)
      - [Solution](#3/iii/c/solution)
- [4](#4)
  - [i](#4/i)
    - [Solution](#4/i/solution)
  - [ii](#4/ii)
    - [Solution](#4/ii/solution)
  - [iii](#4/iii)
    - [Solution](#4/iii/solution)
- [5](#5)
  - [1](#5/1)
    - [Solution](#5/1/solution)
  - [2](#5/2)
    - [Solution](#5/2/solution)
  - [3](#5/3)
    - [Solution](#5/3/solution)

## 1

↑ **Parent:** [Paper 323](paper-323.md)

<h3 id="1/i">i</h3>

↑ **Parent:** [1](#1)

<h4 id="1/i/solution">Solution</h4>

↑ **Parent:** [I](#1/i)

The useful object is the [Choi state](../../../quantum-information-theory.md#choi-state) of the [entanglement-breaking channel](../../../quantum-information-theory.md#entanglement-breaking-channel). Put $d_A=\dim\mathcal H_A$, introduce a reference $R$ with the same [computational basis](../../../quantum-theory.md#computational-basis) as $A$, and use the normalized [maximally entangled state](../../../quantum-theory.md#maximally-entangled-state)

$$
|\Phi\rangle_{RA}=d_A^{-1/2}\sum_j|j\rangle_R|j\rangle_A,\qquad
C_{RB}=(\operatorname{id}_R\otimes\mathcal E)(|\Phi\rangle\langle\Phi|).
$$

The [entanglement-breaking channel](../../../quantum-information-theory.md#entanglement-breaking-channel) makes $C_{RB}$ a [separable quantum state](../../../quantum-information-theory.md#separable-quantum-state). Its [partial trace](../../../quantum-theory.md#partial-trace) is $\operatorname{Tr}_B C_{RB}=I_R/d_A$, because $\mathcal E$ is a [quantum channel](../../../quantum-information-theory.md#quantum-channel). Write a [separable positive operator](../../../quantum-information-theory.md#separable-positive-operator) decomposition

$$
C_{RB}=\sum_y\alpha_y\otimes\beta_y,\qquad \alpha_y\geq0,\quad\beta_y\geq0.
$$

Discard any term with $\operatorname{Tr}\beta_y=0$: a [positive operator](../../../hilbert-space.md#positive-operator) with zero [trace](../../../linear-algebra.md#matrix-trace) is zero. Define

$$
\tau_y=\frac{\beta_y}{\operatorname{Tr}\beta_y},\qquad
E_y=d_A(\operatorname{Tr}\beta_y)\alpha_y^T.
$$

Each $\tau_y$ is a [density operator](../../../quantum-theory.md#density-matrix). Each $E_y$ is a [positive operator](../../../hilbert-space.md#positive-operator), and taking the [matrix transpose](../../../vector-space.md#transpose) of the [partial trace](../../../quantum-theory.md#partial-trace) identity gives

$$
\sum_y E_y=d_A\left(\sum_y(\operatorname{Tr}\beta_y)\alpha_y\right)^T=I_A.
$$

Thus the $E_y$ form a [POVM](../../../quantum-measurement.md#positive-operator-valued-measure). In this reference-first convention, the [Choi reconstruction formula](../../../quantum-information-theory.md#choi-reconstruction-formula) is

$$
\mathcal E(L)=d_A\operatorname{Tr}_R[(L^T\otimes I_B)C_{RB}]
=\sum_y\tau_y\operatorname{Tr}(E_yL).
$$

The factor $d_A$ is essential because we used a normalized [Choi state](../../../quantum-information-theory.md#choi-state). A [measurement channel](../../../quantum-information-theory.md#measurement-channel) storing the outcome $y$, followed by the prescribed [quantum state preparation](../../../quantum-circuit.md#quantum-state-preparation) of $\tau_y$, has precisely this action on every [linear operator](../../../vector-space.md#linear-operator) $L$. **The desired factorization is therefore**

$$
\boxed{\mathcal E^{B\leftarrow A}=\mathcal P^{B\leftarrow\widetilde Y}\mathcal M^{\widetilde Y\leftarrow A}.}
$$

<h3 id="1/ii">ii</h3>

↑ **Parent:** [1](#1)

<h4 id="1/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#1/ii)

Write $X$ and $Y$ for the classical [quantum registers](../../../quantum-circuit.md#quantum-register) $\widetilde X$ and $\widetilde Y$. By the [quantum mutual information](../../../von-neumann-entropy.md#quantum-mutual-information) formula $I(U:V)=S(U)+S(V)-S(UV)$, expanding the right-hand side of the [quantum mutual information balance identity](../../../von-neumann-entropy.md#quantum-mutual-information-balance-identity) gives

$$
\begin{aligned}
&I(X:B)+I(XB:D)-I(B:D)\\
&=S(X)+S(B)-S(XB)+S(XB)+S(D)-S(XBD)\\
&\qquad-S(B)-S(D)+S(BD)\\
&=S(X)+S(BD)-S(XBD)=I(X:BD).
\end{aligned}
$$

All [Von Neumann entropies](../../../von-neumann-entropy.md) here are evaluated in $\omega$.

We use three facts: [quantum mutual information](../../../von-neumann-entropy.md#quantum-mutual-information) is nonnegative by [nonnegativity of quantum relative entropy](../../../von-neumann-entropy.md#nonnegativity-of-quantum-relative-entropy); a local [quantum channel](../../../quantum-information-theory.md#quantum-channel) cannot increase it by [data processing for quantum mutual information](../../../von-neumann-entropy.md#data-processing-for-quantum-mutual-information); and the [quantum mutual information](../../../von-neumann-entropy.md#quantum-mutual-information) of a [classical-quantum state](../../../quantum-information-theory.md#classical-quantum-state) is its ensemble's [Holevo quantity](../../../quantum-information-theory.md#holevo-quantity). Write $\chi(\mathcal T)$ for the [Holevo capacity](../../../quantum-information-theory.md#holevo-capacity), the supremum of the output [Holevo quantity](../../../quantum-information-theory.md#holevo-quantity) over finite input ensembles.

The $XB$ marginal is an output ensemble for $\mathcal E$, with inputs $\rho(x)_A=\operatorname{Tr}_C\rho(x)_{AC}$. Consequently $I(X:B)_\omega\leq\chi(\mathcal E)$. Also $\omega_{XBD}$ is obtained from $\sigma_{XYD}$ by a [quantum channel](../../../quantum-information-theory.md#quantum-channel) on $XY$ which retains $X$ and prepares $B$ from $Y$. Hence

$$
I(XB:D)_\omega\leq I(XY:D)_\sigma.
$$

To bound the latter even for [entangled states](../../../bell-state.md#entangled-state) $\rho(x)_{AC}$, exhibit the [conditional input ensemble after a local measurement](../../../quantum-information-theory.md#conditional-input-ensemble-after-a-local-measurement). Set

$$
q(y|x)=\operatorname{Tr}[(E_y\otimes I_C)\rho(x)_{AC}],\qquad
\rho_C^{x,y}=\frac{\operatorname{Tr}_A[(\sqrt{E_y}\otimes I_C)\rho(x)_{AC}(\sqrt{E_y}\otimes I_C)]}{q(y|x)}
$$

when $q(y|x)>0$; zero-weight outcomes can be omitted. The numerator is a [positive operator](../../../hilbert-space.md#positive-operator), its [trace](../../../linear-algebra.md#matrix-trace) is $q(y|x)$, and the $q(y|x)$ sum to one. Thus

$$
\sigma_{XYD}=\sum_{x,y}P_X(x)q(y|x)|x,y\rangle\langle x,y|\otimes\mathcal N(\rho_C^{x,y}).
$$

This is a [classical-quantum state](../../../quantum-information-theory.md#classical-quantum-state) with an output ensemble for $\mathcal N$, so $I(XY:D)_\sigma\leq\chi(\mathcal N)$. Combining these bounds with $I(B:D)_\omega\geq0$ yields

$$
\boxed{I(X:BD)_\omega\leq\chi(\mathcal E)+\chi(\mathcal N),\qquad
\chi(\mathcal E\otimes\mathcal N)\leq\chi(\mathcal E)+\chi(\mathcal N).}
$$

The last step takes the supremum over all input ensembles on $AC$. **The left-hand channel direction is $B\leftarrow A$**, as established in part (i); the printed $A\leftarrow B$ in the last inequality is a typographical reversal. Independent product ensembles also give the reverse inequality, so this proves [Holevo-capacity additivity for entanglement-breaking channels](../../../quantum-information-theory.md#holevo-capacity-additivity-for-entanglement-breaking-channels).

## 2

↑ **Parent:** [Paper 323](paper-323.md)

<h3 id="2/i">i</h3>

↑ **Parent:** [2](#2)

<h4 id="2/i/solution">Solution</h4>

↑ **Parent:** [I](#2/i)

Use an [orthonormal eigenbasis](../../../linear-operator-theory.md#orthonormal-eigenbasis) of the [Hermitian operator](../../../hilbert-space.md#hermitian-operator) $A$ and set $b_j=\langle\alpha_j|B|\alpha_j\rangle$. Since $B$ is a [positive contraction](../../../hilbert-space.md#positive-contraction),

$$
0\leq b_j\leq1,\qquad \sum_jb_j=r,\qquad \operatorname{Tr}(AB)=\sum_j\lambda_jb_j.
$$

For $0<r<d$, the missing weight among the first $r$ entries equals the weight in the remaining entries:

$$
t:=\sum_{j<r}(1-b_j)=\sum_{j\geq r}b_j.
$$

The ordered [eigenvalues](../../../linear-operator-theory.md#eigenvalue) satisfy $\lambda_j\geq\lambda_{r-1}$ for $j<r$ and $\lambda_j\leq\lambda_{r-1}$ for $j\geq r$. Therefore

$$
\sum_{j<r}\lambda_j-\operatorname{Tr}(AB)
=\sum_{j<r}\lambda_j(1-b_j)-\sum_{j\geq r}\lambda_jb_j
\geq\lambda_{r-1}t-\lambda_{r-1}t=0.
$$

This argument does not require the [eigenvalues](../../../linear-operator-theory.md#eigenvalue) of $A$ to be positive. For $r=0$, positivity and zero [trace](../../../linear-algebra.md#matrix-trace) give $B=0$; for $r=d$, the same argument applied to $I-B$ gives $B=I$. Thus **in every case**

$$
\boxed{\operatorname{Tr}(AB)\leq\sum_{j<r}\lambda_j.}
$$

The [orthogonal projection](../../../hilbert-space.md#orthogonal-projection) onto the leading $r$ [eigenvectors](../../../linear-operator-theory.md#eigenvector) attains equality. This is the [Hermitian effect variational principle](../../../mathematical-optimization.md#hermitian-effect-variational-principle), extending the [Ky Fan maximum principle](../../../mathematical-optimization.md#ky-fan-maximum-principle) to all [positive contractions](../../../hilbert-space.md#positive-contraction) with the prescribed [trace](../../../linear-algebra.md#matrix-trace).

<h3 id="2/ii">ii</h3>

↑ **Parent:** [2](#2)

<h4 id="2/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#2/ii)

Choose [Kraus representations](../../../quantum-information-theory.md#kraus-representation)

$$
\mathcal C(L)=\sum_a C_aLC_a^\dagger,\qquad
\mathcal D(M)=\sum_b D_bMD_b^\dagger,\qquad
\sum_aC_a^\dagger C_a=I_Q,\quad\sum_bD_b^\dagger D_b=I_K.
$$

The composite [quantum channel](../../../quantum-information-theory.md#quantum-channel) has [Kraus operators](../../../quantum-information-theory.md#kraus-operator) $T_{ba}=D_bC_a$. Each has [matrix rank](../../../vector-space.md#matrix-rank) at most $k$, because it factors through the $k$-dimensional space $K$, and

$$
\sum_{a,b}T_{ba}^\dagger T_{ba}=I_Q.
$$

The [operation fidelity](../../../quantum-information-theory.md#operation-fidelity) uses the unsquared [quantum fidelity](../../../quantum-information-theory.md#fidelity-of-quantum-states) on a [purification of a density operator](../../../quantum-theory.md#purification-of-a-density-operator), so its square is [entanglement fidelity](../../../quantum-information-theory.md#entanglement-fidelity). The [Kraus formula for entanglement fidelity](../../../quantum-information-theory.md#kraus-formula-for-entanglement-fidelity) gives

$$
F_{\rm op}(\mathcal D\mathcal C,\rho_Q)^2
=\sum_{a,b}|\operatorname{Tr}(\rho_Q T_{ba})|^2.
$$

Indeed each overlap $\langle\Psi_\rho|(I_R\otimes T_{ba})|\Psi_\rho\rangle$ equals $\operatorname{Tr}(\rho_QT_{ba})$.

For any one of these [Kraus operators](../../../quantum-information-theory.md#kraus-operator) $T$, let $\Pi_T$ be the [orthogonal projection](../../../hilbert-space.md#orthogonal-projection) onto its image, of [matrix rank](../../../vector-space.md#matrix-rank) $r_T\leq k$. Since $\Pi_TT=T$, the [Cauchy-Schwarz inequality](../../../probability-and-statistics.md#cauchy-schwarz-inequality) for the [Hilbert-Schmidt inner product](../../../compact-operator.md#hilbert-schmidt-inner-product) gives the [rank bound for a weighted operator trace](../../../compact-operator.md#rank-bound-for-a-weighted-operator-trace):

$$
\begin{aligned}
|\operatorname{Tr}(\rho_QT)|^2
&=|\operatorname{Tr}[(\Pi_T\sqrt{\rho_Q})^\dagger(T\sqrt{\rho_Q})]|^2\\
&\leq\operatorname{Tr}(\rho_Q\Pi_T)\operatorname{Tr}(\rho_QT^\dagger T)\\
&\leq\left(\sum_{j<k}\lambda_j\right)\operatorname{Tr}(\rho_QT^\dagger T).
\end{aligned}
$$

The last step uses part (i) at $r_T$, followed by nonnegativity of the [eigenvalues](../../../linear-operator-theory.md#eigenvalue) of the [density operator](../../../quantum-theory.md#density-matrix) $\rho_Q$. Summing over the [Kraus operators](../../../quantum-information-theory.md#kraus-operator) and using their completeness relation proves **the [finite-dimensional quantum compression converse](../../../quantum-information-theory.md#finite-dimensional-quantum-compression-converse)**:

$$
\boxed{1-\epsilon\leq F_{\rm op}(\mathcal D\mathcal C,\rho_Q)^2\leq\sum_{j<k}\lambda_j.}
$$

No invertibility of $\rho_Q$, or restriction to an isometric decoder, was used.

## 3

↑ **Parent:** [Paper 323](paper-323.md)

<h3 id="3/i">i</h3>

↑ **Parent:** [3](#3)

<h4 id="3/i/solution">Solution</h4>

↑ **Parent:** [I](#3/i)

The [absolute value of an operator](../../../banach-algebra.md#absolute-value-of-an-operator), [trace norm](../../../functional-analysis.md#trace-norm), and [operator norm](../../../continuous-dual-space.md#operator-norm) are respectively

$$
|L|=\sqrt{L^\dagger L},\qquad
\|L\|_1=\operatorname{Tr}|L|,\qquad
\|L\|_{\rm op}=\sup_{\|v\|=1}\|Lv\|.
$$

The [positive square root of an operator](../../../hilbert-space.md#positive-square-root-of-an-operator) makes $|L|$ well defined. Its [eigenvalues](../../../linear-operator-theory.md#eigenvalue) $s_j\geq0$ are the [singular values](../../../linear-algebra.md#singular-value) of $L$, so $\|L\|_1=\sum_js_j$ and $\|L\|_{\rm op}=\max_js_j$.

Use the [polar decomposition of a bounded operator](../../../banach-algebra.md#polar-decomposition-of-a-bounded-operator) $L=U|L|$, with the given [unitary operator](../../../vector-space.md#unitary-operator) $U$. In an [orthonormal eigenbasis](../../../linear-operator-theory.md#orthonormal-eigenbasis) $e_j$ for $|L|$,

$$
\operatorname{Tr}(ZL)=\sum_js_j\langle e_j|ZU|e_j\rangle.
$$

The [operator norm](../../../continuous-dual-space.md#operator-norm) assumption and unitarity imply $|\langle e_j|ZU|e_j\rangle|\leq\|Z\|_{\rm op}\leq1$. The [triangle inequality](../../../topological-analysis.md#triangle-inequality) therefore yields **the required trace estimate**:

$$
\boxed{|\operatorname{Tr}(ZL)|\leq\sum_js_j=\|L\|_1.}
$$

Choosing $Z=U^\dagger$ attains equality, which also gives the finite-dimensional [trace duality](../../../compact-operator.md#trace-duality) formula $\|L\|_1=\max_{\|Z\|_{\rm op}\leq1}|\operatorname{Tr}(ZL)|$. A singular $L$ causes no difficulty: in a finite-dimensional square space the polar factor can be extended to a [unitary operator](../../../vector-space.md#unitary-operator) on the complementary subspaces.

<h3 id="3/ii">ii</h3>

↑ **Parent:** [3](#3)

<h4 id="3/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#3/ii)

Let $\Gamma=T_B$ denote the [partial transpose](../../../quantum-information-theory.md#partial-transpose). The [partial transpose of a maximally entangled projector](../../../quantum-information-theory.md#partial-transpose-of-a-maximally-entangled-projector) is

$$
(\phi^+)^\Gamma=\frac1d\sum_{i,j}|i\rangle\langle j|\otimes|j\rangle\langle i|=\frac Sd,
$$

where $S$ is the [swap operator](../../../quantum-information-theory.md#swap-operator), satisfying $S^\dagger S=I$ and $\|S\|_{\rm op}=1$. If $\sigma$ has [positive partial transpose](../../../quantum-information-theory.md#positive-partial-transpose), then $\sigma^\Gamma$ is a [positive operator](../../../hilbert-space.md#positive-operator) of [trace](../../../linear-algebra.md#matrix-trace) one, hence $\|\sigma^\Gamma\|_1=1$.

For a [pure state](../../../quantum-theory.md#pure-state) $\phi^+=|\Phi\rangle\langle\Phi|$, the unsquared [quantum fidelity](../../../quantum-information-theory.md#fidelity-of-quantum-states) obeys $F(\phi^+,\sigma)^2=\langle\Phi|\sigma|\Phi\rangle$. Using the [trace-adjoint identity for partial transpose](../../../quantum-information-theory.md#trace-adjoint-identity-for-partial-transpose) and part (i),

$$
F(\phi^+,\sigma)^2
=\operatorname{Tr}(\phi^+\sigma)
=\frac1d\operatorname{Tr}(S\sigma^\Gamma)
\leq\frac1d\|\sigma^\Gamma\|_1=\frac1d.
$$

The overlap is nonnegative, so taking its square root proves **the [PPT maximally entangled overlap bound](../../../quantum-information-theory.md#ppt-maximally-entangled-overlap-bound)**:

$$
\boxed{F(\phi^+,\sigma)\leq\frac1{\sqrt d}.}
$$

The [product state](../../../bell-state.md#product-state) $|00\rangle\langle00|$ attains the bound, so it is sharp.

<h3 id="3/iii">iii</h3>

↑ **Parent:** [3](#3)

<h4 id="3/iii/a">a</h4>

↑ **Parent:** [Iii](#3/iii)

<h5 id="3/iii/a/solution">Solution</h5>

↑ **Parent:** [A](#3/iii/a)

In the [computational basis](../../../quantum-theory.md#computational-basis) ordered as $00,01,10,11$, the [Hermitian matrix](../../../hilbert-space.md#hermitian-operator) is

$$
\rho_{AB}=\frac12\begin{pmatrix}1&0&0&\alpha\\0&0&0&0\\0&0&0&0\\\alpha&0&0&1\end{pmatrix}.
$$

Its [trace](../../../linear-algebra.md#matrix-trace) is one, and its [eigenvalues](../../../linear-operator-theory.md#eigenvalue) are $(1+\alpha)/2$, $(1-\alpha)/2$, $0$, and $0$. Thus the remaining [density operator](../../../quantum-theory.md#density-matrix) condition, positivity, holds exactly when **both nonzero candidates are nonnegative**:

$$
\boxed{-1\leq\alpha\leq1.}
$$

This is the admissible parameter interval for the [dephased Bell-state mixture](../../../bell-state.md#dephased-bell-state-mixture).

<h4 id="3/iii/b">b</h4>

↑ **Parent:** [Iii](#3/iii)

<h5 id="3/iii/b/solution">Solution</h5>

↑ **Parent:** [B](#3/iii/b)

A [density operator](../../../quantum-theory.md#density-matrix) is a [pure state](../../../quantum-theory.md#pure-state) exactly when its [matrix rank](../../../vector-space.md#matrix-rank) is one. Within the admissible interval from part (a), one of $(1+\alpha)/2$ and $(1-\alpha)/2$ must vanish. Therefore **the pure-state parameters and vectors are**

$$
\boxed{\alpha=1:\quad\rho_{AB}=|\Phi^+\rangle\langle\Phi^+|,\qquad
\alpha=-1:\quad\rho_{AB}=|\Phi^-\rangle\langle\Phi^-|,}
$$

where the [Bell states](../../../bell-state.md) are $|\Phi^\pm\rangle=(|00\rangle\pm|11\rangle)/\sqrt2$. Equivalently, the [purity of a density operator](../../../quantum-theory.md#purity-of-a-density-operator) is $\operatorname{Tr}\rho_{AB}^2=(1+\alpha^2)/2$, reaching one exactly at these two endpoints.

<h4 id="3/iii/c">c</h4>

↑ **Parent:** [Iii](#3/iii)

<h5 id="3/iii/c/solution">Solution</h5>

↑ **Parent:** [C](#3/iii/c)

Every [separable quantum state](../../../quantum-information-theory.md#separable-quantum-state) has [positive partial transpose](../../../quantum-information-theory.md#positive-partial-transpose). Here the [partial transpose](../../../quantum-information-theory.md#partial-transpose) is

$$
\rho_{AB}^{T_B}=\frac12\begin{pmatrix}1&0&0&0\\0&0&\alpha&0\\0&\alpha&0&0\\0&0&0&1\end{pmatrix},
$$

with [eigenvalues](../../../linear-operator-theory.md#eigenvalue) $1/2,1/2,\alpha/2,-\alpha/2$. Any nonzero $\alpha$ therefore gives a negative [eigenvalue](../../../linear-operator-theory.md#eigenvalue), excluding a [separable quantum state](../../../quantum-information-theory.md#separable-quantum-state). At $\alpha=0$, the explicit decomposition

$$
\rho_{AB}=\frac12|0\rangle\langle0|\otimes|0\rangle\langle0|+
\frac12|1\rangle\langle1|\otimes|1\rangle\langle1|
$$

is a mixture of [product states](../../../bell-state.md#product-state). **Consequently**

$$
\boxed{\rho_{AB}\text{ is separable}\iff\alpha=0.}
$$

Only necessity of the [positive partial transpose criterion](../../../quantum-information-theory.md#positive-partial-transpose-criterion) is needed here; sufficiency at zero follows directly from the decomposition.

## 4

↑ **Parent:** [Paper 323](paper-323.md)

<h3 id="4/i">i</h3>

↑ **Parent:** [4](#4)

<h4 id="4/i/solution">Solution</h4>

↑ **Parent:** [I](#4/i)

For any normalized [pure state](../../../quantum-theory.md#pure-state) on finite-dimensional [Hilbert spaces](../../../hilbert-space.md) $\mathcal H_A\otimes\mathcal H_B$, the [Schmidt decomposition](../../../von-neumann-entropy.md#schmidt-decomposition) gives

$$
\boxed{|\psi\rangle_{AB}=\sum_{j=1}^r\sqrt{p_j}\,|u_j\rangle_A|v_j\rangle_B,\qquad
p_j>0,\quad\sum_jp_j=1,\quad r\leq\min(d_A,d_B).}
$$

The $u_j$ and $v_j$ form [orthonormal sets](../../../linear-algebra.md#orthonormal-set) in their respective spaces. The positive numbers $\sqrt{p_j}$ are the [Schmidt coefficients](../../../von-neumann-entropy.md#schmidt-coefficient), and $r$ is the [Schmidt rank](../../../von-neumann-entropy.md#schmidt-rank). Taking a [partial trace](../../../quantum-theory.md#partial-trace) gives the [reduced density matrices](../../../bell-state.md#reduced-density-matrix)

$$
\rho_A=\sum_jp_j|u_j\rangle\langle u_j|,\qquad
\rho_B=\sum_jp_j|v_j\rangle\langle v_j|.
$$

Thus the nonzero [eigenvalues](../../../linear-operator-theory.md#eigenvalue) of the two [reduced density matrices](../../../bell-state.md#reduced-density-matrix) agree.

One construction is a [singular value decomposition](../../../linear-algebra.md#singular-value-decomposition) of the coefficient [matrix](../../../vector-space.md#matrix) $M$ in $|\psi\rangle=\sum_{a,b}M_{ab}|a\rangle|b\rangle$. If $M=U\Sigma V^\dagger$, the columns of $U$ give $u_j$, the complex conjugates of the columns of $V$ give $v_j$, and the [singular values](../../../linear-algebra.md#singular-value) give $\sqrt{p_j}$. This also explains why the [Schmidt coefficients](../../../von-neumann-entropy.md#schmidt-coefficient) are real and nonnegative.

<h3 id="4/ii">ii</h3>

↑ **Parent:** [4](#4)

<h4 id="4/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#4/ii)

The coefficient [matrix](../../../vector-space.md#matrix) in the [computational basis](../../../quantum-theory.md#computational-basis) is

$$
M=\frac1{\sqrt{15}}\begin{pmatrix}2\sqrt2&-1\\\sqrt2&2\end{pmatrix}.
$$

For a bipartite [pure state](../../../quantum-theory.md#pure-state), the [partial traces](../../../quantum-theory.md#partial-trace) give $\psi_A=MM^\dagger$ and $\psi_B=M^T\overline M$. Therefore **the requested reduced density matrices are**

$$
\boxed{\psi_A=\frac1{15}\begin{pmatrix}9&2\\2&6\end{pmatrix},\qquad
\psi_B=\frac1{15}\begin{pmatrix}10&0\\0&5\end{pmatrix}.}
$$

The columns of $M$ are orthogonal. Their norms are $\sqrt{2/3}$ and $\sqrt{1/3}$, so normalizing them gives the [orthonormal set](../../../linear-algebra.md#orthonormal-set)

$$
|u_0\rangle=\frac{2|0\rangle+|1\rangle}{\sqrt5},\qquad
|u_1\rangle=\frac{-|0\rangle+2|1\rangle}{\sqrt5}.
$$

With $|v_0\rangle=|0\rangle$ and $|v_1\rangle=|1\rangle$, a [Schmidt decomposition](../../../von-neumann-entropy.md#schmidt-decomposition) is

$$
\boxed{|\psi\rangle=\sqrt{\frac23}|u_0\rangle|0\rangle+
\sqrt{\frac13}|u_1\rangle|1\rangle.}
$$

Expanding this expression reproduces the minus sign in the $|01\rangle$ coefficient. The two [reduced density matrices](../../../bell-state.md#reduced-density-matrix) both have [eigenvalues](../../../linear-operator-theory.md#eigenvalue) $2/3$ and $1/3$, consistent with these [Schmidt coefficients](../../../von-neumann-entropy.md#schmidt-coefficient).

<h3 id="4/iii">iii</h3>

↑ **Parent:** [4](#4)

<h4 id="4/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#4/iii)

Write $|\zeta\rangle=\sum_{i,j}M_{ij}|i\rangle_A|j\rangle_B$. Normalization says $\|M\|_{\rm HS}=1$, and the [Schmidt rank](../../../von-neumann-entropy.md#schmidt-rank) equals the [matrix rank](../../../vector-space.md#matrix-rank) of $M$. Its nonzero [singular values](../../../linear-algebra.md#singular-value) are therefore $s_1,\ldots,s_r$ with $\sum_js_j^2=1$.

The overlap with the [maximally entangled state](../../../quantum-theory.md#maximally-entangled-state) is $\langle\phi^+|\zeta\rangle=\operatorname{Tr}(M)/\sqrt d$. The [trace norm](../../../functional-analysis.md#trace-norm) estimate of Q3(i), with test [linear operator](../../../vector-space.md#linear-operator) $I$, followed by the [Cauchy-Schwarz inequality](../../../probability-and-statistics.md#cauchy-schwarz-inequality), gives

$$
|\operatorname{Tr}M|\leq\|M\|_1=\sum_{j=1}^rs_j\leq\sqrt{r\sum_js_j^2}=\sqrt r.
$$

For two [pure states](../../../quantum-theory.md#pure-state), the unsquared [quantum fidelity](../../../quantum-information-theory.md#fidelity-of-quantum-states) is the absolute value of their overlap. **Hence the [maximally entangled overlap bound from Schmidt rank](../../../von-neumann-entropy.md#maximally-entangled-overlap-bound-from-schmidt-rank) is**

$$
\boxed{F(|\phi^+\rangle\langle\phi^+|,|\zeta\rangle\langle\zeta|)\leq\sqrt{\frac rd}.}
$$

The bound is attained by $|\zeta\rangle=r^{-1/2}\sum_{j=0}^{r-1}|jj\rangle$. Thus uniform [Schmidt coefficients](../../../von-neumann-entropy.md#schmidt-coefficient) on $r$ aligned basis pairs give the greatest possible overlap for that [Schmidt rank](../../../von-neumann-entropy.md#schmidt-rank).

## 5

↑ **Parent:** [Paper 323](paper-323.md)

<h3 id="5/1">1</h3>

↑ **Parent:** [5](#5)

<h4 id="5/1/solution">Solution</h4>

↑ **Parent:** [1](#5/1)

Use logarithms to base two, so [Von Neumann entropy](../../../von-neumann-entropy.md) and [quantum relative entropy](../../../von-neumann-entropy.md#quantum-relative-entropy) are measured in bits. For [density operators](../../../quantum-theory.md#density-matrix) $\rho,\sigma$,

$$
\boxed{S(\rho)=-\operatorname{Tr}(\rho\log_2\rho),\qquad
D(\rho\|\sigma)=\operatorname{Tr}[\rho(\log_2\rho-\log_2\sigma)].}
$$

The [quantum relative entropy](../../../von-neumann-entropy.md#quantum-relative-entropy) formula applies when the [support of a positive operator](../../../hilbert-space.md#support-of-a-positive-operator) $\rho$ is contained in that of $\sigma$; otherwise $D(\rho\|\sigma)=+\infty$. Use $0\log_2 0=0$ in the [Von Neumann entropy](../../../von-neumann-entropy.md) formula.

The binary [density operator](../../../quantum-theory.md#density-matrix) $\omega[p]$ is diagonal with [eigenvalues](../../../linear-operator-theory.md#eigenvalue) $1-p,p$. Its [Von Neumann entropy](../../../von-neumann-entropy.md) is the [binary entropy](../../../information-theory.md#binary-entropy):

$$
\boxed{S(\omega[p])=h_2(p)=-(1-p)\log_2(1-p)-p\log_2p.}
$$

The two diagonal [density operators](../../../quantum-theory.md#density-matrix) commute, so their [quantum relative entropy](../../../von-neumann-entropy.md#quantum-relative-entropy) is

$$
\boxed{D(\omega[p]\|\omega[q])=(1-p)\log_2\frac{1-p}{1-q}+p\log_2\frac pq.}
$$

A term with zero numerator has value zero; a positive numerator and zero denominator give $+\infty$. In particular, $D(\omega[0]\|\omega[0])=D(\omega[1]\|\omega[1])=0$, whereas $q=0,p>0$ or $q=1,p<1$ gives $+\infty$.

<h3 id="5/2">2</h3>

↑ **Parent:** [5](#5)

<h4 id="5/2/solution">Solution</h4>

↑ **Parent:** [2](#5/2)

Choose $P_X$ uniform on $\mathcal A_M$ and zero outside it, so the marginal [density operator](../../../quantum-theory.md#density-matrix) of $Q$ is $\bar\rho_Q=k^{-1}\sum_m\rho(m)_Q$. Define the [binary test for quantum decoding success](../../../quantum-information-theory.md#binary-test-for-quantum-decoding-success) by

$$
\boxed{F(0)=\sum_{m\in\mathcal A_M}|m\rangle\langle m|_{\widetilde X}\otimes E(m)_Q,\qquad
F(1)=I_{\widetilde XQ}-F(0).}
$$

Each $E(m)$ is a [positive contraction](../../../hilbert-space.md#positive-contraction). The [computational basis](../../../quantum-theory.md#computational-basis) blocks of $F(0)$ are these effects on $\mathcal A_M$ and zero elsewhere. Thus $0\leq F(0)\leq I$, making $F$ a [POVM](../../../quantum-measurement.md#positive-operator-valued-measure) on the whole space, including labels outside $\mathcal A_M$.

On the correlated [classical-quantum state](../../../quantum-information-theory.md#classical-quantum-state), its acceptance probability is

$$
\operatorname{Tr}[F(0)\rho_{\widetilde XQ}]
=\frac1k\sum_m\operatorname{Tr}[E(m)\rho(m)]=1-\epsilon.
$$

On the product of the marginal [density operators](../../../quantum-theory.md#density-matrix),

$$
\operatorname{Tr}[F(0)(\rho_{\widetilde X}\otimes\bar\rho_Q)]
=\frac1k\sum_m\operatorname{Tr}[E(m)\bar\rho_Q]
=\frac1k\operatorname{Tr}\bar\rho_Q=\frac1k,
$$

since $\sum_mE(m)=I_Q$. **The two requested probabilities are therefore $1-\epsilon$ and $1/k$.** In the notation for binary output [density operators](../../../quantum-theory.md#density-matrix), the [measurement channel](../../../quantum-information-theory.md#measurement-channel) sends the joint input to $\omega[\epsilon]$ and the product input to $\omega[1-1/k]$; their parameters describe outcome one, not outcome zero.

<h3 id="5/3">3</h3>

↑ **Parent:** [5](#5)

<h4 id="5/3/solution">Solution</h4>

↑ **Parent:** [3](#5/3)

For the distribution and [POVM](../../../quantum-measurement.md#positive-operator-valued-measure) from part 2, apply the [data-processing inequality for quantum relative entropy](../../../von-neumann-entropy.md#data-processing-inequality-for-quantum-relative-entropy) to the [measurement channel](../../../quantum-information-theory.md#measurement-channel). The [quantum mutual information](../../../von-neumann-entropy.md#quantum-mutual-information) is the [quantum relative entropy](../../../von-neumann-entropy.md#quantum-relative-entropy) from the joint [density operator](../../../quantum-theory.md#density-matrix) to the product of its marginals, so for $k\geq2$,

$$
\begin{aligned}
I(\widetilde X:Q)_\rho
&=D(\rho_{\widetilde XQ}\|\rho_{\widetilde X}\otimes\bar\rho_Q)\\
&\geq D(\omega[\epsilon]\|\omega[1-1/k])\\
&=(1-\epsilon)\log_2 k-h_2(\epsilon)-\epsilon\log_2(1-1/k)\\
&\geq(1-\epsilon)\log_2 k-1.
\end{aligned}
$$

The last step uses $h_2(\epsilon)\leq1$ for the [binary entropy](../../../information-theory.md#binary-entropy) and $\log_2(1-1/k)\leq0$. If $0\leq\epsilon<1$, rearrangement and then the supremum over $P_X$ give **the [one-shot classical-quantum coding converse](../../../quantum-information-theory.md#one-shot-classical-quantum-coding-converse)**:

$$
\boxed{\log_2 k\leq\frac{I(\widetilde X:Q)_\rho+1}{1-\epsilon}
\leq\frac{\sup_{P_X}I(\widetilde X:Q)_{\rho_{\widetilde XQ}}+1}{1-\epsilon}.}
$$

For $k=1$, the sole [POVM](../../../quantum-measurement.md#positive-operator-valued-measure) effect is $I_Q$, forcing $\epsilon=0$, and the bound is trivial. For $\epsilon=1$, division by $1-\epsilon$ is undefined: the undivided inequality remains valid and gives no size restriction. The displayed coding bound is therefore understood for $\epsilon<1$, or with a vacuous $+\infty$ right-hand side at $\epsilon=1$.

An alternative uses the original decoder directly. Let $M$ be the uniform message and $\widehat M$ its measured estimate. For $k\geq2$, [Fano's inequality](../../../information-theory.md#fano-s-inequality) bounds the [conditional entropy](../../../information-theory.md#conditional-entropy) by $H(M|\widehat M)\leq h_2(\epsilon)+\epsilon\log_2(k-1)$. The [Holevo bound](../../../quantum-information-theory.md#holevo-s-theorem) gives

$$
I(\widetilde X:Q)_\rho\geq I(M:\widehat M)
=\log_2 k-H(M|\widehat M)
\geq\log_2 k-h_2(\epsilon)-\epsilon\log_2(k-1)
\geq(1-\epsilon)\log_2 k-1.
$$

Thus the same coding bound follows by bounding the classical [mutual information](../../../information-theory.md#mutual-information) obtainable from the [POVM](../../../quantum-measurement.md#positive-operator-valued-measure).

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2016](../../2016.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
