<h1 id="5/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For fixed $s\in(0,1)$, uniqueness gives

$$
\{M^*\leq s\}
=\left\{\max_{t\leq s}B_t-B_s
\geq\max_{s\leq t\leq1}(B_t-B_s)\right\}.
$$

The two sides of the comparison are independent and distributed as $\sqrt s|Z_1|$ and $\sqrt{1-s}|Z_2|$ for independent standard normal random variables. Rotational invariance of $(Z_1,Z_2)$ makes its angle uniform, so

$$
\begin{aligned}
\mathbb P(M^*\leq s)
&=\mathbb P\left(\frac{|Z_2|}{|Z_1|}\leq\sqrt{\frac{s}{1-s}}\right)\\
&=\frac2\pi\arctan\sqrt{\frac{s}{1-s}}
=\frac2\pi\arcsin\sqrt s.
\end{aligned}
$$

The endpoint values follow by continuity. Thus the [time of the Brownian maximum](../../../../../../time-of-the-brownian-maximum.md) has the arcsine distribution.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [5](../../5.md)
3. [Paper 201](../../../paper-201-split.md)
4. [Iii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
