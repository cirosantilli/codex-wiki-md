<h1 id="5/solution">Solution</h1>

↑ **Parent:** [5](../5.md)

An [exponentiable object](../../../../../exponentiable-object.md) $X$ in a category with finite products is one for which

$$
-\times X
$$

has a right adjoint $[X,-]$. The [terminal object](../../../../../terminal-object.md) is exponentiable because $-\times1\cong1_{\mathcal C}$. If $X$ and $Y$ are exponentiable, then

$$
-\times(X\times Y)\cong(-\times X)\times Y
$$

is a composite of two left adjoints and therefore has the composite right adjoint $[X,[Y,-]]$. Exponentiable objects are consequently closed under finite products.

In the [category of metric spaces and non-expansive maps](../../../../../category-of-metric-spaces-and-non-expansive-maps.md), the terminal object is the one-point space. The product of $X$ and $Y$ has underlying set $X\times Y$ and metric

$$
d((x,y),(x',y'))
=\max\{d_X(x,x'),d_Y(y,y')\}.
$$

This is the smallest metric making both projections [non-expansive](../../../../../non-expansive-map.md), and the product pairing of two non-expansive maps is non-expansive. If $X$ and $Y$ are bounded, so is this product. Hence both $\mathbf{Met}$ and the [category of bounded metric spaces and non-expansive maps](../../../../../category-of-bounded-metric-spaces-and-non-expansive-maps.md) $\mathbf{Met}_b$ have finite products.

For bounded $X,Y$, define the [metric exponential candidate](../../../../../metric-exponential-candidate.md)

$$
\bar d(f,g)=sup\{d_Y(fx,gy):d_X(x,y)<d_Y(fx,gy)\}.
$$

The supremum is finite because $Y$ is bounded. For every $x,y$ one has the useful evaluation inequality

$$
d_Y(fx,gy)
\leq\max\{\bar d(f,g),d_X(x,y)\}.
$$

Indeed, if the second term does not already dominate, the pair $(x,y)$ occurs in the defining supremum.

Assume $\bar d$ is a metric. The evaluation map

$$
\operatorname{ev}:[X,Y]\times X\longrightarrow Y,
\qquad(f,x)\longmapsto f(x)
$$

is non-expansive by this inequality. Postcomposition by a non-expansive $k:Y\to Y'$ is non-expansive on function spaces, because every pair contributing to $\bar d(kf,kg)$ also contributes a no-smaller bound to $\bar d(f,g)$. Thus $[X,-]$ is a functor.

If $h:Z\times X\to Y$ is non-expansive, each $h_z(x)=h(z,x)$ is non-expansive. Whenever

$$
d_X(x,y)<d_Y(h_z(x),h_{z'}(y)),
$$

non-expansiveness of $h$ forces the latter distance to be at most $d_Z(z,z')$. Hence $z\mapsto h_z$ is non-expansive into $[X,Y]$. Conversely, a non-expansive $Z\to[X,Y]$ followed by evaluation gives a non-expansive $Z\times X\to Y$. These inverse operations are natural, proving

$$
\mathbf{Met}_b(Z\times X,Y)
\cong\mathbf{Met}_b(Z,[X,Y]).
$$

It remains to obtain the triangle inequality from interpolation. Nonnegativity and symmetry of $\bar d$ are immediate. If $f\ne g$, taking $x=y$ where $f(x)\ne g(x)$ proves separation; and $\bar d(f,f)=0$ follows from non-expansiveness of $f$.

Let

$$
a=\bar d(f,g),\qquad b=\bar d(g,h).
$$

Fix a pair $x,y$ contributing $D=d_Y(fx,hy)$, so $t=d_X(x,y)<D$. Suppose for contradiction that $D>a+b$. If $t\leq a+b$, choose $r+s=t$ with $r\leq a$ and $s\leq b$. If $t>a+b$, choose $r+s=t$ with $r>a$ and $s>b$. Since $X$ is an [interpolating metric space](../../../../../interpolating-metric-space.md), there is $z$ with $d(x,z)=r$ and $d(z,y)=s$. Applying the evaluation inequality twice gives

$$
D\leq d_Y(fx,gz)+d_Y(gz,hy)
\leq\max\{a,r\}+\max\{b,s\}.
$$

In the first case the right side is at most $a+b$, and in the second it equals $r+s=t<D$. Both are contradictions. Therefore $D\leq a+b$ for every contributing pair, and taking the supremum gives

$$
\bar d(f,h)\leq\bar d(f,g)+\bar d(g,h).
$$

**Thus $\bar d$ is a metric whenever $X$ is interpolating, and the preceding adjunction proves every bounded interpolating space is exponentiable in $\mathbf{Met}_b$.**

## ↑ Ancestors (10)

1. [5](../5.md)
2. [Paper 119](../../paper-119-split.md)
3. [Iii](../../split.md)
4. [2023](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
