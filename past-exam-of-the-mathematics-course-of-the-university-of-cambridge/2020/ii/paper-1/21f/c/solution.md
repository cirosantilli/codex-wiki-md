<h1 id="21f/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Choose $\widehat x_i\in p_i^{-1}(x_0)$. By the [classification of connected covering spaces](../../../../../../classification-of-connected-covering-spaces.md) and the [degree of a connected covering](../../../../../../degree-of-a-connected-covering.md), each cover corresponds to an index-two subgroup

$$
H_i=(p_i)_*\pi_1(\widehat X_i,\widehat x_i)
\le\pi_1(X,x_0)\cong\mathbb Z^2.
$$

An index-two subgroup is the kernel of a nonzero homomorphism $\mathbb Z^2\to\mathbb Z/2\mathbb Z$. There are three:

$$
\{(m,n):m\equiv0\pmod2\},\qquad
\{(m,n):n\equiv0\pmod2\},\qquad
\{(m,n):m+n\equiv0\pmod2\}.
$$

The group $GL_2(\mathbb F_2)$ acts transitively on the three nonzero linear functionals on $\mathbb F_2^2$, and its elementary matrices lift to the [integral general linear group](../../../../../../integral-general-linear-group.md). Hence there is $A\in GL_2(\mathbb Z)$ such that

$$
AH_1=H_2.
$$

Take $\psi=f_A$. Since $\psi_*(H_1)=H_2$, the [lifting criterion for a covering space](../../../../../../lifting-criterion-for-a-covering-space.md) gives a based lift

$$
\phi:\widehat X_1\to\widehat X_2
$$

such that

$$
\boxed{p_2\circ\phi=\psi\circ p_1}.
$$

Applying the same argument to $A^{-1}$ gives a lift in the reverse direction. The composites are based lifts of the appropriate identity maps; uniqueness of based lifts makes them identities. Thus $\phi$ and $\psi$ are homeomorphisms, and the required square commutes. This proves the [equivalence of connected double covers of the torus](../../../../../../equivalence-of-connected-double-covers-of-the-torus.md).

## ↑ Ancestors (11)

1. [C](../c.md)
2. [21F](../../21f.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2020](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
