<h1 id="4/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

Put $\kappa=\aleph_2^M$ and let $F=\bigcup G$. Conditions from [Fn forcing](../../../../../../fn-forcing.md) agree on common coordinates because $G$ is directed, so $F$ is a function. For each $(\xi,n)\in\kappa\times\omega$, the ground-model [set](../../../../../../set-split.md)

$$
D_{\xi,n}=\{p:(\xi,n)\in\operatorname{dom}p\}
$$

is dense: add a value at that coordinate if necessary. The [generic filter](../../../../../../generic-filter.md) meets all these [sets](../../../../../../set-split.md), making $F:\kappa\times\omega\to2$ total.

For distinct $\xi,\eta<\kappa$, the ground-model [set](../../../../../../set-split.md)

$$
D_{\xi,\eta}=\{p:\exists n\ ((\xi,n),(\eta,n)\in\operatorname{dom}p\text{ and }p(\xi,n)\ne p(\eta,n))\}
$$

is dense. Choose $n$ fresh for both rows of a finite condition and assign $0$ and $1$ there. Genericity therefore makes the rows pairwise different. The [generic coordinate reals for finite-function forcing](../../../../../../generic-coordinate-reals-for-finite-function-forcing.md) are $c_\xi=\{n\in\omega:F(\xi,n)=1\}$, and in the [generic extension](../../../../../../generic-extension.md)

$$
\boxed{\xi\longmapsto c_\xi\text{ is an injection }\aleph_2^M\hookrightarrow\mathcal P^{M[G]}(\omega).}
$$

The family is a [set](../../../../../../set-split.md) in $M[G]$, for example by collecting the ground-model names $\dot c_\xi=\{(\check n,p):p(\xi,n)=1\}$ and evaluating the corresponding name for their indexed family. This argument only needs $\kappa$ as the specified ground-model [ordinal](../../../../../../ordinal.md); it does not silently assume a [cardinal preservation by chain-condition forcing](../../../../../../cardinal-preservation-by-chain-condition-forcing.md) result.

## ↑ Ancestors (11)

1. [Iv](../iv.md)
2. [4](../../4.md)
3. [Paper 121](../../../paper-121-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
