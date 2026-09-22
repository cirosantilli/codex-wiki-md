<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Let $G=\operatorname{Gal}(L/K)$ and normalize $v_L$. In lower numbering,

$$
G_{-1}=G,
\qquad
G_s=\{\sigma\in G:v_L(\sigma(x)-x)\geq s+1\text{ for every }x\in\mathcal O_L\}
\quad(s\geq0).
$$

These are the [ramification groups](../../../../../../ramification-group.md); $G_0$ is the [inertia group](../../../../../../inertia-group.md) and $G_1$ is the [wild inertia group](../../../../../../wild-inertia-group.md).

Because $\mathcal O_L=\mathcal O_K[\alpha]$, every $x\in\mathcal O_L$ is $P(\alpha)$ for some $P\in\mathcal O_K[X]$. The polynomial identity $P(Y)-P(X)=(Y-X)Q(X,Y)$ has integral coefficients. Consequently the inequality for $\alpha$ implies it for every $x$, and the converse follows by taking $x=\alpha$. Therefore

$$
G_s=\{\sigma\in G:v_L(\sigma(\alpha)-\alpha)\geq s+1\}.
$$

Since $L/K$ is a [Finite Galois extension](../../../../../../finite-galois-extension.md), the minimal polynomial factors as

$$
f(X)=\prod_{\sigma\in G}(X-\sigma(\alpha)).
$$

Differentiating and evaluating at $\alpha$ gives

$$
f'(\alpha)=\prod_{1\ne\sigma\in G}(\alpha-\sigma(\alpha)),
$$

and hence

$$
v_L(f'(\alpha))
=\sum_{1\ne\sigma\in G}v_L(\sigma(\alpha)-\alpha).
$$

For a fixed nonidentity $\sigma$, its valuation is exactly the number of integers $s\geq0$ for which $\sigma\in G_s$. Interchanging the two finite sums proves the [ramification-group sum for a monogenic integer ring](../../../../../../ramification-group-sum-for-a-monogenic-integer-ring.md):

$$
v_L(f'(\alpha))=\sum_{s\geq0}(|G_s|-1).
$$

The extension is unramified exactly when $G_0=1$, which by this nonnegative sum is equivalent to $v_L(f'(\alpha))=0$, or $f'(\alpha)\in\mathcal O_L^\times$. Moreover $|G_0|=e(L/K)$, so the $s=0$ term is $e(L/K)-1$. Equality

$$
v_L(f'(\alpha))=e(L/K)-1
$$

holds exactly when $G_1=1$, which is exactly tame ramification.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 136](../../../paper-136-split.md)
4. [Iii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
