<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

A [Cartan subalgebra](../../../../../cartan-subalgebra.md) $\mathfrak h$ of a finite-dimensional complex [semisimple Lie algebra](../../../../../semisimple-lie-algebra-split.md) is a maximal abelian subalgebra consisting of semisimple elements. The [root-space decomposition](../../../../../root-space-decomposition.md) is

$$
\mathfrak g=\mathfrak h\oplus\bigoplus_{\alpha\in\Phi}\mathfrak g_\alpha,
\qquad
\mathfrak g_\alpha=\{X:[H,X]=\alpha(H)X\text{ for all }H\in\mathfrak h\},
$$

and the nonzero functionals $\alpha$ are the roots. A [Cartan-Weyl basis](../../../../../cartan-weyl-basis.md) consists of a basis $H_i$ of $\mathfrak h$ and root vectors $E_\alpha\in\mathfrak g_\alpha$. Its brackets have the form

$$
[H_i,H_j]=0,qquad [H_i,E_\alpha]=\alpha(H_i)E_\alpha,qquad
[E_\alpha,E_{-\alpha}]=H_\alpha,
$$

and $[E_\alpha,E_\beta]=N_{\alpha\beta}E_{\alpha+\beta}$ when $\alpha+\beta$ is a root, and zero when $\alpha+\beta$ is neither a root nor zero.

For the complexified [so4 Lie algebra](../../../../../so4-lie-algebra.md), take $H^1=T^{(12)}$ and $H^2=T^{(34)}$. Write

$$
A_1^\pm=T^{(13)}\pm T^{(24)},
\qquad
A_2^\pm=T^{(14)}\pm T^{(23)}.
$$

Direct use of the stated commutation relations gives

$$
\begin{array}{c|rrrr}
&A_1^+&A_1^-&A_2^+&A_2^-\\ \hline
\operatorname{ad}H^1&A_2^-&-A_2^+&A_1^-&-A_1^+\\
\operatorname{ad}H^2&-A_2^-&-A_2^+&A_1^-&A_1^+
\end{array}.
$$

The simultaneous [eigenvectors](../../../../../eigenvector.md), hence the step generators, may be chosen as

$$
\begin{aligned}
E_{++}&=A_2^+-iA_1^-,& \alpha_{++}&=(i,i),\\
E_{+-}&=A_2^-+iA_1^+,& \alpha_{+-}&=(i,-i),\\
E_{-+}&=A_2^--iA_1^+,& \alpha_{-+}&=(-i,i),\\
E_{--}&=A_2^++iA_1^-,& \alpha_{--}&=(-i,-i).
\end{aligned}
$$

Thus the roots relative to $(H^1,H^2)$ are $(\pm i,\pm i)$. Replacing $H^a$ by $-iH^a$ gives the usual real coordinates $(\pm1,\pm1)$. The only nonzero brackets between step generators, apart from those obtained by antisymmetry, are

$$
\boxed{[E_{++},E_{--}]=4i(H^1+H^2),
\qquad [E_{+-},E_{-+}]=4i(H^1-H^2).}
$$

An [isomorphism](../../../../../isomorphism.md) of Lie algebras is a bijective [linear map](../../../../../linear-map.md) preserving the Lie bracket. Define

$$
\begin{aligned}
J_1^\pm&=-\tfrac12(T^{(23)}\pm T^{(14)}),\\
J_2^\pm&=-\tfrac12(T^{(31)}\pm T^{(24)}),\\
J_3^\pm&=-\tfrac12(T^{(12)}\pm T^{(34)}).
\end{aligned}
$$

Then

$$
[J_i^\pm,J_j^\pm]=\epsilon_{ijk}J_k^\pm,
\qquad [J_i^+,J_j^-]=0.
$$

The two spans are commuting copies of the complexified $\mathfrak{su}_2$, and together contain all six basis elements of $\mathfrak{so}_4$. [Chiral decomposition of the complexified so4 Lie algebra](../../../../../chiral-decomposition-of-the-complexified-so4-lie-algebra.md) therefore gives

$$
\boxed{\mathfrak{so}_4(\mathbb C)\cong
\mathfrak{su}_2(\mathbb C)\oplus\mathfrak{su}_2(\mathbb C).}
$$

Under this isomorphism the [Adjoint representation](../../../../../adjoint-representation-of-a-lie-algebra.md) is the direct sum of the adjoint representations of the two factors:

$$
\boxed{\mathbf6=(\mathbf3,\mathbf1)\oplus(\mathbf1,\mathbf3).}
$$

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 302](../../paper-302-split.md)
3. [Iii](../../split.md)
4. [2019](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
