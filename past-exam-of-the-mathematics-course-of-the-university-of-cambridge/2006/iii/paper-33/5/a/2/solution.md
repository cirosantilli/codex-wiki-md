<h1 id="5/a/2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Here a quantum operation is interpreted as a deterministic [quantum channel](../../../../../../../quantum-channel.md), so it is completely positive and [matrix trace](../../../../../../../matrix-trace.md) preserving. Write its [Kraus representation](../../../../../../../kraus-representation.md) with $\sum_kA_k^\dagger A_k=I$ and define the [isometry](../../../../../../../isometry.md) in its [Stinespring dilation](../../../../../../../stinespring-dilation.md)

$$
V|\psi\rangle=\sum_kA_k|\psi\rangle\otimes|k\rangle_E.
$$

Then $V^\dagger V=I$ and $\Phi(\rho)=\operatorname{Tr}_E(V\rho V^\dagger)$. Acting on $B$ gives $\sigma_{AB'E}=(I_A\otimes V)\rho_{AB}(I_A\otimes V^\dagger)$. An [isometry](../../../../../../../isometry.md) preserves the nonzero [eigenvalues](../../../../../../../eigenvalue.md) of a [density operator](../../../../../../../density-matrix.md). Hence $S(AB'E)=S(AB)$, $S(B'E)=S(B)$, and $S(A)$ is unchanged. It follows that $I(A:B'E)_\sigma=I(A:B)_\rho$.

Now discard $E$ and apply part 1. This proves [data processing for quantum mutual information](../../../../../../../data-processing-for-quantum-mutual-information.md):

$$
\boxed{I(A:B')\le I(A:B'E)=I(A:B).}
$$

The [matrix trace](../../../../../../../matrix-trace.md)-preserving convention matters. [Postselection can increase conditional quantum mutual information](../../../../../../../postselection-can-increase-conditional-quantum-mutual-information.md): take a uniform classical bit $A$, copy it to $B$ with probability $\varepsilon$, and otherwise put $B$ in an erasure state independent of $A$. Initially $I(A:B)=\varepsilon$ bits. Projecting onto the nonerased sector and conditioning on success gives a perfectly correlated bit pair with [quantum mutual information](../../../../../../../quantum-mutual-information.md) one. That success branch is [matrix trace](../../../../../../../matrix-trace.md) decreasing, and its renormalized action is not a deterministic channel. Retaining the full outcome flag and averaging all branches restores the ordinary channel inequality.

## ↑ Ancestors (12)

1. [2](../2.md)
2. [A](../../a.md)
3. [5](../../../5.md)
4. [Paper 33](../../../../paper-33-split.md)
5. [Iii](../../../../split.md)
6. [2006](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
