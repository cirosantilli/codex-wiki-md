<h1 id="2/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

For $\sigma=1$, the formal outer family is

$$
z_0=A\exp\left(-\frac1{\log x}\right).
$$

Every nonzero member diverges as $x\to1^-$, so bounded matching selects the outer solution $z_0=0$. Boundary layers are now required at both endpoints.

The $x=1$ layer still has width $O(\varepsilon)$ and leading profile

$$
Z_R(X)=e^{-2X},
\qquad X=\frac{1-x}{\varepsilon}.
$$

Near $x=0$, diffusion and the logarithmically vanishing convection balance on the thinner scale

$$
x|\log x|=O(\varepsilon).
$$

At leading order the reaction term is smaller there. Using the supplied first integral with $\mu=\varepsilon^2$, define

$$
S(x)=x^2(2\log^2x-2\log x+1),
\qquad
I(x)=\int_0^x e^{-S(\xi)/\varepsilon^2}\,d\xi.
$$

The left layer that equals $1$ at the endpoint and matches zero is

$$
Z_L(x)=1-\frac{I(x)}{I(1)}.
$$

Consequently a leading composite description is

$$
\boxed{
z(x;\varepsilon)\sim
1-\frac{I(x)}{I(1)}
+\exp\left[-\frac{2(1-x)}{\varepsilon}\right]
}.
$$

Its sketch has value $1$ at each endpoint, drops sharply to an almost-zero outer plateau just to the right of $x=0$, and rises through an $O(\varepsilon)$ layer just before $x=1$.

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [2](../../../2.md)
4. [Paper 336](../../../../paper-336-split.md)
5. [Iii](../../../../split.md)
6. [2021](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
