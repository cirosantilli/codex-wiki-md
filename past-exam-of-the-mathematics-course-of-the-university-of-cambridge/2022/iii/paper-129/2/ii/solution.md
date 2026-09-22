<h1 id="2/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Let $G_0=\mathbb F_p^n$ and let

$$
\Gamma=\{(x,\phi(x)):x\in G_0\}\subseteq G_0\times G_0.
$$

For each fixed first coordinate $d$, the second coordinates occurring in $\Gamma-\Gamma$ are values of $\phi(x+d)-\phi(x)$, of which there are at most $C$. Therefore

$$
|\Gamma-\Gamma|\leq C|G_0|=C|\Gamma|.
$$

The difference-set form of the [Plünnecke-Ruzsa inequality](../../../../../../plunnecke-ruzsa-inequality.md) now gives

$$
|3\Gamma-2\Gamma|\leq C^5|\Gamma|.
$$

Every $u\in X$ has the form

$$
(0,u)=(x,\phi(x))-(x+a,\phi(x+a))-(x+b,\phi(x+b))+(x+a+b,\phi(x+a+b)),
$$

so $\{0\}\times X\subseteq2\Gamma-2\Gamma$. Consequently

$$
(\{0\}\times X)+\Gamma\subseteq3\Gamma-2\Gamma.
$$

The set on the left has exactly $|X||\Gamma|$ elements, since its fiber over each $x$ is $\phi(x)+X$. It follows that

$$
|X||\Gamma|\leq C^5|\Gamma|,
$$

and hence $|X|\leq C^5$.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [2](../../2.md)
3. [Paper 129](../../../paper-129-split.md)
4. [Iii](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
