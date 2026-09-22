<h1 id="12g/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For each $x\in X$, [density](../../../../../../dense-set.md) of $Y$ allows a sequence $y_n\in Y$ with $d(y_n,x)<1/n$. If $f_1,f_2$ are two continuous extensions, [continuity](../../../../../../continuous-function.md) gives

$$
f_1(x)=\lim_n g(y_n)=f_2(x).
$$

Thus **a continuous extension is unique if it exists**.

Now assume $g$ is [uniformly continuous](../../../../../../uniform-continuity.md). Each chosen $y_n\to x$ is a [Cauchy sequence](../../../../../../cauchy-sequence.md), so part (a), applied to $Y$, shows that $g(y_n)$ converges in $\mathbb R$. Define

$$
\boxed{f(x)=\lim_{n\to\infty}g(y_n).}
$$

This is independent of the choice: for another $z_n\to x$ in $Y$, $d(y_n,z_n)\to0$, and uniform continuity gives $g(y_n)-g(z_n)\to0$. At $x\in Y$, comparison with the constant sequence $x$ proves $f(x)=g(x)$.

To prove uniform continuity of the extension, choose $\delta>0$ so that $|g(y)-g(z)|<\varepsilon/2$ whenever $y,z\in Y$ and $d(y,z)<\delta$. If $d(x,x')<\delta/3$, choose sequences $y_n\to x$ and $z_n\to x'$ in $Y$. For large $n$, both approximation distances are less than $\delta/3$, so $d(y_n,z_n)<\delta$. Passing to the limit gives $|f(x)-f(x')|\leq\varepsilon/2<\varepsilon$. The same $\delta/3$ works for all $x,x'$. Therefore **the extension exists and is uniformly continuous**. No completeness of $X$ is needed; completeness of the target $\mathbb R$ is the relevant requirement.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [12G](../../12g.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ib](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
