<h1 id="10e/solution">Solution</h1>

↑ **Parent:** [10E](../10e.md)

Take any sequence $(y_n)$ in $Y$. Surjectivity lets us choose $x_n\in X$ with $f(x_n)=y_n$. By [sequential compactness](../../../../../sequentially-compact-space.md) of $X$, some $x_{n_j}\to x\in X$. [Continuity](../../../../../continuous-function.md) gives $y_{n_j}=f(x_{n_j})\to f(x)\in Y$. Thus **$Y$ has the Bolzano–Weierstrass property**.

Now suppose $f$ is a bijection. To prove [continuity](../../../../../continuous-function.md) of its inverse, let $y_n\to y$ and put $x_n=f^{-1}(y_n)$, $x=f^{-1}(y)$. If $x_n\not\to x$, there are $\varepsilon>0$ and a subsequence with $d(x_{n_j},x)\geq\varepsilon$. [Sequential compactness](../../../../../sequentially-compact-space.md) supplies a further subsequence converging to $x'$. By [continuity](../../../../../continuous-function.md) of $f$, $f(x')=\lim y_{n_j}=y=f(x)$. Injectivity implies $x'=x$, contradicting the fixed lower distance bound. Hence $x_n\to x$. Sequential [continuity](../../../../../continuous-function.md) is equivalent to [continuity](../../../../../continuous-function.md) in [metric spaces](../../../../../metric-space.md), proving **$f^{-1}$ is continuous**.

Apply this to $g(t)=e^{it}$ on $[-\pi/2,\pi/2]$, mapping onto the closed right semicircle $S$. This interval is sequentially compact, and $g$ is a continuous bijection: two equal exponential values differ by an integral multiple of $2\pi$, impossible for distinct points of an interval of length $\pi$. Consequently $g^{-1}:S\to[-\pi/2,\pi/2]$ is continuous. For $\operatorname{Re}z>0$, the normalization $z\mapsto z/|z|$ is continuous and takes values in the open right semicircle. Therefore

$$
\boxed{\operatorname{Arg}(z)=g^{-1}(z/|z|)\in(-\pi/2,\pi/2)}
$$

is a continuous argument satisfying $z=|z|e^{i\operatorname{Arg}z}$. Equivalently it is $\arctan(\operatorname{Im}z/\operatorname{Re}z)$.

## ↑ Ancestors (10)

1. [10E](../10e.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ib](../../split.md)
4. [2002](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
