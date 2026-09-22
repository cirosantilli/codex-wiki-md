<h1 id="8/solution">Solution</h1>

↑ **Parent:** [8](../8.md)

A [right coset](../../../../right-coset.md) of $H$ in $G$ is $Hg=\{hg:h\in H\}$. Right multiplication by $g$ is a [bijection](../../../../bijection.md) $H\to Hg$, with inverse $x\mapsto xg^{-1}$, so every right coset has $|H|$ elements. The analogous map $h\mapsto gh$ proves the same assertion for [left cosets](../../../../left-coset.md).

Write the displayed matrices as $M(a,b,c)$. Direct multiplication gives

$$
M(a,b,c)M(A,B,C)=M(a+A,b+B+aC,c+C).
$$

All new coordinates are integers, so the set is closed. Matrix multiplication is associative, the identity is $M(0,0,0)$, and

$$
\boxed{M(a,b,c)^{-1}=M(-a,ac-b,-c),}
$$

which also has integer coordinates. Thus it is the [Integer Heisenberg group](../../../../integer-heisenberg-group.md).

The subset $H=\{M(0,0,t):t\in\mathbb Z\}$ contains the identity, and multiplication and inversion add or negate $t$, so it is a [subgroup](../../../../subgroup.md). Its [right cosets](../../../../right-coset.md) are

$$
\boxed{HM(a,b,c)=\{M(a,b,c+t):t\in\mathbb Z\}=\{M(a,b,s):s\in\mathbb Z\}.}
$$

They are exactly the sets with fixed integer coordinates $(a,b)$, as described by [cosets of a coordinate subgroup of the integer Heisenberg group](../../../../cosets-of-a-coordinate-subgroup-of-the-integer-heisenberg-group.md). The factor order $HM$ is essential; multiplying by $H$ on the other side would also change the upper-right coordinate by $at$.

## ↑ Ancestors (12)

1. [8](../8.md)
2. [Paper 2](../../paper-2-split.md)
3. [2004](../../split.md)
4. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../split.md)
5. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
6. [Year 2 of the natural sciences course of the University of Cambridge](../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year of the natural sciences course of the University of Cambridge](../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Natural sciences course of the University of Cambridge](../../../../natural-sciences-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
