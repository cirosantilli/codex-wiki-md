<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

The [root lattice](../../../../../root-lattice.md) is $Q=\sum_i\mathbb Z\alpha^{(i)}$. The [weight lattice](../../../../../weight-lattice.md) is

$$
P=\{\lambda:\langle\lambda,(\alpha^{(i)})^\vee\rangle\in\mathbb Z\text{ for every }i\}.
$$

Because every [Cartan integer](../../../../../cartan-integer.md) $\langle\alpha^{(j)},(\alpha^{(i)})^\vee\rangle$ is integral, $Q\subseteq P$. The [Dynkin labels](../../../../../dynkin-label.md) of $\lambda$ are

$$
[m_1,\ldots,m_r],
\qquad m_i=\langle\lambda,(\alpha^{(i)})^\vee\rangle.
$$

There are three isomorphism classes of complex simple rank-three Lie algebras: types [A3 root system](../../../../../a3-root-system.md)$A_3$, [B3 root system](../../../../../b3-root-system.md)$B_3$, and [C3 root system](../../../../../c3-root-system.md)$C_3$. Use the convention $A_{ij}=\langle\alpha^{(i)},(\alpha^{(j)})^\vee\rangle$, and order the chain as $1$--$2$--$3$ with $|\alpha^{(1)}|=|\alpha^{(2)}|$.


- For $A_3$, all roots have the same length and the diagram has two single edges. Its [Cartan matrix](../../../../../cartan-matrix.md) and angles are


$$
A_{A_3}=\begin{pmatrix}2&-1&0\\-1&2&-1\\0&-1&2\end{pmatrix},
\qquad
\theta_{12}=\theta_{23}=120^\circ,quad\theta_{13}=90^\circ,quad
\frac{|\alpha^{(2)}|}{|\alpha^{(3)}|}=1.
$$


- For $B_3$, take $\alpha^{(1)}=e_1-e_2$, $\alpha^{(2)}=e_2-e_3$, and $\alpha^{(3)}=e_3$. The double-edge arrow points to the short third root, and


$$
A_{B_3}=\begin{pmatrix}2&-1&0\\-1&2&-2\\0&-1&2\end{pmatrix},
\qquad
\theta_{12}=120^\circ,quad\theta_{23}=135^\circ,quad\theta_{13}=90^\circ,quad
\frac{|\alpha^{(2)}|}{|\alpha^{(3)}|}=\sqrt2.
$$


- For $C_3$, take $\alpha^{(1)}=e_1-e_2$, $\alpha^{(2)}=e_2-e_3$, and $\alpha^{(3)}=2e_3$. The double-edge arrow points to the short second root, and


$$
A_{C_3}=\begin{pmatrix}2&-1&0\\-1&2&-1\\0&-2&2\end{pmatrix},
\qquad
\theta_{12}=120^\circ,quad\theta_{23}=135^\circ,quad\theta_{13}=90^\circ,quad
\frac{|\alpha^{(2)}|}{|\alpha^{(3)}|}=\frac1{\sqrt2}.
$$

The Dynkin labels of a finite-dimensional [irreducible representation](../../../../../irreducible-representation.md) are those of its [highest weight](../../../../../highest-weight-of-a-representation.md). Thus $[1,0,0]$ means the [fundamental representation](../../../../../fundamental-representation.md) $V(\omega_1)$. The weights, written in Dynkin labels and in a lowering order, are

$$
\begin{array}{c|l|c}
\text{type}&\text{weight labels}&\dim V(\omega_1)\\ \hline
A_3&[1,0,0],[-1,1,0],[0,-1,1],[0,0,-1]&4\\
B_3&[1,0,0],[-1,1,0],[0,-1,2],[0,0,0],[0,1,-2],[1,-1,0],[-1,0,0]&7\\
C_3&[1,0,0],[-1,1,0],[0,-1,1],[0,1,-1],[1,-1,0],[-1,0,0]&6
\end{array}.
$$

For $A_3$ these are the weights of the defining representation of $\mathfrak{sl}_4$; for $B_3$ they are $\{\pm e_1,\pm e_2,\pm e_3,0\}$ in the vector representation of $\mathfrak{so}_7$; for $C_3$ they are $\{\pm e_1,\pm e_2,\pm e_3\}$ in the defining representation of $\mathfrak{sp}_6$. Hence the requested dimensions are **$4$, $7$, and $6$**, respectively.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 302](../../paper-302-split.md)
3. [Iii](../../split.md)
4. [2019](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
