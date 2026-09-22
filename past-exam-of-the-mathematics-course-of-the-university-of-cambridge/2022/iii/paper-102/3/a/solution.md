<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

A finite-dimensional [Lie algebra](../../../../../../lie-algebra-split.md) $L$ is [semisimple](../../../../../../semisimple-lie-algebra-split.md) when its [solvable radical](../../../../../../radical-of-a-lie-algebra.md) is zero, equivalently when it has no nonzero solvable [ideals](../../../../../../ideal-of-a-lie-algebra.md).

We prove the [Weyl complete reducibility theorem](../../../../../../weyl-complete-reducibility-theorem.md). Induct on the dimension of a finite-dimensional $L$-module $V$. It is enough first to split a submodule $W$ of codimension one. The one-dimensional quotient is trivial because a semisimple Lie algebra is [perfect](../../../../../../perfect-lie-algebra.md). By induction, $W$ is a direct sum of irreducible modules. A [Casimir element](../../../../../../casimir-element.md) formed using the [Killing form](../../../../../../killing-form.md) commutes with the $L$-action, acts as zero on every trivial summand, and acts by a nonzero scalar on every nontrivial irreducible summand. Its image is therefore the sum $W_1$ of the nontrivial summands, while its kernel contains the trivial summands $W_0$ and maps onto $V/W$. Thus

$$
V=W_1\oplus\ker\Omega.
$$

Inside $\ker\Omega$, choose a lift $v$ of a basis of $V/W$. For $x\in L$, $xv\in W_0$, and $L$ acts trivially on $W_0$. Hence $[x,y]v=0$ for all $x,y\in L$. Since $L=[L,L]$, actually $xv=0$ for every $x$, so $\mathbb Cv$ is the required invariant complement.

This codimension-one case implies the general case. For an arbitrary submodule $W\subseteq V$, let

$$
X=\{f\in\operatorname{Hom}_{\mathbb C}(V,W):f|_W\text{ is scalar}\}
$$

with the natural [Hom representation](../../../../../../hom-representation.md). The maps vanishing on $W$ form an $L$-submodule $X_0$ of codimension one. Splitting $X_0$ supplies an $L$-equivariant $f$ with $f|_W=I_W$. Then

$$
V=W\oplus\ker f,
$$

so every invariant subspace has an invariant complement and every finite-dimensional representation is completely reducible.

For the requested example, embed $\mathfrak{sl}_2$ as the upper-left $2\times2$ block in the [special linear Lie algebra](../../../../../../special-linear-lie-algebra.md) $\mathfrak{sl}_3$. Under the restricted [Adjoint representation](../../../../../../adjoint-representation-of-a-lie-algebra.md),

$$
\mathfrak{sl}_3
=\underbrace{\mathfrak{sl}_2}_{V_2}
\oplus\underbrace{\mathbb C\operatorname{diag}(1,1,-2)}_{V_0}
\oplus\underbrace{\langle E_{13},E_{23}\rangle}_{V_1}
\oplus\underbrace{\langle E_{31},E_{32}\rangle}_{V_1}.
$$

Here $V_n$ is the irreducible $\mathfrak{sl}_2$-module of highest weight $n$. The first summand is the three-dimensional adjoint module, the second is trivial, and the last two are the two-dimensional defining module and its dual, which are isomorphic. This explicit direct sum demonstrates complete reducibility.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3](../../3.md)
3. [Paper 102](../../../paper-102-split.md)
4. [Iii](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
