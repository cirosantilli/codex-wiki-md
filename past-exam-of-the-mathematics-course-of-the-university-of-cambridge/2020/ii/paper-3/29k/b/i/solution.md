<h1 id="29k/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Write $\Phi$ for the [standard normal cumulative distribution function](../../../../../../../standard-normal-distribution-function.md). Since $B_t\leq M_t$, for $y\geq0$ and $x>y$,

$$
\mathbb P(B_t\leq x,M_t\leq y)
=\mathbb P(M_t\leq y)
=2\Phi\!\left(\frac y{\sqrt t}\right)-1.
$$

For $x\leq y$, the [Brownian reflection principle](../../../../../../../reflection-principle-wiener-process.md) gives

$$
\begin{aligned}
\mathbb P(B_t\leq x,M_t\leq y)
&=\mathbb P(B_t\leq x)
-\mathbb P(B_t\leq x,M_t>y)\\
&=\Phi\!\left(\frac x{\sqrt t}\right)
-\mathbb P(B_t>2y-x)\\
&=\Phi\!\left(\frac x{\sqrt t}\right)
+\Phi\!\left(\frac{2y-x}{\sqrt t}\right)-1.
\end{aligned}
$$

The [joint distribution function](../../../../../../../joint-distribution-function.md) is therefore

$$
\boxed{
F_{B_t,M_t}(x,y)=
\begin{cases}
0,&y<0,\\
\Phi(x/\sqrt t)+\Phi((2y-x)/\sqrt t)-1,&y\geq0,\ x\leq y,\\
2\Phi(y/\sqrt t)-1,&y\geq0,\ x>y.
\end{cases}}
$$

## ↑ Ancestors (12)

1. [I](../i.md)
2. [B](../../b.md)
3. [29K](../../../29k.md)
4. [Paper 3](../../../../paper-3-split.md)
5. [Ii](../../../../split.md)
6. [2020](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
