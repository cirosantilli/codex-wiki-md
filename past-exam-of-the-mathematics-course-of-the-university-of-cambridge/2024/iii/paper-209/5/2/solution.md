<h1 id="5/2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Set $N=3^j$. At $p=1/2$, first use the [Russo-Seymour-Welsh theorem](../../../../../../russo-seymour-welsh-theorem.md) to produce, with probability bounded below independently of $N$, two separated open crossings from left to right and a closed crossing between them. Explore the interface separating the lower open cluster from the adjacent closed cluster until it reaches the opposite macroscopic boundary. The explored interface supplies two alternating arms, while fresh RSW crossings in the unexplored regions supply the other two.

Repeat this construction in the geometrically separated scale bands

$$
3^k\leq r\leq3^{k+1},
\qquad k=2,\ldots,j-1.
$$

The [domain Markov property of a percolation exploration](../../../../../../domain-markov-property-of-a-percolation-exploration.md) leaves unrevealed sites with their original independent critical law. RSW and the [Harris-FKG inequality](../../../../../../harris-fkg-inequality.md) therefore give a uniform conditional probability $c>0$ that the required open and closed connections occur in each band. On that event the exploration identifies a site having four alternating arms to the four sides of $W_N$, hence a pivotal site for $E_N$.

Choose the candidates in disjoint scale bands, so successful bands give distinct pivotal sites. If $Y_k$ indicates success at scale $k$, then

$$
N_{\mathrm{piv}}(E_N)\geq\sum_{k=2}^{j-1}Y_k,
\qquad
\mathbb E_{1/2}Y_k\geq c.
$$

Thus

$$
\left.\frac d{dp}\mathbb P_p(E_N)\right|_{p=1/2}
=\mathbb E_{1/2}N_{\mathrm{piv}}(E_N)
\geq c(j-2)\geq c'j
$$

for $j\geq2$, after adjusting the positive constant. This is the required logarithmic-in-$N$ lower bound.

## ↑ Ancestors (11)

1. [2](../2.md)
2. [5](../../5.md)
3. [Paper 209](../../../paper-209-split.md)
4. [Iii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
