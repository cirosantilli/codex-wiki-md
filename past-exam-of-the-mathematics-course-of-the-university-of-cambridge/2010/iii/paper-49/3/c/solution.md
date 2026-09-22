<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The point needing proof is that a corrected error's residual state cannot retain dependence on the logical input. Let $W_j$ denote the complete linear map from the logical input to all five output wires for error $E_j$. Protection gives $W_j|0\rangle=|0\rangle|\eta_{j,0}\rangle$ and $W_j|1\rangle=|1\rangle|\eta_{j,1}\rangle$. Applying protection to $|+\rangle$ and comparing its two top-qubit components yields

$$
\frac{|0\rangle|\eta_{j,0}\rangle+|1\rangle|\eta_{j,1}\rangle}{\sqrt2}
=|+\rangle|\eta_{j,+}\rangle,
$$

so $|\eta_{j,0}\rangle=|\eta_{j,1}\rangle=|\eta_{j,+}\rangle$. Denote the common vector by $|\eta_j\rangle$. Linearity then gives $W_j|\psi\rangle=|\psi\rangle|\eta_j\rangle$ for every input.

The encoding and all operations surrounding the error are fixed. Replacing the error by $E=\alpha E_1+\beta E_2$ consequently replaces the overall map by $\alpha W_1+\beta W_2$, giving

$$
\boxed{W_E|\psi\rangle=|\psi\rangle\otimes\left(\alpha|\eta_1\rangle+\beta|\eta_2\rangle\right).}
$$

Because $E$ and the surrounding circuit are unitary, the output is normalized for every normalized input; the residual vector in parentheses thus has norm one. This proves [linearity of coherent quantum error correction](../../../../../../linearity-of-coherent-quantum-error-correction.md) and hence protection against $E$. Orthogonality of $|\eta_1\rangle$ and $|\eta_2\rangle$ is not required for this proof.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [3](../../3.md)
3. [Paper 49](../../../paper-49-split.md)
4. [Iii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
