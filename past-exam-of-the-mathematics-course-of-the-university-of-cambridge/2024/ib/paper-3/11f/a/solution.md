<h1 id="11f/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

A [function](../../../../../../function-split.md) $f:(X,d_X)\to(Y,d_Y)$ is uniformly continuous if for every $\varepsilon>0$ there is $\delta>0$ such that

$$
d_X(x,x')<\delta
\implies d_Y(f(x),f(x'))<\varepsilon
$$

for all $x,x'\in X$.

Suppose $f_n\to f$ uniformly and every $f_n$ is uniformly continuous. Given $\varepsilon>0$, choose $N$ such that

$$
d_Y(f_N(x),f(x))<\varepsilon/3
$$

for every $x$. Uniform continuity of $f_N$ supplies $\delta>0$ such that $d_X(x,x')<\delta$ implies

$$
d_Y(f_N(x),f_N(x'))<\varepsilon/3.
$$

The triangle inequality then gives $d_Y(f(x),f(x'))<\varepsilon$. Thus the [uniform limit theorem for uniformly continuous functions](../../../../../../uniform-limit-theorem-for-uniformly-continuous-functions.md) proves that $f$ is uniformly continuous.

[Pointwise convergence](../../../../../../pointwise-convergence.md) is insufficient. On $[0,1]$, the uniformly [continuous functions](../../../../../../continuous-function.md) $f_n(x)=x^n$ converge pointwise to

$$
f(x)=\begin{cases}0,&0\leq x<1,\\1,&x=1,\end{cases}
$$

which is discontinuous and therefore not uniformly continuous.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [11F](../../11f.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ib](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
