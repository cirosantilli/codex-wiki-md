<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Take $d=1$ and start from the lower endpoint. The stationary distribution of this birth-death chain satisfies detailed balance with

$$
\frac{\pi(k+1)}{\pi(k)}=\frac{1/3}{1/6}=2,
$$

so it is concentrated within $O(1)$ of the upper endpoint $n$. Before reaching that region the walk has drift $1/6$. The [weak law of large numbers](../../../../../../weak-law-of-large-numbers.md) and exponential concentration therefore imply that its hitting time of $n-O(1)$ is

$$
6n+O_{\mathbb P}(\sqrt n).
$$

At time $(6-\varepsilon)n$ the chain is still macroscopically below the stationary region with probability tending to one, so its total-variation distance tends to one. Under the monotone coupling from part (b), by time $(6+\varepsilon)n$ the extremal copies have coalesced with probability tending to one, so the distance tends to zero. Therefore the family has

$$
\boxed{\text{cutoff at }6n\text{ with an }O(\sqrt n)\text{ window}.}
$$

## ↑ Ancestors (11)

1. [C](../c.md)
2. [2](../../2.md)
3. [Paper 215](../../../paper-215-split.md)
4. [Iii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
