<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

A [linear map](../../../../../linear-map.md) $\Phi$ is a [completely positive map](../../../../../completely-positive-map.md) if $\operatorname{id}_R\otimes\Phi$ sends every [positive operator](../../../../../positive-operator.md) to a [positive operator](../../../../../positive-operator.md) for every finite-dimensional auxiliary system $R$. Positivity of $\Phi$ alone tests only inputs without an auxiliary system and is weaker.

For the [Kraus representation](../../../../../kraus-representation.md), let $\Omega\ge0$ be any operator on the auxiliary system and the input system. Then

$$
(\operatorname{id}_R\otimes\Phi)(\Omega)=\sum_k(I_R\otimes A_k)\Omega(I_R\otimes A_k^\dagger).
$$

For any vector $v$, its expectation is $\sum_k\langle(I_R\otimes A_k^\dagger)v,\Omega(I_R\otimes A_k^\dagger)v\rangle\ge0$. Every amplification is therefore positive, proving **the Kraus-form map is completely positive**. No normalization condition on the $A_k$ is needed for this positivity proof. To make it a deterministic [quantum channel](../../../../../quantum-channel.md), one additionally requires $\sum_kA_k^\dagger A_k=I$; a physical outcome branch instead obeys $\sum_kA_k^\dagger A_k\le I$.

Transposition is positive on one system: for any positive $\rho$ and any $v$, $v^\dagger\rho^Tv$ is the complex conjugate of $\bar v^\dagger\rho\bar v$, hence is real and nonnegative. It fails complete positivity already for a [qubit](../../../../../qubit.md). Apply partial transposition to the second subsystem of the [Bell state](../../../../../bell-state-split.md) $|\Phi^+\rangle=(|00\rangle+|11\rangle)/\sqrt2$. The resulting operator is

$$
(\operatorname{id}\otimes T)(|\Phi^+\rangle\langle\Phi^+|)=\frac12\bigl(|00\rangle\langle00|+|01\rangle\langle10|+|10\rangle\langle01|+|11\rangle\langle11|\bigr).
$$

On the antisymmetric vector $(|01\rangle-|10\rangle)/\sqrt2$, its eigenvalue is $-1/2$. Thus the [partial transpose](../../../../../partial-transpose.md) is not positive on this entangled input, and

$$
\boxed{T\text{ is positive but not completely positive in dimension at least two}.}
$$

The same witness embeds into any larger input dimension; in the exceptional one-dimensional case transposition is simply the identity.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 33](../../paper-33-split.md)
3. [Iii](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
