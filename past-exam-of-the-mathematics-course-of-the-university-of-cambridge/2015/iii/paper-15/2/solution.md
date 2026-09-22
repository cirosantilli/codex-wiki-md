<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

**The tensor differential.** Use homological grading, so each differential lowers degree by one. The [tensor product of chain complexes](../../../../../tensor-product-of-chain-complexes.md) has

$$
(C\otimes_R C')_k=\bigoplus_{p+q=k}C_p\otimes_R C'_q,\qquad
D(x\otimes y)=d_Cx\otimes y+(-1)^p x\otimes d_{C'}y
$$

for $x\in C_p$. This [Koszul sign rule](../../../../../koszul-sign-rule.md) gives

$$
D^2(x\otimes y)=d_C^2x\otimes y+
\bigl((-1)^{p-1}+(-1)^p\bigr)d_Cx\otimes d_{C'}y+
x\otimes d_{C'}^2y=0.
$$

Thus the graded [tensor product](../../../../../tensor-product.md) is a [chain complex](../../../../../chain-complex.md).

**The Hom differential.** Write $M_j=\prod_p\operatorname{Hom}_R(C_p,C'_{p+j})$. For a degree-$j$ element of this [graded Hom complex of chain complexes](../../../../../graded-hom-complex-of-chain-complexes.md), use the prescribed differential

$$
d_M f=f d_C+(-1)^{j-1}d_{C'}f.
$$

The next application uses degree $j-1$, so

$$
d_M^2f=f d_C^2+
\bigl((-1)^{j-1}+(-1)^{j-2}\bigr)d_{C'}f d_C+
(-1)^{2j-3}d_{C'}^2f=0.
$$

In degree zero, $d_Mf=f d_C-d_{C'}f$, so its kernel consists exactly of [chain maps](../../../../../chain-map.md). A degree-one element $h$ has $d_Mh=h d_C+d_{C'}h$, which is exactly the change between two [chain maps](../../../../../chain-map.md) related by a [chain homotopy](../../../../../chain-homotopy.md). Consequently

$$
\boxed{H_0(M(C,C'))\cong
\{\text{chain maps }C\to C'\}/\text{chain homotopy}.}
$$

This is natural: precomposition and postcomposition by [chain maps](../../../../../chain-map.md) preserve both degree-zero cycles and degree-zero boundaries.

**The dual complex and the sign adjustment.** Define the [reversed dual chain complex](../../../../../reversed-dual-chain-complex.md)

$$
X_i=\operatorname{Hom}_R(C_{-i},R),\qquad
d_X\phi=\phi d_C.
$$

Here $d_X\phi$ is a functional on $C_{1-i}$, so it belongs to $X_{i-1}$, and $d_X^2=0$. The absence of an additional sign in $d_X$ is intentional.

Interpret finite generation of the free [chain complexes](../../../../../chain-complex.md) as finiteness of their total graded [free modules](../../../../../free-module.md). Then only finitely many degrees occur, and the finite-free evaluation isomorphisms assemble into a graded isomorphism

$$
\psi:X\otimes_R C'\longrightarrow M(C,C'),\qquad
\psi(\phi\otimes y)(c)=\phi(c)y,
$$

where $\phi\in X_i$, $y\in C'_j$, and this component is zero outside $C_{-i}$. The [dual module](../../../../../dual-module.md) construction and evaluation make $\psi$ natural. Finite rank is needed for evaluation to be an isomorphism; finite total support also makes the sums on the tensor side agree with the products on the [Hom functor](../../../../../hom-functor.md) side.

Under $\psi$, the [Hom functor](../../../../../hom-functor.md) differential has the form

$$
\psi^{-1}d_M\psi(\phi\otimes y)=d_X\phi\otimes y+
(-1)^{i+j-1}\phi\otimes d_{C'}y.
$$

The usual [tensor product of chain complexes](../../../../../tensor-product-of-chain-complexes.md) instead has second coefficient $(-1)^i$. Set

$$
\boxed{\rho(j)=\frac{j(j-1)}2,\qquad
A|_{X_i\otimes C'_j}=(-1)^{\rho(j)}\,\mathrm{id}.}
$$

This is integer-valued for every $j\in\mathbb Z$, including negative $j$, and satisfies $\rho(j)-\rho(j-1)=j-1$. Conjugating the usual tensor differential by $A$ leaves the first term unchanged and changes its second coefficient to $(-1)^{i+j-1}$. Hence $d_M=\psi A D A^{-1}\psi^{-1}$, giving the [sign conjugation for the tensor-Hom identification](../../../../../sign-conjugation-for-the-tensor-hom-identification.md)

$$
\boxed{\Phi=\psi A:X\otimes_R C'\xrightarrow{\;\cong\;}M(C,C'),
\qquad
\Phi(\phi\otimes y_j)(c)=(-1)^{j(j-1)/2}\phi(c)y_j.}
$$

This is an isomorphism of [chain complexes](../../../../../chain-complex.md), not merely of their [homology](../../../../../homology-split.md). If one instead assumes only degreewise finite rank with unbounded grading, the ordinary tensor need not identify with the product defining $M$; the finite-total convention is essential to this last conclusion.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 15](../../paper-15-split.md)
3. [Iii](../../split.md)
4. [2015](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
