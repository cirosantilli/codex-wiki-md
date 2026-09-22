<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Let $\mathcal P$ be the [pinching map](../../../../../../pinching-map.md) determined by the projectors, and put $\sigma=\mathcal P(\rho)$. This is a [nonselective projective measurement](../../../../../../nonselective-projective-measurement.md); its projectors are its [Kraus operators](../../../../../../kraus-operator.md). We will prove the exact [relative entropy of a pinched state](../../../../../../relative-entropy-of-a-pinched-state.md) identity.

First the support of $\rho$ is contained in that of $\sigma$. Indeed, if $v$ lies in the kernel of $\sigma$, positivity gives

$$
0=\langle v|\sigma|v\rangle=\sum_i\langle P_iv|\rho|P_iv\rangle
=\sum_i\|\rho^{1/2}P_iv\|^2.
$$

Every summand is zero. Since $\sum_iP_i=I$, also $\rho^{1/2}v=0$, and thus $v$ is in the kernel of $\rho$. Therefore the logarithm of $\sigma$ may be used on its support without an infinite relative-entropy term.

The operator $\sigma$ is block diagonal, so each $P_i$ commutes with $\log\sigma$ on that support. Cyclicity of the [trace](../../../../../../matrix-trace.md) gives

$$
\operatorname{Tr}(\sigma\log\sigma)
=\sum_i\operatorname{Tr}(P_i\rho P_i\log\sigma)
=\operatorname{Tr}\left(\rho\sum_iP_i\log\sigma P_i\right)
=\operatorname{Tr}(\rho\log\sigma).
$$

Expand the [quantum relative entropy](../../../../../../quantum-relative-entropy.md):

$$
D(\rho\|\sigma)=\operatorname{Tr}(\rho\log\rho)-\operatorname{Tr}(\rho\log\sigma)
=S(\sigma)-S(\rho).
$$

Its nonnegativity now proves the [entropy increase under nonselective projective measurement](../../../../../../entropy-increase-under-nonselective-projective-measurement.md):

$$
\boxed{S(\sigma)\geq S(\rho).}
$$

The equality case in [nonnegativity of quantum relative entropy](../../../../../../nonnegativity-of-quantum-relative-entropy.md) says equality holds exactly when $\rho=\sigma$. Equivalently,

$$
\boxed{P_i\rho P_j=0\text{ for }i\ne j,\quad\text{or, equivalently, }[\rho,P_i]=0\text{ for every }i.}
$$

Thus equality means the state already has no coherence between distinct measurement blocks. It need not be diagonal inside a block of rank greater than one.

## ↑ Ancestors (11)

1. [C](../c.md)
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
