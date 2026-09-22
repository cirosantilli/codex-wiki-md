<h1 id="4/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For $s<r<1$, part a gives

$$
\mathbb E\left(\left.\frac{X_1-X_r}{1-r}\right|\mathcal F_s\right)
=\frac{X_1-X_s}{1-s}.
$$

Conditional Fubini then yields

$$
\mathbb E(A_t-A_s\mid\mathcal F_s)
=\frac{t-s}{1-s}(X_1-X_s)
=\mathbb E(X_t-X_s\mid\mathcal F_s).
$$

**Hence $\mathbb E(M_t\mid\mathcal F_s)=M_s$, so $M$ is a martingale.**

## ↑ Ancestors (11)

1. [C](../c.md)
2. [4](../../4.md)
3. [Paper 201](../../../paper-201-split.md)
4. [Iii](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
