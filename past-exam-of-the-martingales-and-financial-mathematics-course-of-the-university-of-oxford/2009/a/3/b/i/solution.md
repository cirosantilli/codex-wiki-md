<h1 id="a/3/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Use $\mathcal F_0=\{\varnothing,\Omega\}$; the printed $\{\varnothing,\mathcal F\}$ does not define the intended trivial sigma-algebra. With the [simple symmetric random walk](../../../../../../simple-symmetric-random-walk.md) convention from part (a), $M_n$ is adapted and integrable because $|S_n|\leq n$. Independence gives

$$
\mathbb E(X_{n+1}\mid\mathcal F_n)=0,\qquad
\mathbb E(X_{n+1}^2\mid\mathcal F_n)=1.
$$

By linearity, the pull-out property for the $\mathcal F_n$-measurable $S_n$, and preservation of measurable variables by [conditional expectation](../../../../../../conditional-expectation.md),

$$
\begin{aligned}
\mathbb E(M_{n+1}\mid\mathcal F_n)
&=S_n^2+2S_n\mathbb E(X_{n+1}\mid\mathcal F_n)
+\mathbb E(X_{n+1}^2\mid\mathcal F_n)-n-1\\
&=S_n^2-n=M_n.
\end{aligned}
$$

This proves the [square-minus-time martingale of a simple symmetric random walk](../../../../../../square-minus-time-martingale-of-a-simple-symmetric-random-walk.md).

## ↑ Ancestors (14)

1. [I](../i.md)
2. [B](../../b.md)
3. [3](../../../3.md)
4. [A](../../../../a.md)
5. [2009](../../../../../2009-split.md)
6. [Past exam of the martingales and financial mathematics course of the University of Oxford](../../../../../split.md)
7. [Martingales and financial mathematics course of the University of Oxford](../../../../../../martingales-and-financial-mathematics-course-of-the-university-of-oxford.md)
8. [Year 3 of the mathematics course of the University of Oxford](../../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
9. [Mathematics course of the University of Oxford](../../../../../../mathematics-course-of-the-university-of-oxford.md)
10. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
11. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
12. [University of Oxford](../../../../../../university-of-oxford-split.md)
13. [List of universities](../../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../../split.md)
