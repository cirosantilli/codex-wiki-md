<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Write

$$
\pi(r)=\mathbb P_{1/2}(0\longleftrightarrow\partial\Lambda_r).
$$

The [Russo-Seymour-Welsh theorem](../../../../../../russo-seymour-welsh-theorem.md) and the [Harris-FKG inequality](../../../../../../harris-fkg-inequality.md) give the standard [one-arm extension estimate](../../../../../../one-arm-extension-estimate.md): there is $c>0$ such that

$$
\pi(2r)\geq c\pi(r)
$$

uniformly in $r$. Indeed, on the one-arm event to scale $r$, a fixed finite collection of open rectangle crossings in the annulus $\Lambda_{2r}\setminus\Lambda_r$, each having probability bounded below by RSW, joins that arm to $\partial\Lambda_{2r}$; FKG multiplies the lower bounds. Iteration shows that $\pi(ar)$ and $\pi(r)$ are comparable for every fixed $a>0$. This proves the estimate suggested in the hint.

Fix $x\in\partial\Lambda_n$ and choose $r=\lfloor n/4\rfloor$. If $0\longleftrightarrow x$, there is an open arm from $0$ to distance $r$ and another from $x$ to distance $r$. These are [independent events](../../../../../../independent-events.md) because they use disjoint edge sets, so the extension estimate gives

$$
\mathbb P_{1/2}(0\longleftrightarrow x)
\leq\pi(r)^2\leq C\pi(n)^2.
$$

For the reverse inequality, take one-arm events from $0$ and $x$ at scale comparable with $n$, in disjoint boxes. A fixed collection of open crossings of rectangles of bounded aspect ratio joins the two arms. The [Russo-Seymour-Welsh theorem](../../../../../../russo-seymour-welsh-theorem.md) bounds the probability of every added crossing below uniformly in $n$ and in the position of $x$ along the four sides; the [Harris-FKG inequality](../../../../../../harris-fkg-inequality.md) and the arm-extension estimate therefore give

$$
\mathbb P_{1/2}(0\longleftrightarrow x)
\geq c\pi(n)^2.
$$

This is the usual [RSW gluing lemma for two one-arm events](../../../../../../rsw-gluing-lemma-for-two-one-arm-events.md). Enlarging the constants handles the finitely many small $n$, proving the claim with positive constants $c_1,c_2$.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 212](../../../paper-212-split.md)
4. [Iii](../../../split.md)
5. [2026](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
