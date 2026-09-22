<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

The [long exact sequence in homology](../../../../../long-exact-sequence-in-homology.md) of the triple $A\subseteq U\subseteq X$ contains

$$
\cdots\to H_q(U,A)\to H_q(X,A)\to H_q(X,U)\to H_{q-1}(U,A)\to\cdots.
$$

Because $A\hookrightarrow U$ is a [homotopy equivalence](../../../../../homotopy-equivalence.md), $H_*(U,A)=0$. Hence the middle map is an isomorphism in every degree:

$$
H_*(X,A)\cong H_*(X,U).
$$

The [Excision theorem](../../../../../excision-theorem.md) says that if $Z\subseteq A\subseteq X$ and $\overline Z\subseteq\operatorname{int}A$, then inclusion induces

$$
H_*(X\setminus Z,A\setminus Z)\xrightarrow{\sim}H_*(X,A).
$$

A [good pair](../../../../../good-pair.md) $(X,A)$ has $A$ closed and a neighborhood $U$ that deformation retracts onto $A$. The [collapsing a pair theorem](../../../../../collapsing-a-pair-theorem.md) states that the quotient map gives

$$
H_q(X,A)\cong\widetilde H_q(X/A).
$$

To prove it, choose such a neighborhood $U$. The first result identifies $H_*(X,A)$ with $H_*(X,U)$. Excision identifies the latter with $H_*(X/A,U/A)$, while $U/A$ is contractible because the deformation retraction can be chosen relative to $A$ using the [homotopy extension property](../../../../../homotopy-extension-property.md). The long exact sequence of the pair $(X/A,U/A)$ then identifies this relative group with $\widetilde H_*(X/A)$.

For $f:(D^n,\partial D^n)\to(D^n,\partial D^n)$, define $\deg f$ by

$$
f_*[D^n,\partial D^n]=(\deg f)[D^n,\partial D^n]
$$

in $H_n(D^n,\partial D^n;\mathbb Z)\cong\mathbb Z$. In the long exact sequence of the pair, the [connecting homomorphism](../../../../../connecting-homomorphism.md)

$$
H_n(D^n,\partial D^n)\xrightarrow{\sim}H_{n-1}(\partial D^n)
$$

is an isomorphism. Naturality shows that $f_*$ and $(f|_{\partial D^n})_*$ multiply the corresponding generators by the same integer, so

$$
\deg f=\deg(f|_{\partial D^n}).
$$

Finally,

$$
(D^n\times I)/\partial(D^n\times I)\cong\Sigma(D^n/\partial D^n)\cong S^{n+1}.
$$

Under this identification, the map induced by $g(x,t)=(f(x),t)$ is the suspension of the map induced by $f$. By [degree under suspension](../../../../../degree-under-suspension.md),

$$
\deg g=\deg f.
$$

This argument proves the needed product assertion directly from the natural suspension isomorphism in reduced homology.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 114](../../paper-114-split.md)
3. [Iii](../../split.md)
4. [2023](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
