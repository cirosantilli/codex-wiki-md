<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Put $q=r_0^2$ and $\eta=d\psi+\tfrac12\cos\theta\,d\phi$. Expanding the [metric tensor](../../../../../../metric-tensor.md) in the stationary direction gives the useful exact identities

$$
g_{tt}=-1+\frac q{r^2},\qquad g_{t\psi}=-\frac{\alpha q}{r^2},\qquad
k=\left(-1+\frac q{r^2}\right)dt-\frac{\alpha q}{r^2}\eta.
$$

Taking the [exterior derivative](../../../../../../exterior-derivative.md) gives

$$
dk=\frac{2q}{r^3}dt\wedge dr
+\frac{2\alpha q}{r^3}dr\wedge\eta
+\frac{\alpha q\sin\theta}{2r^2}d\theta\wedge d\phi.
$$

The fibered form of the [metric tensor](../../../../../../metric-tensor.md) has [determinant](../../../../../../determinant.md) $\det g=-r^6\sin^2\theta/16$. Its inverse components needed for the flux are

$$
g^{tt}=-\frac h f,\qquad g^{t\psi}=-\frac{h\Omega}f,\qquad g^{rr}=f.
$$

Therefore

$$
(dk)^{tr}=f\left[g^{tt}(dk)_{tr}+g^{t\psi}(dk)_{\psi r}\right]
=-\frac{2q}{r^3}h(1-\alpha\Omega)=-\frac{2q}{r^3},
$$

since $h(1-\alpha\Omega)=1$. This calculation includes the rotational mixed term; dropping it prematurely would miss the exact cancellation.

With the stipulated negative coordinate [orientation](../../../../../../orientation-of-a-simplex.md), $\epsilon_{tr\psi\theta\phi}=-r^3\sin\theta/4$. The pullback of the [Hodge star operator](../../../../../../hodge-star-operator.md) to the constant-$t,r$ three-dimensional [spacelike submanifold](../../../../../../spacelike-submanifold.md) is consequently

$$
(\star dk)_{\psi\theta\phi}=\epsilon_{\psi\theta\phi tr}(dk)^{tr}
=\frac q2\sin\theta.
$$

The coordinate ranges and standard sphere identifications give

$$
\int\star dk=\frac q2(2\pi)^2\int_0^\pi\sin\theta\,d\theta=4\pi^2q.
$$

Thus the five-dimensional [Komar mass](../../../../../../komar-mass.md), in the normalization given and $G_5=1$, is

$$
\boxed{M=\frac{3\pi r_0^2}{8}.}
$$

The flux is already independent of $r$ in the vacuum region, so its limit at infinity has the same value. The negative orientation in the question is crucial for the positive sign; reversing that orientation reverses the flux.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3](../../3.md)
3. [Paper 311](../../../paper-311-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
