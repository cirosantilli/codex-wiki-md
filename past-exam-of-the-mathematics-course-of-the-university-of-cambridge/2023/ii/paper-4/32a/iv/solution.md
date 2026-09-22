<h1 id="32a/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

Let $x^*(\lambda)=\sqrt{1-1/\lambda}$ and center the map at this parameter-dependent fixed point:

$$
G(X,\mu)=F(x^*(2+\mu)+X,2+\mu)-x^*(2+\mu).
$$

A [Taylor polynomial](../../../../../../taylor-polynomial.md) in $X$, with the coefficients expanded at $(x,\lambda)=(1/\sqrt2,2)$, gives

$$
G(X,\mu)=-X+\alpha\mu X+\beta X^2+\gamma X^3+O(\mu^2)
$$

under the period-doubling scaling $X=O(\sqrt\mu)$. The coefficients are

$$
\alpha=\left.\frac{d}{d\lambda}F_x(x^*(\lambda),\lambda)\right|_{\lambda=2}=-2,
$$



$$
\beta=\frac12F_{xx}\left(\frac1{\sqrt2},2\right)=-3\sqrt2,
\qquad
\gamma=\frac16F_{xxx}\left(\frac1{\sqrt2},2\right)=-2.
$$

Here we used $F_x(x^*(\lambda),\lambda)=3-2\lambda$, $F_{xx}=-6\lambda x$, and $F_{xxx}=-6\lambda$.

Composing the local map with itself and retaining the terms of order $\mu X$ and $X^3$ gives

$$
G(G(X,\mu),\mu)-X
=-2\alpha\mu X-2(\gamma+\beta^2)X^3
+o(\mu X+X^3).
$$

Besides the fixed solution $X=0$, the two leading solutions therefore satisfy

$$
X^2=-\frac{\alpha\mu}{\gamma+\beta^2}.
$$

Thus the period-two points born at $\lambda=2$ are

$$
\boxed{x_\pm=x^*\pm
\sqrt{\frac{-\alpha\mu}{\gamma+\beta^2}}}
$$

to leading order. With the coefficients above, the radicand is positive for $\mu>0$.

## ↑ Ancestors (11)

1. [Iv](../iv.md)
2. [32A](../../32a.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
