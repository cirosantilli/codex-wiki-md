<h1 id="30k/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For $0\leq t\leq1$, [concavity](../../../../../../concave-function.md) of $U$ implies

$$
\begin{aligned}
G(ts_1+(1-t)s_2)
&=\mathbb E\left[U\left(t(m+s_1Z)+(1-t)(m+s_2Z)\right)\right]\\
&\geq tG(s_1)+(1-t)G(s_2),
\end{aligned}
$$

so $G$ is concave.

Since $\mathbb E Z=0$, [Jensen inequality](../../../../../../jensen-s-inequality.md) gives

$$
G(s)=\mathbb E[U(m+sZ)]
\leq U(m+s\mathbb EZ)=U(m)=G(0).
$$

If $0\leq s<t$, concavity and $s=(1-s/t)0+(s/t)t$ yield

$$
G(s)\geq\left(1-\frac st\right)G(0)+\frac stG(t)\geq G(t).
$$

**Hence $G$ is decreasing on $[0,\infty)$; this is [scaled centered risk under concave utility](../../../../../../scaled-centered-risk-under-concave-utility.md).**

## ↑ Ancestors (11)

1. [B](../b.md)
2. [30K](../../30k.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
