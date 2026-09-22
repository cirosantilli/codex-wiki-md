<h1 id="4/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

For a line bundle $L$ on $X$, define the [homomorphism associated to a line bundle on an abelian variety](../../../../../../homomorphism-associated-to-a-line-bundle-on-an-abelian-variety.md)

$$
\phi_L:X(k)\longrightarrow\operatorname{Pic}(X),
\qquad
\phi_L(x)=T_x^*L\otimes L^\vee.
$$

The [Theorem of the square](../../../../../../theorem-of-the-square.md) gives

$$
\phi_L(x+y)=T_{x+y}^*L\otimes L^\vee\simeq\phi_L(x)\otimes\phi_L(y),
$$

so $\phi_L$ is a homomorphism. Pullback distributes over the [tensor product of sheaves](../../../../../../tensor-product-of-sheaves.md), and therefore

$$
\boxed{\phi_{L\otimes M}(x)=\phi_L(x)\otimes\phi_M(x).}
$$

Iterating the homomorphism law in $x$ gives

$$
\boxed{\phi_{L^{\otimes n}}(x)=\phi_L(x)^{\otimes n}=\phi_L(nx).}
$$

Suppose $L^{\otimes n}\in\operatorname{Pic}^0(X)$. Then $\phi_L(nx)$ is trivial for every $x$. The [multiplication-by-n morphism](../../../../../../multiplication-by-n-morphism.md) on an abelian variety is surjective, so $\phi_L$ is trivial and $L\in\operatorname{Pic}^0(X)$. Thus the [Néron-Severi group](../../../../../../neron-severi-group.md)

$$
\operatorname{Pic}(X)/\operatorname{Pic}^0(X)
$$

is torsion-free.

Finally, put $M=\phi_L(x)$. For every $y$,

$$
\phi_M(y)=T_y^*(T_x^*L\otimes L^\vee)\otimes(T_x^*L\otimes L^\vee)^\vee
\simeq T_{x+y}^*L\otimes T_y^*L^\vee\otimes T_x^*L^\vee\otimes L,
$$

which is trivial by the Theorem of the square. Hence

$$
\boxed{\operatorname{im}\phi_L\subseteq\operatorname{Pic}^0(X).}
$$

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [4](../../4.md)
3. [Paper 126](../../../paper-126-split.md)
4. [Iii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
