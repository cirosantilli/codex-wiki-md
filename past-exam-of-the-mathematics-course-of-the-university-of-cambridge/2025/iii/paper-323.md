# Paper 323

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2025/III_Paper_323.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2025/III_Paper_323.pdf)

**Table of contents**

- [1](#1)
  - [i](#1/i)
    - [Solution](#1/i/solution)
  - [ii](#1/ii)
    - [Solution](#1/ii/solution)
  - [iii](#1/iii)
    - [Solution](#1/iii/solution)
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
  - [i](#3/i)
    - [Solution](#3/i/solution)
  - [ii](#3/ii)
    - [a](#3/ii/a)
      - [Solution](#3/ii/a/solution)
    - [b](#3/ii/b)
      - [Solution](#3/ii/b/solution)
    - [c](#3/ii/c)
      - [Solution](#3/ii/c/solution)
    - [d](#3/ii/d)
      - [Solution](#3/ii/d/solution)
- [4](#4)
  - [i](#4/i)
    - [Solution](#4/i/solution)
  - [ii](#4/ii)
    - [Solution](#4/ii/solution)
  - [iii](#4/iii)
    - [Solution](#4/iii/solution)

## 1

↑ **Parent:** [Paper 323](paper-323.md)

<h3 id="1/i">i</h3>

↑ **Parent:** [1](#1)

<h4 id="1/i/solution">Solution</h4>

↑ **Parent:** [I](#1/i)

In [quantum channel discrimination](../../../quantum-information-theory.md#quantum-channel-discrimination), prepare a [density operator](../../../quantum-theory.md#density-matrix) $\rho_{HR}$ on the channel input $H$ and an optional [quantum ancilla](../../../quantum-information-theory.md#quantum-ancilla) $R$. Under hypothesis $j\in\{1,2\}$ the output is

$$
\omega_j=(T_j\otimes\operatorname{id}_R)(\rho_{HR}).
$$

Use a two-outcome [measurement in quantum mechanics](../../../quantum-measurement.md) $\{Q,I-Q\}$ and decide for $T_1$ on outcome $Q$. The conditional [Type I error](../../../information-theory.md#type-i-and-type-ii-errors) and [Type II error](../../../information-theory.md#type-i-and-type-ii-errors) are

$$
\alpha=\operatorname{Tr}[(I-Q)\omega_1],
\qquad
\beta=\operatorname{Tr}[Q\omega_2].
$$

With [prior probabilities](../../../statistical-inference.md#prior-probability) $p$ and $1-p$, symmetric Bayesian discrimination minimizes the average error $p\alpha+(1-p)\beta$ over the input and measurement.

<h3 id="1/ii">ii</h3>

↑ **Parent:** [1](#1)

<h4 id="1/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#1/ii)

For a fixed input, the [Holevo–Helstrom theorem](../../../quantum-information-theory.md#holevo-helstrom-theorem) gives the optimal error for the two output states. Optimizing the input and [quantum ancilla](../../../quantum-information-theory.md#quantum-ancilla) therefore gives

$$
\boxed{
P_{\mathrm{err}}^{\mathrm{anc}}
=\frac12\left(1-\left\|pT_1-(1-p)T_2\right\|_\diamond\right)}.
$$

The stabilization in the [diamond norm](../../../functional-analysis.md#diamond-norm) is exactly the optimization over ancillary systems. Without an ancilla the same argument instead gives

$$
\boxed{
P_{\mathrm{err}}^{\mathrm{no\ anc}}
=\frac12\left(1-\left\|pT_1-(1-p)T_2\right\|_1\right)},
$$

where $\|\cdot\|_1$ is the [induced trace norm](../../../functional-analysis.md#induced-trace-norm).

<h3 id="1/iii">iii</h3>

↑ **Parent:** [1](#1)

<h4 id="1/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#1/iii)

For $p=(d+1)/(2d)$, the weighted difference of the two [Werner–Holevo channels](../../../quantum-information-theory.md#werner-holevo-channel) is

$$
\begin{aligned}
\bigl(pT_+-(1-p)T_-\bigr)(X)
&=\frac1{2d}\bigl(\operatorname{Tr}(X)I+X^T\bigr)
-\frac1{2d}\bigl(\operatorname{Tr}(X)I-X^T\bigr)\\
&=\frac1dX^T.
\end{aligned}
$$

Thus the map is the [transposition map](../../../vector-space.md#transpose) divided by $d$. The [diamond norm of the transposition map](../../../quantum-information-theory.md#diamond-norm-of-the-transposition-map) and invariance of the [trace norm](../../../functional-analysis.md#trace-norm) under [matrix transpose](../../../vector-space.md#transpose) give

$$
\boxed{\|pT_+-(1-p)T_-\|_\diamond
=\frac1d\|\Theta\|_\diamond=1},
\qquad
\boxed{\|pT_+-(1-p)T_-\|_1
=\frac1d\|\Theta\|_1=\frac1d}.
$$

Substitution into the optimal-error formulas shows that an entangled [quantum ancilla](../../../quantum-information-theory.md#quantum-ancilla) permits perfect discrimination, whereas every ancilla-free strategy has

$$
\boxed{P_{\mathrm{err}}^{\mathrm{no\ anc}}=\frac12\left(1-\frac1d\right)}.
$$

## 2

↑ **Parent:** [Paper 323](paper-323.md)

<h3 id="2/i">i</h3>

↑ **Parent:** [2](#2)

<h4 id="2/i/solution">Solution</h4>

↑ **Parent:** [I](#2/i)

A bipartite [density operator](../../../quantum-theory.md#density-matrix) is a [separable quantum state](../../../quantum-information-theory.md#separable-quantum-state) when it has a [convex combination](../../../mathematical-optimization.md#convex-combination) decomposition

$$
\rho_{AB}=\sum_rq_r\,\rho_r^A\otimes\rho_r^B,
\qquad q_r\geq0,\qquad\sum_rq_r=1,
$$

into [product states](../../../bell-state.md#product-state). A state for which no such decomposition exists is an [entangled state](../../../bell-state.md#entangled-state).

<h3 id="2/ii">ii</h3>

↑ **Parent:** [2](#2)

<h4 id="2/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#2/ii)

The [positive partial transpose criterion](../../../quantum-information-theory.md#positive-partial-transpose-criterion) states that every [separable quantum state](../../../quantum-information-theory.md#separable-quantum-state) satisfies

$$
\rho_{AB}^{T_B}\geq0.
$$

Consequently, a negative [eigenvalue](../../../linear-operator-theory.md#eigenvalue) of the [partial transpose](../../../quantum-information-theory.md#partial-transpose) proves entanglement. Positivity of the partial transpose is also sufficient for separability in dimensions $2\otimes2$ and $2\otimes3$, equivalently $3\otimes2$, but it is not sufficient in general higher dimensions.

<h3 id="2/iii">iii</h3>

↑ **Parent:** [2](#2)

<h4 id="2/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#2/iii)

Each rank-one [density operator](../../../quantum-theory.md#density-matrix) is

$$
|z\rangle\langle z|
=\frac1d\sum_{j,k}z_jz_k^*|j\rangle\langle k|,
\qquad
|z^*\rangle\langle z^*|
=\frac1d\sum_{j',k'}z_{j'}^*z_{k'}|j'\rangle\langle k'|.
$$

Taking their [tensor product](../../../linear-algebra.md#tensor-product) and averaging over the $4^d$ independent choices of the fourth roots of unity gives

$$
\boxed{
\sigma
=\frac1{4^dd^2}
\sum_{j,k,j',k'}
\left(\sum_z z_jz_k^*z_{j'}^*z_{k'}\right)
|j\rangle\langle k|\otimes|j'\rangle\langle k'|}.
$$

This is the claimed expansion in [matrix elements](../../../vector-space.md#matrix-element).

<h3 id="2/iv">iv</h3>

↑ **Parent:** [2](#2)

<h4 id="2/iv/solution">Solution</h4>

↑ **Parent:** [Iv](#2/iv)

The average of $z_jz_k^*z_{j'}^*z_{k'}$ vanishes unless the exponent of every independent fourth root is balanced modulo four. The surviving index patterns are $j=k,\ j'=k'$ and $j=j',\ k=k'$. Their intersection $j=k=j'=k'$ has been counted twice. Hence, writing

$$
D=\sum_{j=1}^d|j\rangle\langle j|\otimes|j\rangle\langle j|,
$$

the phase average is

$$
\sigma=\frac1{d^2}\left(I\otimes I
+d|\Phi^+\rangle\langle\Phi^+|-D\right).
$$

Solving for the projector onto the [maximally entangled state](../../../quantum-theory.md#maximally-entangled-state) gives

$$
\boxed{
|\Phi^+\rangle\langle\Phi^+|
=d\sigma-\frac1dI\otimes I+\frac1dD}.
$$

<h3 id="2/v">v</h3>

↑ **Parent:** [2](#2)

<h4 id="2/v/solution">Solution</h4>

↑ **Parent:** [V](#2/v)

At the proposed boundary $p_0=1/(d+1)$, the identity from part (iv) yields

$$
\rho_{p_0}
=\frac{d}{d+1}\sigma
+\frac1{d+1}\frac Dd.
$$

Both $\sigma$ and $D/d$ are [convex combinations](../../../mathematical-optimization.md#convex-combination) of [product states](../../../bell-state.md#product-state), so $\rho_{p_0}$ is a [separable quantum state](../../../quantum-information-theory.md#separable-quantum-state). For $0\leq p\leq p_0$, the state $\rho_p$ is a convex combination of $\rho_{p_0}$ and the maximally mixed product state $I/d^2$, and is therefore separable.

For the converse, the [partial transpose](../../../quantum-information-theory.md#partial-transpose) of the maximally entangled projector is $F/d$, where $F$ is the [swap operator](../../../quantum-information-theory.md#swap-operator). Therefore

$$
\rho_p^{T_B}=\frac pdF+\frac{1-p}{d^2}I.
$$

On the antisymmetric subspace, $F$ has eigenvalue $-1$, so the corresponding eigenvalue of $\rho_p^{T_B}$ is

$$
\frac{1-p}{d^2}-\frac pd,
$$

which is negative exactly when $p>1/(d+1)$. The [positive partial transpose criterion](../../../quantum-information-theory.md#positive-partial-transpose-criterion) then proves that $\rho_p$ is entangled. Thus

$$
\boxed{\rho_p\text{ is separable exactly when }p\leq\frac1{d+1}}.
$$

## 3

↑ **Parent:** [Paper 323](paper-323.md)

<h3 id="3/i">i</h3>

↑ **Parent:** [3](#3)

<h4 id="3/i/solution">Solution</h4>

↑ **Parent:** [I](#3/i)

Apply the assumed [data-processing inequality for quantum relative entropy](../../../von-neumann-entropy.md#data-processing-inequality-for-quantum-relative-entropy) to the normalized [partial trace](../../../quantum-theory.md#partial-trace) over $C$, with the two input states

$$
\rho_{ABC},
\qquad
\frac{I_A}{d_A}\otimes\rho_{BC}.
$$

The channel sends them to $\rho_{AB}\otimes I_C/d_C$ and $I_A/d_A\otimes\rho_B\otimes I_C/d_C$. Additivity over the common maximally mixed factor reduces data processing to

$$
D\left(\rho_{ABC}\middle\|\frac{I_A}{d_A}\otimes\rho_{BC}\right)
\geq
D\left(\rho_{AB}\middle\|\frac{I_A}{d_A}\otimes\rho_B\right).
$$

Expanding the [Umegaki relative entropy](../../../von-neumann-entropy.md#quantum-relative-entropy) in terms of [Von Neumann entropy](../../../von-neumann-entropy.md) gives

$$
-S(\rho_{ABC})+\log d_A+S(\rho_{BC})
\geq
-S(\rho_{AB})+\log d_A+S(\rho_B).
$$

After cancelling $\log d_A$, this is precisely the [Strong subadditivity of Von Neumann entropy](../../../von-neumann-entropy.md#strong-subadditivity-of-quantum-entropy)

$$
\boxed{S(\rho_B)+S(\rho_{ABC})
\leq S(\rho_{AB})+S(\rho_{BC})}.
$$

<h3 id="3/ii">ii</h3>

↑ **Parent:** [3](#3)

<h4 id="3/ii/a">a</h4>

↑ **Parent:** [Ii](#3/ii)

<h5 id="3/ii/a/solution">Solution</h5>

↑ **Parent:** [A](#3/ii/a)

A real function $f$ on $I=[0,1]$ is an [operator convex function](../../../real-analysis.md#operator-convex-function) when, for all [Hermitian operators](../../../hilbert-space.md#hermitian-operator) $X,Y$ whose spectra lie in $I$ and every $0\leq\lambda\leq1$,

$$
\boxed{
f(\lambda X+(1-\lambda)Y)
\preceq\lambda f(X)+(1-\lambda)f(Y)},
$$

where $\preceq$ is the [Loewner order](../../../linear-algebra.md#loewner-order). Reversing the inequality defines an [operator concave function](../../../real-analysis.md#operator-concave-function), equivalently $-f$ is operator convex.

<h4 id="3/ii/b">b</h4>

↑ **Parent:** [Ii](#3/ii)

<h5 id="3/ii/b/solution">Solution</h5>

↑ **Parent:** [B](#3/ii/b)

Because the two flags $E_C$ and $F_C$ are [orthogonal projections](../../../hilbert-space.md#orthogonal-projection), the flagged state is block diagonal. If $h(\lambda)$ denotes the [binary entropy](../../../information-theory.md#binary-entropy), then

$$
S(\rho_{ABC})
=h(\lambda)+\lambda S(\rho'_{AB})
+(1-\lambda)S(\rho''_{AB}),
$$

and

$$
S(\rho_{BC})
=h(\lambda)+\lambda S(\rho'_B)
+(1-\lambda)S(\rho''_B).
$$

Its unflagged marginals are $\rho_{AB}=\lambda\rho'_{AB}+(1-\lambda)\rho''_{AB}$ and $\rho_B=\lambda\rho'_B+(1-\lambda)\rho''_B$. Substitution in [Strong subadditivity of Von Neumann entropy](../../../von-neumann-entropy.md#strong-subadditivity-of-quantum-entropy) cancels the two binary-entropy terms and gives

$$
\boxed{
H(A|B)_{\lambda\rho'+(1-\lambda)\rho''}
\geq
\lambda H(A|B)_{\rho'}
+(1-\lambda)H(A|B)_{\rho''}}.
$$

This is exactly the [concavity of quantum conditional entropy](../../../von-neumann-entropy.md#concavity-of-quantum-conditional-entropy).

<h4 id="3/ii/c">c</h4>

↑ **Parent:** [Ii](#3/ii)

<h5 id="3/ii/c/solution">Solution</h5>

↑ **Parent:** [C](#3/ii/c)

For $t>0$, [positive homogeneity](../../../real-analysis.md#positively-homogeneous-function-degree-one) and [concavity](../../../real-analysis.md#concave-function) give

$$
\begin{aligned}
f(X+tY)
&=(1+t)f\left(\frac{X}{1+t}+\frac{tY}{1+t}\right)\\
&\geq(1+t)\left(\frac1{1+t}f(X)+\frac t{1+t}f(Y)\right)\\
&=f(X)+tf(Y).
\end{aligned}
$$

After subtracting $f(X)$, dividing by $t$, and taking the one-sided [directional derivative](../../../calculus.md#directional-derivative) at zero,

$$
\boxed{\left.\frac d{dt}\right|_{t=0^+}f(X+tY)\geq f(Y)}.
$$

<h4 id="3/ii/d">d</h4>

↑ **Parent:** [Ii](#3/ii)

<h5 id="3/ii/d/solution">Solution</h5>

↑ **Parent:** [D](#3/ii/d)

Extend the [quantum conditional entropy](../../../von-neumann-entropy.md#quantum-conditional-entropy) from normalized states to positive operators by

$$
F(X_{AB})
=-\operatorname{Tr}(X_{AB}\log X_{AB})
+\operatorname{Tr}(X_B\log X_B).
$$

Since $\operatorname{Tr}X_{AB}=\operatorname{Tr}X_B$, the two terms involving $\log t$ cancel under $X\mapsto tX$, so $F(tX)=tF(X)$. Thus $F$ is [positively homogeneous](../../../real-analysis.md#positively-homogeneous-function-degree-one), and part (b) extends its [concavity](../../../real-analysis.md#concave-function) from states to the positive cone.

Apply part (c) with $X=\sigma_{AB}$ and $Y=\rho_{AB}$. Differentiating the [matrix logarithm](../../../vector-space.md#matrix-logarithm) under the trace gives

$$
\left.\frac d{dt}\right|_{t=0}F(\sigma+t\rho)
=-\operatorname{Tr}(\rho\log\sigma)
+\operatorname{Tr}(\rho_B\log\sigma_B).
$$

The inequality from part (c), after moving $F(\rho)$ to the left, becomes

$$
\boxed{
D(\rho_{AB}\|\sigma_{AB})
\geq D(\rho_B\|\sigma_B)}.
$$

This is the [data-processing inequality for quantum relative entropy](../../../von-neumann-entropy.md#data-processing-inequality-for-quantum-relative-entropy) under [partial trace](../../../quantum-theory.md#partial-trace). Tensoring each output with the appropriate maximally mixed state does not change either side, so it also proves data processing under normalized partial traces. Singular $\sigma$ follows by approximation on its support.

## 4

↑ **Parent:** [Paper 323](paper-323.md)

<h3 id="4/i">i</h3>

↑ **Parent:** [4](#4)

<h4 id="4/i/solution">Solution</h4>

↑ **Parent:** [I](#4/i)

The [Umegaki relative entropy](../../../von-neumann-entropy.md#quantum-relative-entropy) is

$$
D(\rho\|\sigma)
=\operatorname{Tr}\rho(\log\rho-\log\sigma)
$$

when the support of $\rho$ is contained in that of $\sigma$, and $+\infty$ otherwise. Its [additivity of quantum relative entropy](../../../von-neumann-entropy.md#additivity-of-quantum-relative-entropy) is

$$
D(\rho_A\otimes\rho_B\|\sigma_A\otimes\sigma_B)
=D(\rho_A\|\sigma_A)+D(\rho_B\|\sigma_B),
$$

its [superadditivity of quantum relative entropy](../../../von-neumann-entropy.md#superadditivity-of-quantum-relative-entropy) is

$$
D(\rho_{AB}\|\sigma_A\otimes\sigma_B)
\geq D(\rho_A\|\sigma_A)+D(\rho_B\|\sigma_B),
$$

and its [data-processing inequality for quantum relative entropy](../../../von-neumann-entropy.md#data-processing-inequality-for-quantum-relative-entropy) is $D(T(\rho)\|T(\sigma))\leq D(\rho\|\sigma)$ for every [quantum channel](../../../quantum-information-theory.md#quantum-channel) $T$.

Additivity follows from the logarithm of a [tensor product](../../../linear-algebra.md#tensor-product),

$$
\log(\rho_A\otimes\rho_B)
=\log\rho_A\otimes I+I\otimes\log\rho_B,
$$

and the analogous identity for $\sigma_A\otimes\sigma_B$. For superadditivity, subtract the two marginal relative entropies from the joint one. The reference-state terms cancel, leaving

$$
S(\rho_A)+S(\rho_B)-S(\rho_{AB})
=I(A:B)_\rho\geq0.
$$

This is the nonnegativity of [quantum mutual information](../../../von-neumann-entropy.md#quantum-mutual-information), equivalently [Subadditivity of Von Neumann entropy](../../../von-neumann-entropy.md#subadditivity-of-von-neumann-entropy).

<h3 id="4/ii">ii</h3>

↑ **Parent:** [4](#4)

<h4 id="4/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#4/ii)

Apply bipartite [superadditivity of quantum relative entropy](../../../von-neumann-entropy.md#superadditivity-of-quantum-relative-entropy) first to system $1$ and systems $2,\ldots,n$, and then repeat on the remaining joint state. [Mathematical induction](../../../foundations-of-mathematics.md#mathematical-induction) gives

$$
\boxed{
D(\rho_{1\ldots n}\|
\sigma_1\otimes\cdots\otimes\sigma_n)
\geq\sum_{j=1}^nD(\rho_j\|\sigma_j)}.
$$

This is [multipartite superadditivity of quantum relative entropy](../../../von-neumann-entropy.md#multipartite-superadditivity-of-quantum-relative-entropy). Repeated application of bipartite additivity similarly gives

$$
\boxed{
D(\rho_1\otimes\cdots\otimes\rho_n\|
\sigma_1\otimes\cdots\otimes\sigma_n)
=\sum_{j=1}^nD(\rho_j\|\sigma_j)}.
$$

<h3 id="4/iii">iii</h3>

↑ **Parent:** [4](#4)

<h4 id="4/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#4/iii)

Let $\rho'_{n,j}$ be the $j$th one-system marginal of $\rho'_n$, and put $\varepsilon_n=\|\rho'_n-\rho^{\otimes n}\|_1$. Contractivity of [trace distance](../../../quantum-theory.md#trace-distance) under [partial trace](../../../quantum-theory.md#partial-trace) gives

$$
\|\rho'_{n,j}-\rho\|_1\leq\varepsilon_n
$$

uniformly in $j$. Because the one-system state space is a [compact space](../../../topology.md#compact-space), continuity of $f(\,\cdot\,\|\sigma)$ implies [uniform continuity](../../../topological-analysis.md#uniform-continuity). Hence there is a function $\delta(\varepsilon)\to0$ such that

$$
f(\rho'_{n,j}\|\sigma)
\geq f(\rho\|\sigma)-\delta(\varepsilon_n)
$$

for every $j$.

Multipartite superadditivity and additivity now imply

$$
\begin{aligned}
f(\rho'_n\|\sigma^{\otimes n})
&\geq\sum_{j=1}^nf(\rho'_{n,j}\|\sigma)\\
&\geq n f(\rho\|\sigma)-n\delta(\varepsilon_n),\\
f(\rho^{\otimes n}\|\sigma^{\otimes n})
&=n f(\rho\|\sigma).
\end{aligned}
$$

Therefore

$$
\frac1n\left(
f(\rho'_n\|\sigma^{\otimes n})
-f(\rho^{\otimes n}\|\sigma^{\otimes n})\right)
\geq-\delta(\varepsilon_n)\longrightarrow0,
$$

which proves the required [lower asymptotic semicontinuity of quantum relative entropy](../../../von-neumann-entropy.md#lower-asymptotic-semicontinuity-of-quantum-relative-entropy) argument.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2025](../../2025.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
