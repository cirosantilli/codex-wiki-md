<h1 id="11a/solution">Solution</h1>

↑ **Parent:** [11A](../11a.md)

For the [differentiability from continuous partial derivatives](../../../../../differentiability-from-continuous-partial-derivatives.md) argument, choose a small box around zero inside the given open set. For $h=(h_1,\ldots,h_p)$ in that box, telescope $f(h)-f(0)$ by changing one coordinate at a time. The one-dimensional [mean value theorem](../../../../../mean-value-theorem.md) on the $j$th coordinate segment gives

$$
f(h)-f(0)=\sum_{j=1}^p h_j f_j(\xi_j),
$$

where $\xi_j$ lies on that segment, and therefore $\|\xi_j\|_2\le\|h\|_2$. A zero-length segment contributes zero and needs no choice of intermediate point. Set $L(h)=\sum_j f_j(0)h_j$. For every $\varepsilon>0$, continuity of the finitely many [partial derivatives](../../../../../partial-derivative.md) at zero gives $|f_j(\xi_j)-f_j(0)|<\varepsilon/\sqrt p$ when $h$ is sufficiently small. Then the [Cauchy-Schwarz inequality](../../../../../cauchy-schwarz-inequality.md) gives

$$
|f(h)-f(0)-L(h)|\le\frac{\varepsilon}{\sqrt p}\sum_j|h_j|\le\varepsilon\|h\|_2.
$$

Thus $f$ is [Fréchet differentiable](../../../../../frechet-differentiability.md) at zero, with [derivative](../../../../../derivative.md) $L$. No continuity of the [partial derivatives](../../../../../partial-derivative.md) away from zero was used.

For the supplied one-dimensional function,

$$
g'(s)=\begin{cases}2s\sin(1/s)-\cos(1/s),&s\ne0,\\0,&s=0.\end{cases}
$$

The derivative at zero follows from $g(s)/s=s\sin(1/s)\to0$. For nonzero $s$ the derivative is continuous. At zero, the sequences $s_k=1/(2\pi k)$ and $t_k=1/((2k+1)\pi)$ give derivative values $-1$ and $1$. Since $f_x(x,y)=g'(x)$, **the partial derivative is continuous exactly where $x\ne0$**, irrespective of $y$.

Nevertheless **$f$ is differentiable at every point of the plane**. The one-dimensional function $g$ is differentiable at every real number. At a fixed $(x_0,y_0)$,

$$
g(x_0+h)-g(x_0)=g'(x_0)h+o(|h|),\qquad
g(y_0+k)-g(y_0)=g'(y_0)k+o(|k|).
$$

Their sum has remainder $o(\sqrt{h^2+k^2})$, which proves [Fréchet differentiability](../../../../../frechet-differentiability.md) with derivative $(h,k)\mapsto g'(x_0)h+g'(y_0)k$. In particular, at the origin $|f(h,k)|\le h^2+k^2$, an immediate remainder bound. Continuity of all partial derivatives is sufficient, not necessary, for differentiability.

## ↑ Ancestors (10)

1. [11A](../11a.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ib](../../split.md)
4. [2001](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
