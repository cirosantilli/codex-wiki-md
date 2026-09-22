<h1 id="3/a/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

The $2\pi$ [periodization of a Schwartz function](../../../../../periodization-of-a-schwartz-function.md) is

$$
\boxed{P\phi(x)=\sum_{k\in\mathbb Z}\phi(x+2\pi k).}
$$

For every nonnegative integer $j$, the [Schwartz seminorms](../../../../../schwartz-seminorm.md) give $|\phi^{(j)}(x+2\pi k)|\leq C_j(1+|k|)^{-2}$ uniformly for $x\in[0,2\pi]$. The [Weierstrass M-test](../../../../../weierstrass-m-test.md) gives absolute and [uniform convergence](../../../../../uniform-convergence.md) there of the defining [series](../../../../../series-mathematics.md) and all its differentiated [series](../../../../../series-mathematics.md). Termwise differentiation proves that $P\phi$ is a [smooth function](../../../../../smooth-function.md), with $(P\phi)^{(j)}=P(\phi^{(j)})$. Reindexing the absolutely convergent [series](../../../../../series-mathematics.md) proves $P\phi(x+2\pi)=P\phi(x)$, so it is a [periodic function](../../../../../periodic-function.md).

For an explicit [smooth periodic partition of unity](../../../../../smooth-periodic-partition-of-unity.md), choose the [bump function](../../../../../bump-function.md)

$$
\eta(x)=\begin{cases}
\exp\!\bigl(-1/(1-(x/(2\pi))^2)\bigr),&|x|<2\pi,\\
0,&|x|\geq2\pi.
\end{cases}
$$

It is a [test function](../../../../../test-function.md), positive on $[-\pi,\pi]$. The [smooth function](../../../../../smooth-function.md) $S(x)=P\eta(x)$ is $2\pi$ periodic and strictly positive, since every $x$ has a translate in $[-\pi,\pi]$. Set

$$
\boxed{\Psi(x)=\frac{\eta(x)}{S(x)}\in C_c^\infty(\mathbb R),\qquad
P\Psi(x)=\frac{\sum_k\eta(x+2\pi k)}{S(x)}=1.}
$$

Division preserves smoothness because $S>0$, and the [support](../../../../../support.md) remains contained in $[-2\pi,2\pi]$.

## ↑ Ancestors (13)

1. [I](../i.md)
2. [A](../../a.md)
3. [3](../../../3.md)
4. [2023](../../../../2023-split.md)
5. [Past exam of the fourier analysis course of the University of Oxford](../../../../split.md)
6. [Fourier analysis course of the University of Oxford](../../../../../fourier-analysis-course-of-the-university-of-oxford.md)
7. [Year 3 of the mathematics course of the University of Oxford](../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
