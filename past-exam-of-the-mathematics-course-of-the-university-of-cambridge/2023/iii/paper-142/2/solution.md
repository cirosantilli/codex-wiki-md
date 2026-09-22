<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

The [Bott isomorphism](../../../../../bott-isomorphism.md) is multiplication by the [Bott element](../../../../../bott-element.md) $\beta\in\widetilde K^0(S^2)$:

$$
K^i(X)\xrightarrow{\ \cong\ }
\widetilde K^i(S^2\wedge X)
\cong K^{i-2}(X).
$$

Together with the [suspension isomorphism](../../../../../suspension-isomorphism.md) and

$$
K^0(\mathrm{pt})=\mathbb Z,
\qquad
K^{-1}(\mathrm{pt})=0,
$$

it gives the [Complex K-theory of a sphere](../../../../../complex-k-theory-of-a-sphere.md)

$$
\widetilde K^i(S^d)\cong K^{i-d}(\mathrm{pt})
\cong
\begin{cases}
\mathbb Z,&i-d\text{ even},\\
0,&i-d\text{ odd}.
\end{cases}
$$

Let

$$
\varnothing=Y_{-1}\subset Y_0\subset\cdots\subset Y_m=Y
$$

be a [CW filtration](../../../../../cw-filtration.md) in which each quotient $Y_r/Y_{r-1}$ is a wedge of even-dimensional spheres. The six-term exact sequence in [Topological K-theory](../../../../../topological-k-theory.md), the sphere calculation, and induction give

$$
K^{-1}(Y_r)=0
$$

and a short exact sequence whose new summand in $K^0(Y_r)$ is free abelian on the newly attached cells. Every such extension splits as an extension of [free abelian groups](../../../../../free-abelian-group.md), so $K^0(Y)$ is free, with one generator for each cell. This proves the [Complex K-theory of an even-cell complex](../../../../../complex-k-theory-of-an-even-cell-complex.md) result.

The exterior product defines

$$
K^0(Y)\otimes K^i(X)\longrightarrow K^i(Y\times X).
$$

For a point it is the identity. Attaching one layer of even cells gives corresponding exact sequences on the source and target; the sphere case is the [suspension isomorphism](../../../../../suspension-isomorphism.md), and induction with the [Five lemma](../../../../../five-lemma.md) proves that the product map remains an isomorphism. This is the [Künneth theorem for complex K-theory with an even-cell factor](../../../../../kunneth-theorem-for-complex-k-theory-with-an-even-cell-factor.md).

For a [mapping torus](../../../../../mapping-torus.md) $T_f$, the [K-theory Wang sequence of a mapping torus](../../../../../k-theory-wang-sequence-of-a-mapping-torus.md) contains

$$
K^{-1}(Z)\xrightarrow{1-f^*}K^{-1}(Z)
\longrightarrow K^0(T_f)
\longrightarrow K^0(Z)\xrightarrow{1-f^*}K^0(Z).
$$

When $K^{-1}(Z)=0$, exactness gives

$$
K^0(T_f)\cong\ker(1-f^*:K^0(Z)\to K^0(Z)).
$$

For $Z=\mathbb{CP}^2\times\mathbb{CP}^2$, the [Complex K-theory of complex projective space](../../../../../complex-k-theory-of-complex-projective-space.md) and the K-theory Künneth isomorphism give

$$
K^0(Z)\cong\mathbb Z[x,y]/(x^3,y^3).
$$

The factor swap interchanges $x$ and $y$. Its invariant subgroup has the basis

$$
1,\quad xy,\quad x^2y^2,\quad x+y,\quad x^2+y^2,\quad xy^2+x^2y.
$$

It follows that the [K-theory of the mapping torus of the factor swap on two complex projective planes](../../../../../k-theory-of-the-mapping-torus-of-the-factor-swap-on-two-complex-projective-planes.md) is

$$
\boxed{K^0(T_f)\cong\mathbb Z^6.}
$$

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 142](../../paper-142-split.md)
3. [Iii](../../split.md)
4. [2023](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
