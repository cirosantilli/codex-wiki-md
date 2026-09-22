<h1 id="4/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

For [first-order two-local Hamiltonian simulation](../../../../../../first-order-two-local-hamiltonian-simulation.md), regard each term $H_k$ as a [Hermitian operator](../../../../../../hermitian-operator.md), as is standard for a local-Hamiltonian decomposition. The [Lie-Trotter product formula](../../../../../../lie-product-formula.md) for bounded operators states

$$
e^{\sum_k A_k}=\lim_{r\to\infty}\left(e^{A_M/r}\cdots e^{A_1/r}\right)^r
$$

in [operator norm](../../../../../../operator-norm.md); the reversed factor ordering is just as valid as the displayed one. Take $A_k=-iH_k$ and use the circuit

$$
V_r=\left(e^{-iH_M/r}\cdots e^{-iH_1/r}\right)^r.
$$

Each factor is a [unitary operator](../../../../../../unitary-operator.md) on at most two [qubits](../../../../../../qubit.md) and hence is one allowed two-[qubit](../../../../../../qubit.md) gate, with a spectator identity for a one-[qubit](../../../../../../qubit.md) term. The factors in the rightmost part of each written product act first. Merely quoting the limit would not establish the requested rate, so we give a quantitative error bound.

For two [Hermitian operators](../../../../../../hermitian-operator.md) $A,B$ and $t\geq0$, differentiating

$$
F(s)=e^{-i(t-s)(A+B)}e^{-isA}e^{-isB},\qquad0\leq s\leq t,
$$

gives $F'(s)=i e^{-i(t-s)(A+B)}[B,e^{-isA}]e^{-isB}$. The [commutator](../../../../../../commutator.md) identity obtained by differentiating $e^{iuA}Be^{-iuA}$ implies $\|[B,e^{-isA}]\|\leq s\|[A,B]\|$. Since the surrounding factors are unitary, integration yields the [first-order unitary product-formula error bound](../../../../../../first-order-unitary-product-formula-error-bound.md)

$$
\|e^{-it(A+B)}-e^{-itA}e^{-itB}\|\leq\frac{t^2}{2}\|[A,B]\|.
$$

Splitting the terms successively and using the triangle inequality therefore gives the one-step estimate

$$
\left\|e^{-iH/r}-e^{-iH_M/r}\cdots e^{-iH_1/r}\right\|
\leq\frac1{2r^2}\sum_{k<\ell}\|[H_k,H_\ell]\|
<\frac{M(M-1)}{2r^2},
$$

for $M>1$. Here [submultiplicativity of the operator norm](../../../../../../submultiplicativity-of-the-operator-norm.md) gives $\|[H_k,H_\ell]\|\leq2\|H_k\|\|H_\ell\|<2$. The ordering chosen for the products changes the sign of local commutators, not this norm bound. Applying part (i) to the $r$ steps gives

$$
\boxed{\|e^{-iH}-V_r\|\leq\frac1{2r}\sum_{k<\ell}\|[H_k,H_\ell]\|
<\frac{M(M-1)}{2r}.}
$$

Choose $r=\max(1,\lceil M(M-1)/(2\epsilon)\rceil)$. For $M>1$ the error is strictly below $\epsilon$; $M=1$ is exact already with $r=1$. The [quantum circuit](../../../../../../quantum-circuit-split.md) contains $Mr$ two-[qubit](../../../../../../qubit.md) gates. **A sufficient gate count is**

$$
\boxed{Mr=O\!\left(M+\frac{M^3}{\epsilon}\right)
=O\!\left(\frac{n^6}{\epsilon}\right),\qquad0<\epsilon\leq1.}
$$

Thus the worst-case polynomial degree in this first-order bound is six. Terms with disjoint supports commute and may improve the count in particular decompositions, but the stated assumptions alone suffice for this bound, without a further sparsity or bounded-degree condition. The requested gate model allows arbitrary two-[qubit](../../../../../../qubit.md) unitaries, so no additional compilation error is incurred here.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [4](../../4.md)
3. [Paper 324](../../../paper-324-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
