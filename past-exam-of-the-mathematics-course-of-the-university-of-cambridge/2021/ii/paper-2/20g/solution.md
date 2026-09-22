<h1 id="20g/solution">Solution</h1>

↑ **Parent:** [20G](../20g.md)

An element $\alpha$ is [algebraic](../../../../../algebraic-element.md) over $\mathbb Q$ when it is a root of a nonzero polynomial in $\mathbb Q[X]$. Clearing denominators gives

$$
a_0+a_1\alpha+\cdots+a_d\alpha^d=0,
\qquad a_i\in\mathbb Z,quad a_0\ne0.
$$

For $\alpha\ne0$, take $\beta=-(a_1+a_2\alpha+\cdots+a_d\alpha^{d-1})\in\mathbb Z[\alpha]$; then $\alpha\beta=a_0\ne0$.

Since $K=\operatorname{Frac}R$, write $x=a/b$ with $a,b\in R$ and $b\ne0$. Applying the first result to $b$ gives $b\beta=m\in\mathbb Z\setminus\{0\}$, whence $x=a\beta/m$. Changing signs makes $m>0$.

Choose a $\mathbb Z$-basis $e_1,\ldots,e_d$ of $\mathcal O_K$. Write each $e_i=r_i/m_i$ as above and take a common multiple $m$. Then

$$
m\mathcal O_K\subseteq R\subseteq\mathcal O_K.
$$

Thus $R$ is a free abelian group of rank $d=[K:\mathbb Q]$ and has finite index in $\mathcal O_K$. If $0\ne a\in I$, then $aR\subseteq I$ and multiplication by $a$ has nonzero determinant on the rank-$d$ lattice $R$, so $(R:aR)$, and hence $(R:I)$, is finite. Also $m\mathcal O_K\subseteq R$ is an ideal of $R$.

Put $h=(\mathcal O_K:R)$ and $I=m\mathcal O_K$. Then

$$
(R:I)=\frac{m^d}{h},
\qquad
(R:I^2)=\frac{m^{2d}}h.
$$

The assumed multiplicativity of indices gives

$$
\frac{m^{2d}}h=\left(\frac{m^d}h\right)^2,
$$

so $h=1$. Therefore $\boxed{R=\mathcal O_K}$.

## ↑ Ancestors (10)

1. [20G](../20g.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ii](../../split.md)
4. [2021](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
