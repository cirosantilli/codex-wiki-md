<h1 id="2f/solution">Solution</h1>

↑ **Parent:** [2F](../2f.md)

A map $h:X\to X$ is a contraction if there is a constant $q<1$ such that

$$
d(hx,hy)\leq qd(x,y)
$$

for every $x,y\in X$.

The [contraction mapping theorem](../../../../../contraction-mapping-theorem.md) states that a contraction of a nonempty complete metric space has a unique fixed point, and that the iterates from every starting point converge to it. To prove this, choose $x_0\in X$ and put $x_{n+1}=h(x_n)$. Then

$$
d(x_{n+1},x_n)\leq q^nd(x_1,x_0),
$$

so, for $m>n$,

$$
d(x_m,x_n)\leq\frac{q^n}{1-q}d(x_1,x_0).
$$

Thus $(x_n)$ is Cauchy and converges, by completeness, to some $x_*$. A contraction is continuous, so

$$
h(x_*)=\lim_nh(x_n)=\lim_nx_{n+1}=x_*.
$$

If $y_*$ is another fixed point, then

$$
d(x_*,y_*)\leq qd(x_*,y_*),
$$

forcing $x_*=y_*$.

For the Newton map

$$
g(x)=x-\frac{f(x)}{f'(x)},
$$

one has $g(r)=r$ and

$$
g'(x)=\frac{f(x)f''(x)}{f'(x)^2},
\qquad
\boxed{g'(r)=0}.
$$

On the given neighbourhood,

$$
|g'(x)|\leq\frac{M|f(x)|}{\delta^2}.
$$

Since $f(r)=0$, choose a closed interval $U'$ centred at $r$ and contained in $U$ so small that $M|f(x)|/\delta^2\leq1/2$ there. Then

$$
|g(x)-r|\leq\frac12|x-r|,
$$

so $g(U')\subseteq U'$ and $g$ is a contraction on the complete interval $U'$. The [local contraction proof for Newton iteration](../../../../../local-contraction-proof-for-newton-iteration.md) therefore shows that $r$ is the unique fixed point of $g$ on $U'$.

## ↑ Ancestors (10)

1. [2F](../2f.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ib](../../split.md)
4. [2024](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
