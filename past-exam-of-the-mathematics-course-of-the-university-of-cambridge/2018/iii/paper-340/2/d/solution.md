<h1 id="2/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Normalize $\widehat\varphi(0)=1$, as in the displayed product convention. Iterating the [scaling refinement equation](../../../../../../scaling-refinement-equation.md) gives $\widehat\varphi(\xi)=\prod_{j\ge1}m(\xi/2^j)$. The finite-product identity

$$
\prod_{j=1}^J\frac{1+e^{-i\xi/2^j}}2
=\frac{1-e^{-i\xi}}{2^J(1-e^{-i\xi/2^J})}
\longrightarrow\frac{1-e^{-i\xi}}{i\xi}
$$

has the value one at zero by continuity. Therefore

$$
\boxed{\widehat\varphi(\xi)=\left(\frac{1-e^{-i\xi}}{i\xi}\right)^N\prod_{j\ge1}L(\xi/2^j).}
$$

Write $M=\sup|L|$. Since $L(0)=1$, we have $M\ge1$. For $|\xi|>1$, take $J=\lceil\log_2|\xi|\rceil$. The first $J$ factors are bounded by $M^J\le M|\xi|^{\log_2M}$. For the remaining factors, the [trigonometric polynomial](../../../../../../trigonometric-polynomial.md) satisfies $|L(t)|\le1+C|t|$ on $|t|\le1$, hence

$$
\prod_{j>J}|L(\xi/2^j)|\le\exp\left(C\sum_{j>J}|\xi|2^{-j}\right)\le e^C.
$$

Using $|(1-e^{-i\xi})/(i\xi)|\le\min(1,2/|\xi|)$ gives

$$
|\widehat\varphi(\xi)|\le C'(1+|\xi|)^{-N+\log_2M}.
$$

The strict hypothesis permits $\varepsilon>0$ with $N-\log_2M\ge\alpha+1+\varepsilon$. The given Fourier-decay criterion proves **uniform Hölder regularity of exponent $\alpha$**. For the ordinary increment definition of [Hölder continuity](../../../../../../holder-condition.md), take $0<\alpha\le1$: Fourier inversion and $|e^{ih\xi}-1|\le C_\alpha|h\xi|^\alpha$ directly give the required bound. If $\alpha>1$, “Lipschitz-$\alpha$” must mean higher-order [Hölder space](../../../../../../holder-space.md) regularity; an ordinary increment bound of exponent greater than one forces a function to be constant. An unnormalized [scaling function](../../../../../../scaling-function.md) contributes its constant phase to the product formula.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [2](../../2.md)
3. [Paper 340](../../../paper-340-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
