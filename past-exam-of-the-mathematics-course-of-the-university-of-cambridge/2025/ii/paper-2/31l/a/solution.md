<h1 id="31l/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

A set of points $x_1,\ldots,x_n$ is shattered by $H$ when every one of the $2^n$ binary label vectors is realized by some $h\in H$. The [shattering coefficient](../../../../../../shattering-coefficient.md) is

$$
s(H,n)=\max_{x_1,\ldots,x_n}
\left|\{(h(x_1),\ldots,h(x_n)):h\in H\}\right|,
$$

and the [VC dimension](../../../../../../vc-dimension.md) is

$$
VC(H)=\sup\{n:s(H,n)=2^n\}.
$$

The Sauer--Shelah lemma states that if $VC(H)=D<\infty$, then

$$
s(H,n)\leq\sum_{j=0}^{D}\binom nj
$$

for every $n$; in particular $s(H,n)\leq(n+1)^D$.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [31L](../../31l.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
