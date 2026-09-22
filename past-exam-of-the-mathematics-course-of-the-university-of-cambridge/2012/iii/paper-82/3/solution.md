<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Use the density form of the [Szemerédi theorem](../../../../../szemeredi-s-theorem.md): for fixed $\alpha>0$ and length $r$, every sufficiently large subset of $\{1,\ldots,N\}$ of size at least $\alpha N$ contains a nonconstant [arithmetic progression](../../../../../arithmetic-progression.md) of length $r$, as established in [Szemerédi's density theorem](https://matwbn.icm.edu.pl/ksiazki/aa/aa27/aa27132.pdf). This theorem supplies a progression, not the desired averaging configuration; we now select the actual indices.

Take $r=2k+1$. Write the resulting progression as

$$
a,a+d,\ldots,a+2kd\in A,\qquad d\ge1,
$$

and put $y=a+kd\in A$. If $k=2m$ is even, select $y-d,y+d,\ldots,y-md,y+md$. These are $2m=k$ distinct members of the progression, and each opposite pair sums to $2y$. If $k=2m+1$ is odd, select those $2m$ opposite points together with $y$ itself. All $k$ selected points are distinct, and their sum is again $ky$. The case $k=1$ simply selects $y$.

In both cases the indices stay between $0$ and $2k$ and the difference $d$ is nonzero. Thus the precise answer is

$$
\boxed{x_1,\ldots,x_k\in A\text{ distinct},\qquad\frac{x_1+\cdots+x_k}{k}=y\in A.}
$$

No deletion of diagonal solutions and no multidimensional density theorem is needed. The averaging point is allowed to be one of the selected points, as it is in the odd case.

## ↑ Ancestors (11)

1. [3](../3.md)
2. [Section B](../section-b.md)
3. [Paper 82](../../paper-82-split.md)
4. [Iii](../../split.md)
5. [2012](../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
