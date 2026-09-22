<h1 id="5/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Apply the [Itô formula](../../../../../../ito-s-lemma.md) to $f(t,x)=x_0e^{\sigma x+(\mu-\sigma^2/2)t}$ and the semimartingale vector $(t,B_t)$. Its derivatives give

$$
dX_t=\mu X_t\,dt+\sigma X_t\,dB_t.
$$

Therefore

$$
X_t=x_0\exp\left(\sigma B_t+
\left(\mu-\frac12\sigma^2\right)t\right).
$$

This is adapted to the given Brownian filtration and is consequently a strong solution; it is [geometric Brownian motion](../../../../../../geometric-brownian-motion.md).

## ↑ Ancestors (11)

1. [D](../d.md)
2. [5](../../5.md)
3. [Paper 202](../../../paper-202-split.md)
4. [Iii](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
