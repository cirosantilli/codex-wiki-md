<h1 id="19h/solution">Solution</h1>

↑ **Parent:** [19H](../19h.md)

The [permutation representation](../../../../../permutation-representation.md) on the complex [vector](../../../../../vector.md) space with basis $X$ has [permutation character](../../../../../permutation-character.md) $\pi_X(g)=|\operatorname{Fix}_X(g)|$. The multiplicity of the trivial character is $\langle\pi_X,1_G\rangle=|G|^{-1}\sum_g|\operatorname{Fix}(g)|$. Count pairs $(g,x)$ with $gx=x$: each orbit contributes $|G|$, by the [orbit-stabilizer theorem](../../../../../orbit-stabilizer-theorem.md). Hence this multiplicity equals the number of orbits.

For a transitive action the average number of [fixed points](../../../../../fixed-point.md) is one. The identity fixes $|X|>1$ points, so not every other element can fix at least one; otherwise the average would exceed one. Thus there is a derangement $g$ with $\pi_X(g)=0$.

If $\pi_X=1_G+m\chi$, evaluating at that derangement gives $\chi(g)=-1/m$. Character values are algebraic integers, since a finite-order representation [matrix](../../../../../matrix.md) has roots of unity as [eigenvalues](../../../../../eigenvalue.md), and the sum of algebraic integers is integral. A rational [algebraic integer](../../../../../algebraic-integer.md) is an integer. Therefore $-1/m$ is an integer, forcing **$m=1$**.

The diagonal action on $X^2$ is $g(x,y)=(gx,gy)$. Its [permutation character](../../../../../permutation-character.md) is $\pi_X(g)^2$, since both coordinates must be fixed. The orbit-count result and the real-valued character $\pi_X$ give

$$
\boxed{r=\frac1{|G|}\sum_g\pi_X(g)^2=\langle\pi_X,\pi_X\rangle
=1+\sum_{j=2}^km_j^2.}
$$

If any $m_j\geq2$ and another nontrivial constituent occurs, this is at least $1+4+1=6$. If just one nontrivial constituent occurs, the previous result forces its multiplicity to one. Thus $r\leq5$ implies every multiplicity is one, and the formula then gives **$k=r$**.

## ↑ Ancestors (10)

1. [19H](../19h.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ii](../../split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
