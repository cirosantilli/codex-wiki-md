<h1 id="2f/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

An elementary geometric-series construction suffices, without assuming a general polynomial-approximation theorem. Rotate the square by a multiple of $\pi/2$ so that $\Re w>1$. Put $c=-R$ with $R>0$. Every point of the square then satisfies $|z-c|^2\le(R+1)^2+1$, whereas

$$
|w-c|^2-\bigl[(R+1)^2+1\bigr]
=2R(\Re w-1)+|w|^2-2>0
$$

for sufficiently large $R$. Thus the whole square lies inside a disk centred at $c$ whose radius is less than $|w-c|$. The other three ways $w$ can lie outside the square are handled by the indicated rotations, after which rotating back preserves [polynomial](../../../../../../polynomial-split.md) form.

Now expand

$$
\frac1{z-w}
=-\frac1{w-c}\frac1{1-(z-c)/(w-c)}
=-\sum_{j=0}^{\infty}\frac{(z-c)^j}{(w-c)^{j+1}}.
$$

Let $\rho=\max_{z\in K}|z-c|/|w-c|<1$. The tail after degree $m$ is uniformly bounded by $\rho^{m+1}/[|w-c|(1-\rho)]$, tending to zero. Hence the displayed partial sums are the required **uniform [polynomial approximations](../../../../../../polynomial-approximation.md)**. This is the [Taylor series](../../../../../../taylor-series.md) about a carefully chosen distant centre, rather than a potentially inadequate series about $0$.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [2F](../../2f.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2005](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
