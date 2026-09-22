<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Over a [finite field](../../../../../finite-field.md) $\mathbb F_q$, a [linear code](../../../../../linear-code.md) of length $N$ and dimension $k$ is a $k$-dimensional subspace $C\subseteq\mathbb F_q^N$. A full-row-rank [generator matrix](../../../../../generator-matrix.md) $G\in\mathbb F_q^{k\times N}$ gives $C=\{mG:m\in\mathbb F_q^k\}$, using row-vector messages. A full-row-rank [parity-check matrix](../../../../../parity-check-matrix.md) $H\in\mathbb F_q^{(N-k)\times N}$ gives $C=\{x:Hx^T=0\}$. The [dual code](../../../../../dual-code.md) is $C^\perp=\{y:x\cdot y=0\text{ for all }x\in C\}$, of dimension $N-k$. Thus the rows of $H$ span $C^\perp$, and

$$
\boxed{HG^T=0,\qquad G_{C^\perp}=H,\quad H_{C^\perp}=G.}
$$

Conversely the rank conditions and $HG^T=0$ imply that the row space of $G$ equals the kernel of $H$, by inclusion and equality of dimensions.

For a [CSS code](../../../../../css-code.md), specialize to binary [linear codes](../../../../../linear-code.md) $C_2\subseteq C_1\subseteq\mathbb F_2^N$, of dimensions $k_2,k_1$. Define orthonormal encoded states

$$
|x+C_2\rangle=\frac1{\sqrt{|C_2|}}\sum_{y\in C_2}|x+y\rangle,\qquad x\in C_1/C_2.
$$

Different cosets have disjoint computational-basis support. Their span has dimension $2^{k_1-k_2}$, so it encodes $K=k_1-k_2$ logical [qubits](../../../../../qubit.md). For binary vectors write $X(u)=\bigotimes_jX_j^{u_j}$ and $Z(v)=\bigotimes_jZ_j^{v_j}$. The [stabilizer generators](../../../../../stabilizer-generator.md) are $X(u)$ for a basis of $C_2$, and $Z(v)$ for a basis of $C_1^\perp$. They fix each encoded state: the former permute its coset terms and the latter contribute phases $(-1)^{v\cdot(x+y)}=1$. Their commutation relation is $X(u)Z(v)=(-1)^{u\cdot v}Z(v)X(u)$, so the classical dual inclusion $C_1^\perp\subseteq C_2^\perp$ makes them commute. There are $k_2+N-k_1=N-K$ independent checks, giving precisely this encoded space.

For a [Pauli error](../../../../../pauli-operator.md) $X(e)Z(f)$, the Z checks give bit-error [syndrome](../../../../../syndrome.md) $H_1e^T$, where $H_1$ checks $C_1$, and the X checks give phase-error [syndrome](../../../../../syndrome.md) $G_2f^T$, where $G_2$ generates $C_2$ and hence checks $C_2^\perp$. Classical decoders therefore correct up to $t_X$ bit flips and $t_Z$ phase flips if $d(C_1)>2t_X$ and $d(C_2^\perp)>2t_Z$. A Y error has both components; it is not omitted from this correction scheme.

For the precise [quantum code distance](../../../../../distance-of-a-quantum-error-correcting-code.md), harmless stabilizer errors must be excluded. A pure-X error preserves the code exactly when $e\in C_1$, and is a stabilizer when $e\in C_2$; a pure-Z error preserves it when $f\in C_2^\perp$, and is a stabilizer when $f\in C_1^\perp$. Consequently, for $K>0$,

$$
d_X=\min_{e\in C_1\setminus C_2}\operatorname{wt}(e),\quad
d_Z=\min_{f\in C_2^\perp\setminus C_1^\perp}\operatorname{wt}(f),\qquad
\boxed{d=\min(d_X,d_Z).}
$$

A mixed Pauli error has weight equal to the size of the union of its X and Z supports. If it is a nontrivial logical operator, at least one component is nontrivial, so its weight is at least $\min(d_X,d_Z)$; pure-X or pure-Z operators attain that minimum. Thus $t=\lfloor(d-1)/2\rfloor$ arbitrary-qubit errors are correctable: products of two such [Pauli errors](../../../../../pauli-operator.md) have weight below $d$ and act scalarly on the code, or take it to an orthogonal syndrome sector. This is the [Knill--Laflamme condition](../../../../../knill-laflamme-condition.md). Expanding arbitrary errors in the Pauli basis extends correction to their coherent linear span.

An explicit example is the [Steane code](../../../../../steane-code.md). Take $C_1$ to be the binary [Hamming code](../../../../../hamming-code.md) with

$$
H=\begin{pmatrix}1&0&1&0&1&0&1\\0&1&1&0&0&1&1\\0&0&0&1&1&1&1\end{pmatrix},\qquad C_2=C_1^\perp=\operatorname{row}(H).
$$

The distinct nonzero columns show that $C_1$ has no weight-one or weight-two word, while three dependent columns give a weight-three word. Hence its classical distance is three. Direct multiplication gives $HH^T=0$, proving $C_2\subseteq C_1$. Every nonzero word of $C_2$ has weight four, so the logical X and Z distances are both three. Its six stabilizer checks are the X and Z strings given by the three rows of $H$. A logical basis is the uniform superposition over $C_2$ and over $\mathbf1+C_2$, since $\mathbf1=(1,\ldots,1)\in C_1\setminus C_2$. **The resulting $[[7,1,3]]$ CSS code corrects every single-qubit error.**

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 32](../../paper-32-split.md)
3. [Iii](../../split.md)
4. [2004](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
