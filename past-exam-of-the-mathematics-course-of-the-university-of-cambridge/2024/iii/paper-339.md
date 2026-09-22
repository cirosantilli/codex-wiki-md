# Paper 339

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2024/Paper_339.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2024/Paper_339.pdf)

**Table of contents**

- [1](#1)
  - [a](#1/a)
    - [Solution](#1/a/solution)
  - [b](#1/b)
    - [Solution](#1/b/solution)
  - [c](#1/c)
    - [Solution](#1/c/solution)
  - [d](#1/d)
    - [Solution](#1/d/solution)
- [2](#2)
  - [a](#2/a)
    - [Solution](#2/a/solution)
  - [b](#2/b)
    - [Solution](#2/b/solution)
  - [c](#2/c)
    - [Solution](#2/c/solution)
  - [d](#2/d)
    - [Solution](#2/d/solution)
  - [e](#2/e)
    - [Solution](#2/e/solution)

## 1

↑ **Parent:** [Paper 339](paper-339.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

The [Euclidean projection onto a convex set](../../../mathematical-optimization.md#euclidean-projection-onto-a-convex-set) is nonexpansive, and $x^*=P_C(x^*)$ because the optimum is feasible. Therefore the [projected subgradient method](../../../convex-optimization.md#projected-subgradient-method) satisfies

$$
\begin{aligned}
\lVert x_{i+1}-x^*\rVert_2^2
&\leq\lVert x_i-tg_i-x^*\rVert_2^2\\
&=\lVert x_i-x^*\rVert_2^2
-2t\langle g_i,x_i-x^*\rangle+t^2\lVert g_i\rVert_2^2.
\end{aligned}
$$

The [subgradient inequality](../../../real-analysis.md#subgradient-inequality) gives $\langle g_i,x_i-x^*\rangle\geq f(x_i)-f^*$, while [Lipschitz continuity](../../../real-analysis.md#lipschitz-continuity) of the finite [convex function](../../../real-analysis.md#convex-function) gives $\lVert g_i\rVert_2\leq G$. Hence

$$
2t\bigl(f(x_i)-f^*\bigr)
\leq \lVert x_i-x^*\rVert_2^2-
\lVert x_{i+1}-x^*\rVert_2^2+t^2G^2.
$$

Summing this telescoping inequality for $0\leq i<k$, and then bounding the smallest term by the average, yields

$$
\min_{0\leq i<k}f(x_i)-f^*
\leq\frac{\lVert x_0-x^*\rVert_2^2}{2tk}
+\frac{tG^2}{2}.
$$

Writing $D=\lVert x_0-x^*\rVert_2$, the right-hand side is minimized by the constant [step size](../../../convex-optimization.md#step-size)

$$
t=\frac{D}{G\sqrt{k}}.
$$

Substitution gives

$$
\boxed{\min_{0\leq i<k}f(x_i)-f^*\leq\frac{GD}{\sqrt{k}}}.
$$

If $D=0$, the initial point is already optimal and the result is immediate.

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

Associate a nonnegative [Lagrange multiplier](../../../mathematical-optimization.md#lagrange-multiplier) $\lambda_i$ with each inequality. The [Lagrangian dual problem](../../../mathematical-optimization.md#lagrangian-dual-problem) begins with

$$
L(x,\lambda)=c^Tx+\lambda^T(Ax-b)
=(c+A^T\lambda)^Tx-b^T\lambda,
\qquad \lambda\geq0.
$$

Its infimum over $x\in\mathbb R^n$ is finite exactly when $A^T\lambda+c=0$, in which case it equals $-b^T\lambda$. The dual [linear program](../../../mathematical-optimization.md#linear-programming) is consequently

$$
\boxed{\max_{\lambda\in\mathbb R^m}
\{-b^T\lambda:A^T\lambda+c=0,\ \lambda\geq0\}}.
$$

For any primal-feasible $x$ and dual-feasible $\lambda$,

$$
-b^T\lambda
\leq-x^TA^T\lambda
=c^Tx,
$$

which proves [weak duality](../../../mathematical-optimization.md#weak-duality). [Strong duality](../../../mathematical-optimization.md#strong-duality) means equality of the two optimal values. The stated strict feasibility is the [Slater condition](../../../mathematical-optimization.md#slater-s-condition); together with finiteness of the primal optimum it gives strong duality and an attained dual optimum $\lambda^*$.

<h3 id="1/c">c</h3>

↑ **Parent:** [1](#1)

<h4 id="1/c/solution">Solution</h4>

↑ **Parent:** [C](#1/c)

Let $\lambda^*$ be an optimal dual multiplier and define the maximum violation

$$
v(x)=\max\{0,(Ax-b)_1,\ldots,(Ax-b)_m\}.
$$

Dual stationarity and [strong duality](../../../mathematical-optimization.md#strong-duality) imply, for every $x$,

$$
c^Tx+(\lambda^*)^T(Ax-b)
=-b^T\lambda^*=p^*.
$$

Since every component of $Ax-b$ is at most $v(x)$ and $\lambda^*\geq0$,

$$
(\lambda^*)^T(Ax-b)\leq
\lVert\lambda^*\rVert_1v(x).
$$

It follows that the [exact maximum-violation penalty](../../../mathematical-optimization.md#exact-maximum-violation-penalty) obeys

$$
c^Tx+Mv(x)
\geq p^*+\bigl(M-\lVert\lambda^*\rVert_1\bigr)v(x).
$$

Choose any $M>\lVert\lambda^*\rVert_1$. A primal optimum has $v(x)=0$ and penalized value $p^*$, whereas every infeasible point has $v(x)>0$ and penalized value strictly greater than $p^*$. Thus the penalized problem and the original [linear program](../../../mathematical-optimization.md#linear-programming) have exactly the same minimizers.

<h3 id="1/d">d</h3>

↑ **Parent:** [1](#1)

<h4 id="1/d/solution">Solution</h4>

↑ **Parent:** [D](#1/d)

Write $a_i^T$ for row $i$ of $A$, and define affine functions

$$
\ell_0(x)=c^Tx,
\qquad
\ell_i(x)=(c+Ma_i)^Tx-Mb_i
\quad(1\leq i\leq m).
$$

Then

$$
f(x)=\max_{0\leq i\leq m}\ell_i(x).
$$

The [pointwise maximum of convex functions](../../../real-analysis.md#pointwise-maximum-of-convex-functions) is convex, so $f$ is a [convex function](../../../real-analysis.md#convex-function). Moreover,

$$
|f(x)-f(y)|
\leq L\lVert x-y\rVert_2,
\qquad
L=\max\left\{\lVert c\rVert_2,
\max_i\lVert c+Ma_i\rVert_2\right\},
$$

so $f$ has [Lipschitz continuity](../../../real-analysis.md#lipschitz-continuity). The simpler bound $L\leq\lVert c\rVert_2+M\max_i\lVert a_i\rVert_2$ is also valid.

Let $I(x)=\{i:\ell_i(x)=f(x)\}$ be the active set. The [subdifferential](../../../convex-optimization.md#subdifferential) is

$$
\partial f(x)=
\operatorname{conv}\left(
\{c:0\in I(x)\}\cup
\{c+Ma_i:i\in I(x),\ i\geq1\}
\right),
$$

the [convex hull](../../../mathematical-optimization.md#convex-hull) of all active slopes. In particular, choosing any active index gives the [subgradient](../../../real-analysis.md#subgradient)

$$
g(x)=
\begin{cases}
c,&0\in I(x),\\
c+Ma_j,&j\in I(x),\ j\geq1.
\end{cases}
$$

At a tie, every convex combination of the tied slopes is also valid.

## 2

↑ **Parent:** [Paper 339](paper-339.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

The objective is [strictly convex](../../../real-analysis.md#strictly-convex-function), so the minimizer is unique. The [Slater condition](../../../mathematical-optimization.md#slater-s-condition) makes the [Karush-Kuhn-Tucker conditions](../../../mathematical-optimization.md#karush-kuhn-tucker-conditions) necessary and sufficient. Absorb the box constraints into the [Euclidean projection onto a convex set](../../../mathematical-optimization.md#euclidean-projection-onto-a-convex-set) and attach a scalar multiplier $\nu$ to $a^Tx=b$. Stationarity over the box is equivalent to

$$
x^*=P_{[0,1]^n}(y-\nu a),
$$

while primal feasibility requires $a^Tx^*=b$. Coordinatewise, these conditions are

$$
\boxed{x_i^*=\min\{1,\max\{0,y_i-\nu a_i\}\}},
\qquad
\boxed{\sum_{i=1}^na_i
\min\{1,\max\{0,y_i-\nu a_i\}\}=b}.
$$

They are also sufficient because they minimize the [Lagrangian](../../../calculus-of-variations.md#lagrangian) over the box and satisfy the equality constraint. Thus the [projection onto a box-constrained hyperplane](../../../mathematical-optimization.md#projection-onto-a-box-constrained-hyperplane) reduces to solving the displayed one-dimensional continuous, nonincreasing equation for $\nu$. The multiplier need not be unique on a flat interval, but the projected vector is unique.

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/solution">Solution</h4>

↑ **Parent:** [B](#2/b)

For a proper lower-semicontinuous [convex function](../../../real-analysis.md#convex-function) $f$, its [proximal operator](../../../convex-optimization.md#proximal-operator) is

$$
\operatorname{prox}_f(y)=
\arg\min_x\left\{f(x)+\frac12\lVert x-y\rVert_2^2\right\}.
$$

The squared norm is strongly convex, so the minimizer is unique. The [subdifferential sum rule](../../../convex-optimization.md#subdifferential-sum-rule) gives the necessary and sufficient condition

$$
x=\operatorname{prox}_f(y)
\quad\Longleftrightarrow\quad
0\in\partial f(x)+x-y
\quad\Longleftrightarrow\quad
y-x\in\partial f(x).
$$

More generally,

$$
x=\operatorname{prox}_{tf}(y)
\quad\Longleftrightarrow\quad
u:=\frac{y-x}{t}\in\partial f(x).
$$

The subgradient inversion rule for the [convex conjugate](../../../convex-optimization.md#convex-conjugate) says $u\in\partial f(x)$ exactly when $x\in\partial f^*(u)$. Hence

$$
\frac yt-u=\frac xt\in\frac1t\partial f^*(u)
=\partial(t^{-1}f^*)(u),
$$

which is precisely the proximal optimality condition

$$
u=\operatorname{prox}_{t^{-1}f^*}(y/t).
$$

Since $x=y-tu$, this proves the generalized [Moreau decomposition](../../../convex-optimization.md#moreau-decomposition)

$$
\boxed{\operatorname{prox}_{tf}(y)=
y-t\operatorname{prox}_{t^{-1}f^*}(y/t)}.
$$

<h3 id="2/c">c</h3>

↑ **Parent:** [2](#2)

<h4 id="2/c/solution">Solution</h4>

↑ **Parent:** [C](#2/c)

The function $\phi(x)=\max_{v\in C}\langle x,v\rangle$ is the [support function](../../../mathematical-optimization.md#support-function) $\sigma_C$. For a nonempty compact [convex set](../../../mathematical-optimization.md#convex-set),

$$
\sigma_C^*(v)=
\begin{cases}
0,&v\in C,\\
+\infty,&v\notin C,
\end{cases}
$$

so its [convex conjugate](../../../convex-optimization.md#convex-conjugate) is the [indicator function](../../../measure-theory.md#indicator-function) $\iota_C$. Applying the [Moreau decomposition](../../../convex-optimization.md#moreau-decomposition),

$$
\operatorname{prox}_{t\phi}(y)
=y-t\operatorname{prox}_{t^{-1}\iota_C}(y/t).
$$

Multiplication of an [indicator function](../../../measure-theory.md#indicator-function) by a positive scalar does not change it, and its [proximal operator](../../../convex-optimization.md#proximal-operator) is the [Euclidean projection onto a convex set](../../../mathematical-optimization.md#euclidean-projection-onto-a-convex-set). Therefore

$$
\boxed{\operatorname{prox}_{t\phi}(y)=y-tP_C(y/t)}.
$$

<h3 id="2/d">d</h3>

↑ **Parent:** [2](#2)

<h4 id="2/d/solution">Solution</h4>

↑ **Parent:** [D](#2/d)

Take $a=\mathbf1$ and $b=k$, so

$$
C=\left\{v\in\mathbb R^n:
0\leq v_i\leq1,\ \sum_{i=1}^nv_i=k\right\}
$$

is the [capped simplex](../../../mathematical-optimization.md#capped-simplex). A linear objective over this [convex polytope](../../../mathematical-optimization.md#convex-polytope) attains its maximum at a zero-one extreme point. Choosing the $k$ coordinates at which $x_i$ is largest gives

$$
\max_{v\in C}x^Tv=x_{[1]}+\cdots+x_{[k]}=h(x).
$$

Equivalently, an exchange of weight from a smaller component to a larger one never decreases the objective. Thus the [sum of the largest components](../../../mathematical-optimization.md#sum-of-the-largest-components) is the [support function](../../../mathematical-optimization.md#support-function) $\sigma_C$.

Part c now gives

$$
\operatorname{prox}_{th}(y)=y-tP_C(y/t).
$$

By the [projection onto a box-constrained hyperplane](../../../mathematical-optimization.md#projection-onto-a-box-constrained-hyperplane), $v=P_C(y/t)$ has

$$
v_i=\min\{1,\max\{0,y_i/t-\nu\}\},
\qquad
\sum_i v_i=k.
$$

**Consequently the proximal operator is evaluated by solving this one-dimensional equation for $\nu$, then substituting the resulting projection.**

<h3 id="2/e">e</h3>

↑ **Parent:** [2](#2)

<h4 id="2/e/solution">Solution</h4>

↑ **Parent:** [E](#2/e)

Set

$$
g(x)=\frac12\lVert Ax-b\rVert_2^2,
\qquad
\nabla g(x)=A^T(Ax-b).
$$

The gradient has [Lipschitz continuity](../../../real-analysis.md#lipschitz-continuity) with constant

$$
L=\lVert A^TA\rVert_2=\lVert A\rVert_2^2,
$$

where the norm is the [spectral norm](../../../continuous-dual-space.md#matrix-2-norm). The [proximal gradient method](../../../convex-optimization.md#proximal-gradient-method) is therefore

$$
z_r=x_r-\alpha A^T(Ax_r-b),
\qquad
x_{r+1}=\operatorname{prox}_{\alpha\lambda h}(z_r).
$$

For $\lambda>0$, part d makes the second step explicit:

$$
x_{r+1}=z_r-\alpha\lambda
P_C\left(\frac{z_r}{\alpha\lambda}\right),
$$

where $C$ is the [capped simplex](../../../mathematical-optimization.md#capped-simplex); when $\lambda=0$, this proximal step is the identity.

A standard fixed choice is $0<\alpha\leq1/L$; the wider interval $0<\alpha<2/L$ also gives convergence under the usual forward-backward conditions. For a general convex objective, the function-value error is $O(1/r)$. If $A$ has full column rank, the quadratic term is [strongly convex](../../../real-analysis.md#strongly-convex-function) and an appropriate fixed step gives a linear convergence rate.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2024](../../2024.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
