<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Enlarge the space by an independent Brownian motion $W$ and define

$$
B_t=\int_0^t\mathbf1_{\{A_s>0\}}A_s^{-1/2}\,dX_s
+\int_0^t\mathbf1_{\{A_s=0\}}\,dW_s.
$$

The two terms have zero cross-variation and

$$
[B]_t=\int_0^t\mathbf1_{\{A_s>0\}}ds
+\int_0^t\mathbf1_{\{A_s=0\}}ds=t.
$$

The [Lévy characterization of Brownian motion](../../../../../../levy-characterization-of-brownian-motion.md) makes $B$ a Brownian motion. The residual $\int\mathbf1_{\{A=0\}}dX$ has zero quadratic variation and is therefore constant, so

$$
\boxed{X_t-X_0=\int_0^tA_s^{1/2}\,dB_s.}
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [4](../../4.md)
3. [Paper 202](../../../paper-202-split.md)
4. [Iii](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
