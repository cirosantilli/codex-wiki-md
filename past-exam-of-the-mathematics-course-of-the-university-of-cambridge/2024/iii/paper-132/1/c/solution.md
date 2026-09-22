<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Let the blue edges form a graph $B$ on $N$ vertices, and suppose there is no blue copy of $H$. For every vertex $x$, the graph $B[N_B(x)]$ has maximum degree at most one. Indeed, if some $y\in N_B(x)$ had two neighbours $z,w$ inside $N_B(x)$, then

$$
xy,xz,xw,yz,yw
$$

would be the five blue edges of a copy of $H$.

Let $d=\Delta(B)$. If $d\ge2k$, then a maximum-degree neighbourhood, being a matching plus isolated vertices, has an independent set of size at least $d/2\ge k$. This is a red $K_k$. We may therefore assume $d<2k$. Part (b) gives

$$
\alpha(B)\ge c\frac{N\log d}{d}.
$$

If $d<\sqrt{k}$, the [greedy independent-set bound](../../../../../../greedy-independent-set-bound.md) gives $\alpha(B)\ge N/(d+1)>k$ once $N=Ck^2/\log k$. If $\sqrt{k}\le d<2k$, then part (b) gives

$$
\alpha(B)\ge c'\frac{N\log k}{k}\ge k
$$

when $C$ is sufficiently large. In either case there is a red $K_k$, so

$$
\boxed{r(H,K_k)\le Ck^2/\log k.}
$$

## ↑ Ancestors (11)

1. [C](../c.md)
2. [1](../../1.md)
3. [Paper 132](../../../paper-132-split.md)
4. [Iii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
