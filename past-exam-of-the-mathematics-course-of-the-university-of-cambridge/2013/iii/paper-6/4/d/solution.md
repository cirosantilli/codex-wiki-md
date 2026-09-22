<h1 id="4/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Apply the spherical identity of part (b) with $x=v-v_*$, $y=\xi$ and $\phi(s)=e^{-is/2}$. The angular exponential in part (c) can be replaced, after angular integration, by $e^{-i|\xi|(v-v_*)\cdot\sigma/2}$. The full phase is then

$$
-i v\cdot\frac{\xi+|\xi|\sigma}{2}-i v_*\cdot\frac{\xi-|\xi|\sigma}{2}.
$$

The [Fubini theorem](../../../../../../fubini-s-theorem.md) factors the two velocity [integrals](../../../../../../integral.md) into [Fourier transforms](../../../../../../fourier-transform.md). With $\xi^\pm=(\xi\pm|\xi|\sigma)/2$, the gain [integral](../../../../../../integral.md) is exactly $\int_{\mathbb S^2}\widehat f(\xi^+)\widehat f(\xi^-)\,d\sigma$.

The loss [Fourier transform](../../../../../../fourier-transform.md) is $\widehat f(\xi)\widehat f(0)$. Dividing the gain by the [sphere](../../../../../../sphere.md) area gives the [Bobylev identity](../../../../../../bobylev-identity.md) for the [Maxwell molecule collision operator](../../../../../../maxwell-molecule-collision-operator.md):

$$
\boxed{\partial_t\widehat f(\xi)=\frac1{|\mathbb S^2|}\int_{\mathbb S^2}\widehat f(\xi^+)\widehat f(\xi^-)\,d\sigma-\widehat f(\xi)\widehat f(0)}.
$$

The initial Fourier datum is $\widehat f_0$. The [surface measure on a sphere](../../../../../../surface-measure-on-a-sphere.md) here is two-dimensional surface area, not the restriction of ambient three-dimensional [Lebesgue measure](../../../../../../lebesgue-measure.md), which would give the [sphere](../../../../../../sphere.md) measure zero.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [4](../../4.md)
3. [Paper 6](../../../paper-6-split.md)
4. [Iii](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
