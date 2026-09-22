<h1 id="10f/solution">Solution</h1>

↑ **Parent:** [10F](../10f.md)

Let $C\subset\mathbb R$ be compact and let $M=\|f\|_\infty$. Since every $k_n$ is supported in $[-R,R]$, the function $f$ is [uniformly continuous](../../../../../uniform-continuity.md) on the compact set

$$
C_R=\{x-t:x\in C,\ |t|\leq R\}.
$$

Given $\varepsilon>0$, choose $\delta>0$ so that

$$
|f(x-t)-f(x)|<\frac{\varepsilon}{2}
$$

whenever $x\in C$ and $|t|<\delta$. Since $\int k_n=1$ and $k_n\geq0$,

$$
\begin{aligned}
|f_n(x)-f(x)|
&\leq\int_{\mathbb R}k_n(t)|f(x-t)-f(x)|\,dt\\
&\leq\frac{\varepsilon}{2}
+2M\int_{|t|\geq\delta}k_n(t)\,dt.
\end{aligned}
$$

Property 3 makes the final term smaller than $\varepsilon/2$ for all sufficiently large $n$, uniformly in $x\in C$. Hence $f_n\to f$ uniformly on every compact set. The sequence $(k_n)$ is an [approximate identity](../../../../../approximate-identity.md).

For the second part, extend $g$ to a continuous function $\widetilde g$ on $\mathbb R$ by setting it equal to zero outside $[0,1]$; continuity at the endpoints uses $g(0)=g(1)=0$. Define

$$
c_n=\int_{-1}^1(1-t^2)^n\,dt,
\qquad
k_n(t)=\frac{(1-t^2)^n}{c_n}\mathbf1_{[-1,1]}(t).
$$

These nonnegative kernels have integral one. For every $\delta>0$, their mass outside $[-\delta,\delta]$ tends to zero exponentially relative to the mass near zero, so they satisfy property 3.

For $x\in[0,1]$, the convolution is

$$
p_n(x)
=\int_{\mathbb R}k_n(t)\widetilde g(x-t)\,dt
=\frac1{c_n}\int_0^1
\bigl(1-(x-y)^2\bigr)^ng(y)\,dy.
$$

Because $|x-y|\leq1$ on the square $[0,1]^2$, no cutoff remains in this formula. Expanding the $n$th power shows that $p_n$ is a [polynomial](../../../../../polynomial-split.md) in $x$. The first part, applied to the compact interval $[0,1]$, gives

$$
\boxed{\|p_n-g\|_\infty\to0}.
$$

This proves the [Weierstrass approximation theorem](../../../../../weierstrass-approximation-theorem.md) for functions with the stated endpoint values.

## ↑ Ancestors (10)

1. [10F](../10f.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ib](../../split.md)
4. [2021](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
