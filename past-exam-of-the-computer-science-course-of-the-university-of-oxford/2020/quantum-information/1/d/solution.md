<h1 id="1/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

The map sends $|0\rangle$ to $|0\rangle$, $|1\rangle$ to $|2\rangle$, and $|2\rangle$ to $\lambda|1\rangle$. These output columns are mutually [orthogonal](../../../../../orthogonal-vectors.md), with squared [norms](../../../../../norm.md) $1,1,|\lambda|^2$. Consequently

$$
M_\lambda^\dagger M_\lambda=\operatorname{diag}(1,1,|\lambda|^2),
$$

and

$$
\boxed{M_\lambda\text{ is unitary if and only if }|\lambda|=1,\text{ equivalently }\lambda=e^{i\theta}\text{ for real }\theta.}
$$

Necessity follows from preserving the [norm](../../../../../norm.md) of $|2\rangle$; sufficiency follows because the three columns are then an [orthonormal basis](../../../../../orthonormal-basis.md). Merely requiring $\lambda\ne0$ would establish invertibility but not [unitarity](../../../../../unitary-operator.md). This is the [weighted permutation unitarity criterion](../../../../../weighted-permutation-unitarity-criterion.md).

## ↑ Ancestors (11)

1. [D](../d.md)
2. [1](../../1.md)
3. [Quantum information](../../../quantum-information-split.md)
4. [2020](../../../split.md)
5. [Past exam of the computer science course of the University of Oxford](../../../../split.md)
6. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../../../university-of-oxford-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
