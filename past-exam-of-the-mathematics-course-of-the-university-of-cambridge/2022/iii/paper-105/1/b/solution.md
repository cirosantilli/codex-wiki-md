<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The [Lax-Milgram theorem](../../../../../../lax-milgram-theorem.md) says that if $H$ is a real [Hilbert space](../../../../../../hilbert-space-split.md), $B:H\times H\to\mathbb R$ is a bounded bilinear form satisfying

$$
B(v,v)\geq\alpha\lVert v\rVert_H^2
$$

for some $\alpha>0$, and $F\in H^*$, then there is a unique $u\in H$ such that $B(u,v)=F(v)$ for every $v\in H$.

For this problem take $H=H_0^1(U)$ and

$$
B(u,v)=\int_U\big(Du\cdot Dv+(D_nu)v+uv\big),
\qquad
F(v)=\int_Ufv.
$$

The [Cauchy-Schwarz inequality](../../../../../../cauchy-schwarz-inequality.md) and the continuous embedding $H_0^1(U)\hookrightarrow L^2(U)$ make both maps bounded. For smooth zero-boundary functions, integration by parts gives

$$
\int_U(D_nu)u=\frac12\int_U D_n(u^2)=0;
$$

density extends this identity to $H_0^1(U)$. Consequently

$$
B(u,u)=\lVert Du\rVert_2^2+\lVert u\rVert_2^2=\lVert u\rVert_{H^1}^2,
$$

so $B$ is coercive. Lax–Milgram supplies the unique weak solution.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 105](../../../paper-105-split.md)
4. [Iii](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
