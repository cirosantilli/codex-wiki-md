<h1 id="3/a/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

The printed sum contains $Z_n$ although the stated labels end at $n-1$. We use the natural periodic convention $Z_n=Z_0$, with $n\geq3$. If an open chain was intended, omitting the final term gives the same asymptotic bound.

Set $H_j=X_{j-1}Z_j$, with indices modulo $n$, and implement the [product-formula Hamiltonian simulation](../../../../../../../product-formula-hamiltonian-simulation.md)

$$
\widetilde U=\left(\prod_{j=1}^n e^{-iH_j/k}\right)^k.
$$

Each factor acts on two [qubits](../../../../../../../qubit.md), so it is a two-qubit [unitary operator](../../../../../../../unitary-operator.md). More explicitly, if $a=j-1$, $b=j$, and $C_{a\to b}$ is a [controlled-NOT gate](../../../../../../../controlled-not-gate.md),

$$
e^{-i\delta X_aZ_b}
=\mathsf H_a C_{a\to b}\,e^{-i\delta Z_b}\,C_{a\to b}\mathsf H_a,
$$

where $\mathsf H_a$ is a [Hadamard gate](../../../../../../../hadamard-gate.md). This gives a constant number of one-qubit and two-qubit gates per factor; one-qubit gates can also be viewed as two-qubit gates tensored with the identity.

The [spectral norm](../../../../../../../matrix-2-norm.md) obeys the [triangle inequality](../../../../../../../triangle-inequality.md), [submultiplicativity of the operator norm](../../../../../../../submultiplicativity-of-the-operator-norm.md), and invariance under multiplication by [unitary operators](../../../../../../../unitary-operator.md). In particular, the [telescoping bound for products of operators](../../../../../../../telescoping-bound-for-products-of-operators.md) gives $\|V^k-W^k\|\leq k\|V-W\|$ for unitary $V,W$. The [first-order unitary product-formula error bound](../../../../../../../first-order-unitary-product-formula-error-bound.md) consequently yields

$$
\|U-\widetilde U\|\leq\frac1{2k}\sum_{j<l}\|[H_j,H_l]\|.
$$

Only neighboring terms can have a nonzero [commutator](../../../../../../../commutator.md), because all other supports are disjoint. There are $n$ neighboring unordered pairs, and $\|[H_j,H_l]\|\leq2\|H_j\|\|H_l\|=2$. Thus $\|U-\widetilde U\|\leq n/k$. Choosing $k>n/\varepsilon$ gives

$$
\boxed{O(n^2/\varepsilon)\text{ gates},\qquad\text{degree }2\text{ in }n\text{ for fixed }\varepsilon.}
$$

The coarser bound that counts all $\binom n2$ pairs also proves the often-used $O(n^3/\varepsilon)$ construction. Locality improves that cubic estimate to the quadratic bound above; neither assertion is a lower bound on the best possible circuit.

## ↑ Ancestors (12)

1. [Iii](../iii.md)
2. [A](../../a.md)
3. [3](../../../3.md)
4. [Paper 324](../../../../paper-324-split.md)
5. [Iii](../../../../split.md)
6. [2019](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
