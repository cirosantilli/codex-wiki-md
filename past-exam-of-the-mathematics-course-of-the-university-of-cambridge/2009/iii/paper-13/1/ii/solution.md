<h1 id="1/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Count a three-term [arithmetic progression](../../../../../../arithmetic-progression.md) as an ordered triple $(x,x+d,x+2d)$, allowing $d=0$. Inserting [Fourier inversion on a finite group](../../../../../../fourier-inversion-on-a-finite-group.md) into its normalized count and using [additive character](../../../../../../additive-character.md) orthogonality in $x,d$ gives

$$
T=\mathbb E_{x,d}a(x)a(x+d)a(x+2d)
=\sum_r\widehat a(r)^2\widehat a(-2r).
$$

Indeed the two frequency constraints are $r+s+t=0$ and $s+2t=0$, so the surviving frequencies are $(r,s,t)=(t,-2t,t)$. The term at zero is $\alpha^3$.

For odd $N$, let $f=a-\alpha$ be the [balanced indicator function of a finite subset](../../../../../../balanced-indicator-function-of-a-finite-subset.md), and put $M=\max_{s\ne0}|\widehat f(s)|$. Its zero coefficient is zero, and its other coefficients equal those of $a$. Since $-2r\ne0$ when $r\ne0$, the [Parseval identity on a finite group](../../../../../../parseval-identity-on-a-finite-group.md) gives

$$
|T-\alpha^3|\leq M\sum_{r\ne0}|\widehat a(r)|^2\leq M\alpha.
$$

The assumed deficit $T<\alpha^3/2$ therefore forces

$$
\boxed{\max_{s\ne0}|\widehat f(s)|>\frac{\alpha^2}{2}.}
$$

Thus $c=1/2$ and $C=2$ suffice. This is the [large Fourier coefficient from a deficit of three-term progressions](../../../../../../large-fourier-coefficient-from-a-deficit-of-three-term-progressions.md) estimate; no generalized von Neumann theorem is needed. For the remaining prime $N=2$, the count is $T=\mathbb E_{x,d}a(x)a(x+d)=\alpha^2$, so the deficit hypothesis is impossible. The zero common difference was included throughout.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [1](../../1.md)
3. [Paper 13](../../../paper-13-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
