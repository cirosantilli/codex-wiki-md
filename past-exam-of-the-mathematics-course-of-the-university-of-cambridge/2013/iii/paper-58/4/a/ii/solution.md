<h1 id="4/a/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

The printed upper summation limit introduces $Z_n$ although only qubits $0,\ldots,n-1$ were defined. Literally the final term is undefined. Use the natural open-chain repair

$$
H_{\rm open}=\sum_{i=1}^{n-1}h_i,\qquad h_i=X_{i-1}Z_i.
$$

This preserves the stated $n$-qubit system and agrees with the supplied sum-of-squares hint. If a cyclic convention $Z_n=Z_0$ was intended instead, it must be stated; the same argument works for its $n$ terms when $n\ge2$. For $n=1$, the repaired open chain is empty and the target is the identity.

Here is a [product-formula Hamiltonian simulation](../../../../../../../product-formula-hamiltonian-simulation.md) using exactly the two supplied lemmas. Let $L=n-1$ and choose an integer $r\ge L$. Every $h_i$ is a norm-one [Hermitian matrix](../../../../../../../hermitian-operator.md). One time slice is the product of [two-qubit gates](../../../../../../../two-qubit-gate.md)

$$
P_r=e^{ih_1/r}\cdots e^{ih_L/r},\qquad\widetilde U=P_r^r.
$$

To compare a partial product with $e^{i(h_1+\cdots+h_j)/r}$, first propagate the previous error through the next [unitary gate](../../../../../../../quantum-logic-gate.md), which preserves the [spectral norm](../../../../../../../matrix-2-norm.md), and then use Lemma A with $A=-(h_1+\cdots+h_{j-1})/r$, $B=-h_j/r$. Both [norms](../../../../../../../norm.md) are at most $j/r\le1$. Its new error is at most $c(j/r)^2$ for a universal constant $c$. For an explicit choice, $c=4$ follows from the unitary Taylor bounds $\|e^{iA}-I-iA\|\le\|A\|^2/2$ and $\|e^{iA}-I\|\le\|A\|$. Induction and the [triangle inequality](../../../../../../../triangle-inequality.md) therefore give

$$
\|P_r-e^{iH_{\rm open}/r}\|\le\frac c{r^2}\sum_{j=2}^{L}j^2=O\!\left(\frac{L^3}{r^2}\right).
$$

Lemma B, the [unitary product telescoping](../../../../../../../unitary-product-telescoping.md) bound, now compares the $r$ repeated slices with $(e^{iH_{\rm open}/r})^r=e^{iH_{\rm open}}$:

$$
\|\widetilde U-e^{iH_{\rm open}}\|\le\frac{c\sum_{j=2}^{L}j^2}{r}.
$$

Take, for example, $r=\max(1,L,\lceil2c\sum_{j=2}^{L}j^2/\epsilon\rceil)$. If the sum is zero the product is already exact; otherwise its error is at most $\epsilon/2<\epsilon$. There are $Lr$ [two-qubit gates](../../../../../../../two-qubit-gate.md). **This explicit lemma-based construction has fourth-degree dependence on $n$ for fixed precision:**

$$
\boxed{\text{gate count}=O(n^2+n^4/\epsilon),\qquad\|U-\widetilde U\|<\epsilon.}
$$

This is a sufficient polynomial, not an optimality claim. The polynomial-degree statement treats $\epsilon$ as fixed; the inverse-precision dependence is displayed separately. No first-order term error is accumulated without the required repeated-slice factor.

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [A](../../a.md)
3. [4](../../../4.md)
4. [Paper 58](../../../../paper-58-split.md)
5. [Iii](../../../../split.md)
6. [2013](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
