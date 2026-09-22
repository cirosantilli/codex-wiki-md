<h1 id="1/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Assume $|A+A|\le K|A|$ and put

$$
H=2A-2A.
$$

This set is symmetric, contains zero, and the [Plünnecke-Ruzsa inequality](../../../../../../plunnecke-ruzsa-inequality.md) gives

$$
|H|\le K^4|A|.
$$

It also contains $A-A$, so for every $x\in A$,

$$
A\subseteq H+x.
$$

To control $H+H=4A-4A$, observe again by Plünnecke-Ruzsa that

$$
|(H+H)+A|=|5A-4A|\le K^9|A|.
$$

Apply the [Ruzsa covering lemma](../../../../../../ruzsa-covering-lemma.md) with $S=H+H$ and $T=A$. There is a set $Y$ with $|Y|\le K^9$ such that

$$
H+H\subseteq Y+A-A\subseteq Y+H.
$$

Consequently $H$ is a $K^9$-[approximate group](../../../../../../approximate-group.md). Taking a sufficiently large absolute constant $C$ gives

$$
\boxed{|H|\le CK^C|A|,qquad H\text{ is a }CK^C\text{-approximate group},qquad A\subseteq H+x\ (x\in A).}
$$

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [1](../../1.md)
3. [Paper 129](../../../paper-129-split.md)
4. [Iii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
