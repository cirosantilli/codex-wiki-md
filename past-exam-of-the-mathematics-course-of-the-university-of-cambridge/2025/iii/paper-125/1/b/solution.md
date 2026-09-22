<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The [zeta function of an elliptic curve over a finite field](../../../../../../zeta-function-of-an-elliptic-curve-over-a-finite-field.md) is the formal power series

$$
Z_E(T)=\exp\left(\sum_{r\geq1}\#E(\mathbb F_{p^r})\frac{T^r}{r}\right).
$$

The proof of Hasse's theorem gives the characteristic equation $\pi^2-[a]\pi+[p]=0$. If $\alpha,\beta$ are the roots of $X^2-aX+p$, then the [elliptic-curve point count over a finite field](../../../../../../elliptic-curve-point-count-over-a-finite-field.md) is

$$
\#E(\mathbb F_{p^r})=p^r+1-\alpha^r-\beta^r.
$$

Using $\exp(\sum_{r\geq1}u^rT^r/r)=(1-uT)^{-1}$ therefore gives

$$
\boxed{Z_E(T)=\frac{(1-\alpha T)(1-\beta T)}{(1-T)(1-pT)}
=\frac{1-aT+pT^2}{(1-T)(1-pT)}.}
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 125](../../../paper-125-split.md)
4. [Iii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
