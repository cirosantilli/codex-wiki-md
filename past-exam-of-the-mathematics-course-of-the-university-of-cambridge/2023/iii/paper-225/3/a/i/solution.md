<h1 id="3/a/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Because a strictly monotone map fixing both endpoints is increasing, the [change of variables formula](../../../../../../../change-of-variables-formula.md) $t=h(s)$ gives

$$
\lVert Y\rVert^2
=\int_0^1X(h^{-1}(t))^2\,dt
=\int_0^1X(s)^2h'(s)\,ds.
$$

Assuming $\mathbb E\lVert X\rVert^2>0$, define

$$
A=\frac{\mathbb E\int_0^1X(s)^2h'(s)\,ds}
{\mathbb E\int_0^1X(s)^2\,ds}.
$$

The Hilbert-space variance identity then gives

$$
\begin{aligned}
\mathbb E\lVert Y-\mu\rVert^2
&=\mathbb E\lVert Y\rVert^2-\lVert\mu\rVert^2\\
&=A\mathbb E\lVert X\rVert^2-\lVert\mu\rVert^2\\
&=A\mathbb E\lVert X-\nu\rVert^2+A\lVert\nu\rVert^2-\lVert\mu\rVert^2.
\end{aligned}
$$

Under the regularity needed to interchange expectation and differentiation, $\mathbb Eh'(s)=1$ because $\mathbb Eh(s)=s$. Hence

$$
A=1+
\frac{\int_0^1\operatorname{Cov}(X(s)^2,h'(s))\,ds}
{\mathbb E\lVert X\rVert^2}.
$$

**Thus $A=1$ exactly when the integrated covariance in the numerator vanishes. In particular, this holds when the amplitude $X$ and the time warp $h$ are [independent random variables](../../../../../../../independent-random-variables.md).**

## ↑ Ancestors (12)

1. [I](../i.md)
2. [A](../../a.md)
3. [3](../../../3.md)
4. [Paper 225](../../../../paper-225-split.md)
5. [Iii](../../../../split.md)
6. [2023](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
