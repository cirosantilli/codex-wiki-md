<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

One form of the [Mumford rigidity lemma](../../../../../../mumford-rigidity-lemma.md) says that if $X$ is a complete variety, $S$ is connected, and a morphism $F:X\times S\to Z$ maps $X\times\{s_0\}$ to one point, then $F$ factors through the projection to $S$. In particular, if $F$ also maps $\{x_0\}\times S$ to that point, then $F$ is constant.

Choose $s_0\in S(k)$ and put $g=f|_{X\times\{s_0\}}$. To see that the pointed morphism $g:X\to Y$ is a homomorphism, apply rigidity to

$$
D(x_1,x_2)=g(x_1+x_2)-g(x_1)-g(x_2).
$$

It vanishes on $X\times\{e\}$, so it factors through the second projection; it also vanishes on $\{e\}\times X$, so it is identically zero. Now define

$$
F(x,s)=f(x,s)-g(x).
$$

Then $F(x,s_0)=e$ for every $x$ and $F(e,s)=e$ for every $s$. Rigidity forces $F$ to be identically $e$, so

$$
\boxed{f|_{X\times\{s\}}=g\in\operatorname{Hom}_k(X,Y)\quad\text{for every }s\in S(k).}
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 126](../../../paper-126-split.md)
4. [Iii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
