<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Write $\overline\rho=\sum_i p_i\rho_i$. The [Holevo quantity](../../../../../../holevo-quantity.md) is

$$
\boxed{\chi(\mathcal E)=S(\overline\rho)-\sum_i p_iS(\rho_i),}
$$

where $S$ is [Von Neumann entropy](../../../../../../von-neumann-entropy-split.md), with a consistent logarithm base. Attach an orthogonal classical label register $X$ to form the [classical-quantum state](../../../../../../classical-quantum-state.md)

$$
\omega_{XB}=\sum_i p_i|i\rangle\langle i|_X\otimes\rho_i.
$$

The [entropy of an orthogonal quantum mixture](../../../../../../entropy-of-an-orthogonal-quantum-mixture.md) gives

$$
S(X)=H(p),\quad S(XB)=H(p)+\sum_i p_iS(\rho_i),\quad S(B)=S(\overline\rho).
$$

Here $H(p)$ is the [Shannon entropy](../../../../../../information-entropy.md) of the classical label. Hence $I(X:B)=\chi(\mathcal E)$, where $I$ denotes [quantum mutual information](../../../../../../quantum-mutual-information.md).

Let $\Phi:B\to C$ be the proposed [quantum channel](../../../../../../quantum-channel.md). Using its [Kraus representation](../../../../../../kraus-representation.md), define an [linear isometry](../../../../../../linear-isometry-of-hilbert-spaces.md) $V=\sum_\ell A_\ell\otimes|\ell\rangle_E$, since $V^\dagger V=I$. This is a [Stinespring representation](../../../../../../stinespring-representation-of-a-completely-positive-map.md). Apply it to $B$, obtaining a state $\eta_{XCE}$; tracing out $E$ applies $\Phi$ to every ensemble member. An [linear isometry](../../../../../../linear-isometry-of-hilbert-spaces.md) preserves nonzero [eigenvalues](../../../../../../eigenvalue.md) and therefore [Von Neumann entropy](../../../../../../von-neumann-entropy-split.md), so

$$
I(X:CE)_\eta=I(X:B)_\omega=\chi(\mathcal E),
\qquad
I(X:C)_\eta=\chi(\{p_i,\Phi(\rho_i)\}).
$$

Their difference is

$$
I(X:CE)-I(X:C)=S(XC)+S(CE)-S(C)-S(XCE).
$$

The [Strong subadditivity of Von Neumann entropy](../../../../../../strong-subadditivity-of-quantum-entropy.md) states that this expression is nonnegative for every tripartite state. Consequently

$$
\boxed{\chi(\{p_i,\Phi(\rho_i)\})\leq\chi(\mathcal E).}
$$

Thus the [Holevo quantity under a quantum channel](../../../../../../holevo-quantity-under-a-quantum-channel.md) decreases because discarding the dilation environment cannot improve correlations with the classical label. The probabilities remain unchanged throughout.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3](../../3.md)
3. [Paper 50](../../../paper-50-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
