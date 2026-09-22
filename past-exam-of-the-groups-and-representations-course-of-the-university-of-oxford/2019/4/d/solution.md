<h1 id="4/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Use the [basis](../../../../basis.md) [matrices](../../../../matrix.md) $M_{ab}=E_{ab}-E_{ba}$ from [solution](../a/solution.md). Define the [Pauli matrices](../../../../pauli-matrices.md) and the two-by-two identity by

$$
\sigma_1=\begin{pmatrix}0&1\\1&0\end{pmatrix},\qquad
\sigma_2=\begin{pmatrix}0&-i\\i&0\end{pmatrix},\qquad
\sigma_3=\begin{pmatrix}1&0\\0&-1\end{pmatrix},\qquad I=I_2.
$$

The following five [Hermitian](../../../../hermitian-operator.md) four-by-four [matrices](../../../../matrix.md), written as [Kronecker products](../../../../kronecker-product.md), realize a Euclidean [Clifford algebra](../../../../clifford-algebra.md):

$$
\gamma_1=\sigma_1\otimes I,\quad
\gamma_2=\sigma_2\otimes I,\quad
\gamma_3=\sigma_3\otimes\sigma_1,\quad
\gamma_4=\sigma_3\otimes\sigma_2,\quad
\gamma_5=\sigma_3\otimes\sigma_3,
\qquad \gamma_a\gamma_b+\gamma_b\gamma_a=2\delta_{ab}I_4.
$$

Define the [Lie algebra representation](../../../../lie-algebra-representation.md) on $\mathbb C^4$ by

$$
\boxed{\rho(M_{ab})=\frac14[\gamma_a,\gamma_b]=\frac12\gamma_a\gamma_b\qquad(a<b).}
$$

These are [anti-Hermitian matrices](../../../../skew-hermitian-matrix.md), appropriate to the real compact [Lie algebra](../../../../lie-algebra-split.md). For complete explicitness, all ten [representation](../../../../group-representation.md) [matrices](../../../../matrix.md) are

$$
\boxed{\begin{array}{c|c||c|c}
M_{12}&\tfrac i2\sigma_3\otimes I&M_{13}&-\tfrac i2\sigma_2\otimes\sigma_1\\
M_{14}&-\tfrac i2\sigma_2\otimes\sigma_2&M_{15}&-\tfrac i2\sigma_2\otimes\sigma_3\\
M_{23}&\tfrac i2\sigma_1\otimes\sigma_1&M_{24}&\tfrac i2\sigma_1\otimes\sigma_2\\
M_{25}&\tfrac i2\sigma_1\otimes\sigma_3&M_{34}&\tfrac i2 I\otimes\sigma_3\\
M_{35}&-\tfrac i2 I\otimes\sigma_2&M_{45}&\tfrac i2 I\otimes\sigma_1
\end{array}}
$$

Each table entry is the image under $\rho$ of the [basis](../../../../basis.md) [matrix](../../../../matrix.md) immediately to its left. Since the two-by-two factors are specified above, these [Kronecker products](../../../../kronecker-product.md) specify every entry of each four-by-four [matrix](../../../../matrix.md).

To verify the [representation](../../../../group-representation.md) law, the [Clifford algebra](../../../../clifford-algebra.md) relations imply

$$
[\rho(M_{ab}),\gamma_c]=\delta_{bc}\gamma_a-\delta_{ac}\gamma_b.
$$

Apply this identity to $\rho(M_{cd})=\tfrac14[\gamma_c,\gamma_d]$ and use the [commutator product rule](../../../../commutator-product-rule.md). The result is

$$
[\rho(M_{ab}),\rho(M_{cd})]
=\delta_{bc}\rho(M_{ad})-\delta_{ac}\rho(M_{bd})
-\delta_{bd}\rho(M_{ac})+\delta_{ad}\rho(M_{bc}),
$$

exactly the [Lie bracket](../../../../lie-bracket.md) relation in [solution](../a/solution.md). Thus $\rho$ is a [Lie algebra representation](../../../../lie-algebra-representation.md).

It remains to identify its [highest weight](../../../../highest-weight-of-a-representation.md), rather than just its [dimension](../../../../dimension-vector-space.md). The commuting [Hermitian](../../../../hermitian-operator.md) [Cartan subalgebra](../../../../cartan-subalgebra.md) operators are

$$
-i\rho(M_{12})=\tfrac12\sigma_3\otimes I,\qquad
-i\rho(M_{34})=\tfrac12I\otimes\sigma_3.
$$

Their simultaneous [eigenvalues](../../../../eigenvalue.md) are $(x,y)=(\pm\tfrac12,\pm\tfrac12)$. Converting with $(a,b)=(x-y,2y)$ gives exactly the four [weights](../../../../weight-representation-theory.md) of $V(0,1)$ in [solution](../b/solution.md). A state with $(x,y)=(\tfrac12,\tfrac12)$ has [highest weight](../../../../highest-weight-of-a-representation.md) $(0,1)$, so this [Clifford realization of the so5 spin representation](../../../../clifford-realization-of-the-so5-spin-representation.md) is the requested $r$.

Finally, $\rho(M_{12})^2=-I_4/4$, so

$$
\boxed{e^{2\pi\rho(M_{12})}=-I_4,\qquad e^{2\pi M_{12}}=I_5.}
$$

This explicitly exhibits the distinction between the [spinor representation](../../../../spin-representation.md) of $\mathfrak{so}(5)$, or of $\operatorname{Spin}(5)$, and a single-valued [group representation](../../../../group-representation.md) of $SO(5)$.

## ↑ Ancestors (12)

1. [D](../d.md)
2. [4](../../4.md)
3. [2019](../../../2019-split.md)
4. [Past exam of the groups and representations course of the University of Oxford](../../../split.md)
5. [Groups and representations course of the University of Oxford](../../../../groups-and-representations-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematical and theoretical physics course of the University of Oxford](../../../../year-4-of-the-mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
7. [Mathematical and theoretical physics course of the University of Oxford](../../../../mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)

## ← Incoming links (1)

- [Solution](../b/solution.md)
