<h1 id="7b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Each element of $H$ permutes the three-point set, giving a [group homomorphism](../../../../../../group-homomorphism.md) $\rho:H\to S_3$. To prove injectivity, let an element fix all three points. Conjugate it by the normalizing [Möbius transformation](../../../../../../mobius-transformation.md) from part (i). The conjugate fixes $0,1,\infty$. A [Möbius transformation](../../../../../../mobius-transformation.md) $z\mapsto(az+b)/(cz+d)$ fixing $0$ has $b=0$, and fixing infinity has $c=0$. It is then $z\mapsto kz$; fixing $1$ forces $k=1$. Thus the conjugate, and hence the original transformation, is the identity. The [kernel of a group homomorphism](../../../../../../kernel-of-a-group-homomorphism.md) is trivial.

For surjectivity, let $(x_1,x_2,x_3)=(\alpha,\beta,\gamma)$ and choose any permutation $\sigma$. Let $g$ normalize the ordered triple $(x_1,x_2,x_3)$ and let $g_\sigma$ normalize $(x_{\sigma(1)},x_{\sigma(2)},x_{\sigma(3)})$. Then $g_\sigma^{-1}g$ sends $x_j$ to $x_{\sigma(j)}$, lies in $H$, and induces the chosen permutation. Thus $\rho$ is onto and

$$
\boxed{H\cong S_3}.
$$

For the normalized set, the six [Möbius transformations permuting three points](../../../../../../mobius-transformations-permuting-three-points.md) are $z$, $1-z$, $1/z$, $1/(1-z)$, $z/(z-1)$, and $(z-1)/z$. Conjugating by $g$ gives the corresponding six maps for the original set.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [7B](../../7b.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ia](../../../split.md)
5. [2003](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
