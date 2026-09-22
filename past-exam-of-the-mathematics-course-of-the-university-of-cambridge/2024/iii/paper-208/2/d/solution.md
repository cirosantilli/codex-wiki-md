<h1 id="2/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Again put $dQ=Z\,dP$. With $\mathbb E^{[i]}Z=\mathbb E[Z\mid X_i]$, the conditional density of $Q_{X^{(i)}\mid X_i}$ relative to $P_{X^{(i)}}$ is $Z/\mathbb E^{[i]}Z$. Consequently

$$
D(Q_{X^{(i)}\mid X_i}\Vert P_{X^{(i)}}\mid Q_{X_i})
=\mathbb E\left[
Z\log\frac{Z}{\mathbb E^{[i]}Z}\right]
=\mathbb E\operatorname{Ent}_{[i]}(Z).
$$

Part c now gives the alternative tensorization bound

$$
\operatorname{Ent}(Z)
\leq\frac1{n-1}\sum_{i=1}^n
\mathbb E\operatorname{Ent}_{[i]}(Z).
$$

Unlike the bound in part b, each summand averages over all coordinates other than $i$ while holding $X_i$ fixed.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [2](../../2.md)
3. [Paper 208](../../../paper-208-split.md)
4. [Iii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
