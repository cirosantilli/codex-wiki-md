# Paper 339

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2023/Paper_339.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2023/Paper_339.pdf)

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
  - [e](#1/e)
    - [Solution](#1/e/solution)
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

Each map $x\mapsto\langle a_i,x\rangle+b_i$ is an [affine function](../../../vector-space.md#affine-function). For $0\leq t\leq1$, the [pointwise maximum of convex functions](../../../real-analysis.md#pointwise-maximum-of-convex-functions) satisfies

$$
\begin{aligned}
f(tx+(1-t)y)
&=\max_i\{t(\langle a_i,x\rangle+b_i)+(1-t)(\langle a_i,y\rangle+b_i)\}\\
&\leq t f(x)+(1-t)f(y),
\end{aligned}
$$

so $f$ is [convex](../../../real-analysis.md#convex-function).

A vector $g$ is a [subgradient](../../../real-analysis.md#subgradient) of a [convex function](../../../real-analysis.md#convex-function) $f$ at $x$ when

$$
f(y)\geq f(x)+\langle g,y-x\rangle
$$

for every $y$. Choose any active index $j\in I(x):=\{i:f(x)=\langle a_i,x\rangle+b_i\}$. Then

$$
f(y)\geq\langle a_j,y\rangle+b_j
=f(x)+\langle a_j,y-x\rangle,
$$

and hence $\boxed{a_j\in\partial f(x)}$. More generally, every [convex combination](../../../mathematical-optimization.md#convex-combination) of the active vectors is a subgradient, and in fact

$$
\boxed{\partial f(x)=\operatorname{conv}\{a_i:i\in I(x)\}.}
$$

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

Put $G=\max_i\|a_i\|_2$. By the [Cauchy-Schwarz inequality](../../../probability-and-statistics.md#cauchy-schwarz-inequality),

$$
\begin{aligned}
f(x)-f(y)
&\leq\max_i\langle a_i,x-y\rangle\\
&\leq G\|x-y\|_2.
\end{aligned}
$$

Interchanging $x$ and $y$ proves the [Lipschitz bound](../../../real-analysis.md#lipschitz-bound)

$$
\boxed{|f(x)-f(y)|\leq G\|x-y\|_2.}
$$

The [subgradient method](../../../convex-optimization.md#subgradient-method) chooses $g_k\in\partial f(x_k)$ and a [step size](../../../convex-optimization.md#step-size) $t_k>0$, then sets

$$
\boxed{x_{k+1}=x_k-t_kg_k.}
$$

Assume, as the question's use of $\min f$ requires, that a minimizer $x_*$ exists, and write $R=\|x_0-x_*\|_2$. Since every subgradient here has [Euclidean norm](../../../functional-analysis.md#euclidean-norm) at most $G$, the standard best-iterate estimate is

$$
\min_{0\leq j<k}(f(x_j)-f(x_*))
\leq\frac{R^2+G^2\sum_{j<k}t_j^2}{2\sum_{j<k}t_j}.
$$

Taking a suitable constant step when the target accuracy is known, or a standard diminishing sequence, gives error at most $\epsilon$ in

$$
\boxed{O(R^2G^2\epsilon^{-2})=O(\epsilon^{-2})}
$$

iterations, so the requested exponent is $p=2$.

<h3 id="1/c">c</h3>

↑ **Parent:** [1](#1)

<h4 id="1/c/solution">Solution</h4>

↑ **Parent:** [C](#1/c)

Write $z_i(x)=\langle a_i,x\rangle+b_i$. The [log-sum-exp function](../../../convex-optimization.md#log-sum-exp-function) is convex and composition with the [affine functions](../../../vector-space.md#affine-function) $z_i$ preserves convexity, so $f_\beta$ is [convex](../../../real-analysis.md#convex-function). Directly, its [Hessian matrix](../../../calculus.md#hessian-matrix) will also be shown [positive semidefinite](../../../linear-algebra.md#positive-semidefinite-matrix) in part d.

Let $M=f(x)=\max_i z_i(x)$. Factoring $e^{\beta M}$ out of the sum gives

$$
f_\beta(x)
=M+\frac1\beta\log\sum_i e^{\beta(z_i(x)-M)}.
$$

At least one term in the sum is $1$, while every term is at most $1$. Therefore

$$
1\leq\sum_i e^{\beta(z_i-M)}\leq m,
$$

and hence

$$
\boxed{f(x)\leq f_\beta(x)\leq f(x)+\frac{\log m}{\beta}.}
$$

**Thus $f_\beta$ is a uniform [smooth maximum](../../../convex-optimization.md#smooth-maximum) of the affine pieces of $f$.**

<h3 id="1/d">d</h3>

↑ **Parent:** [1](#1)

<h4 id="1/d/solution">Solution</h4>

↑ **Parent:** [D](#1/d)

Define the [softmax weights](../../../statistical-learning.md#softmax-function)

$$
p_i(x)=\frac{e^{\beta z_i(x)}}{\sum_j e^{\beta z_j(x)}}.
$$

They obey $p_i\geq0$ and $\sum_i p_i=1$. The [gradient](../../../calculus.md#gradient) is their weighted mean,

$$
\boxed{\nabla f_\beta(x)=\sum_i p_i(x)a_i.}
$$

Differentiating once more gives the covariance-form [Hessian matrix](../../../calculus.md#hessian-matrix)

$$
\nabla^2f_\beta(x)
=\beta\left(\sum_i p_i a_i a_i^T-\bar a\bar a^T\right),
\qquad \bar a=\sum_i p_i a_i.
$$

For every unit [vector](../../../vector-space.md#vector) $u$,

$$
u^T\nabla^2f_\beta(x)u
=\beta\operatorname{Var}_{i\sim p}(u^Ta_i)
\leq\beta\sum_i p_i(u^Ta_i)^2
\leq\beta G^2,
$$

where $G=\max_i\|a_i\|_2$. The Hessian is a [covariance matrix](../../../variance.md#covariance-matrix), so it is [positive semidefinite](../../../linear-algebra.md#positive-semidefinite-matrix); the displayed upper bound also gives $\nabla^2f_\beta\preceq\beta G^2I$ in the [Loewner order](../../../linear-algebra.md#loewner-order). Consequently $f_\beta$ has a [Lipschitz gradient](../../../numerical-analysis.md#lipschitz-gradient) with

$$
\boxed{L=\beta G^2.}
$$

<h3 id="1/e">e</h3>

↑ **Parent:** [1](#1)

<h4 id="1/e/solution">Solution</h4>

↑ **Parent:** [E](#1/e)

Choose

$$
\beta=\frac{2\log m}{\epsilon},
$$

so the [smooth maximum](../../../convex-optimization.md#smooth-maximum) error is at most $\epsilon/2$ and the [Lipschitz gradient](../../../numerical-analysis.md#lipschitz-gradient) constant is

$$
L=\frac{2G^2\log m}{\epsilon}.
$$

Suppose a minimizer of $f_\beta$ lies within distance $R$ of the starting point. The [Nesterov accelerated gradient method](../../../convex-optimization.md#nesterov-accelerated-gradient-method) can find $x$ such that

$$
f_\beta(x)-\min f_\beta\leq\frac\epsilon2
$$

in

$$
O\left(\sqrt{\frac{LR^2}{\epsilon}}\right)
=O\left(\frac{GR\sqrt{\log m}}{\epsilon}\right)
=O(\epsilon^{-1})
$$

iterations. If $x_*$ minimizes $f$, then the smoothing inequalities imply

$$
\begin{aligned}
f(x)-f(x_*)
&\leq f_\beta(x)-\min f_\beta
+\min f_\beta-f(x_*)\\
&\leq\frac\epsilon2+\frac{\log m}{\beta}
=\epsilon.
\end{aligned}
$$

This improves the nonsmooth [subgradient method](../../../convex-optimization.md#subgradient-method) dependence from $O(\epsilon^{-2})$ to $O(\epsilon^{-1})$.

## 2

↑ **Parent:** [Paper 339](paper-339.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

The first-order [subgradient inequality](../../../real-analysis.md#subgradient-inequality) for a differentiable [convex function](../../../real-analysis.md#convex-function) gives

$$
f(v)\geq f(w)+\langle\nabla f(w),v-w\rangle
$$

and, after interchanging $v$ and $w$,

$$
f(w)\geq f(v)+\langle\nabla f(v),w-v\rangle.
$$

Adding and rearranging yields

$$
\boxed{\langle\nabla f(v)-\nabla f(w),v-w\rangle\geq0.}
$$

**Thus the [gradient](../../../calculus.md#gradient) $F=\nabla f$ is a [monotone operator](../../../convex-optimization.md#monotone-operator).**

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/solution">Solution</h4>

↑ **Parent:** [B](#2/b)

If $T(w)=w$, the defining equation becomes $M(w)+F(w)=M(w)$, so $\boxed{F(w)=0}$.

A map is [firmly nonexpansive](../../../convex-optimization.md#firmly-nonexpansive-mapping) in the $M$-inner product when

$$
\|T(v)-T(w)\|_M^2
\leq\langle T(v)-T(w),v-w\rangle_M.
$$

Put $p=T(v)$ and $q=T(w)$. The two implicit equations give

$$
F(p)=M(v-p),\qquad F(q)=M(w-q).
$$

Because $F$ is a [monotone operator](../../../convex-optimization.md#monotone-operator),

$$
0\leq\langle F(p)-F(q),p-q\rangle
=\langle(v-w)-(p-q),p-q\rangle_M.
$$

Therefore

$$
\boxed{
\|p-q\|_M^2
\leq\langle p-q,v-w\rangle_M,}
$$

which is precisely firm nonexpansiveness. In particular, the [preconditioned proximal point algorithm](../../../convex-optimization.md#preconditioned-proximal-point-algorithm) map $T=(M+F)^{-1}M$ is [nonexpansive](../../../convex-optimization.md#nonexpansive-mapping) in the norm induced by the [positive-definite matrix](../../../linear-algebra.md#positive-definite-matrix) $M$.

<h3 id="2/c">c</h3>

↑ **Parent:** [2](#2)

<h4 id="2/c/solution">Solution</h4>

↑ **Parent:** [C](#2/c)

Use the sign convention

$$
\mathcal L(x,z)=f(x)-z^T(Ax-b)
$$

for the [Lagrangian function in constrained optimization](../../../calculus-of-variations.md#lagrangian-function-in-constrained-optimization). The [Lagrangian dual problem](../../../mathematical-optimization.md#lagrangian-dual-problem) is

$$
\boxed{
\max_{z\in\mathbb R^m}q(z),
\qquad
q(z)=\inf_x\mathcal L(x,z)
=b^Tz-f^*(A^Tz),}
$$

where $f^*$ is the [convex conjugate](../../../convex-optimization.md#convex-conjugate). For this convex problem with affine equality constraints, the stationarity and feasibility parts of the [Karush-Kuhn-Tucker conditions](../../../mathematical-optimization.md#karush-kuhn-tucker-conditions) are

$$
\nabla f(x)-A^Tz=0,
\qquad Ax-b=0.
$$

They say exactly that the displayed operator satisfies

$$
\boxed{
F\binom{x}{z}
=\binom{\nabla f(x)-A^Tz}{Ax-b}=0.}
$$

Thus its zeros are precisely the [primal-dual optimal points](../../../convex-optimization.md#primal-dual-optimal-point), subject to the usual attainment assumptions.

For $u=(x,z)$ and $\widetilde u=(y,s)$, the [Euclidean inner product](../../../linear-algebra.md#inner-product) gives

$$
\begin{aligned}
\langle F(u)-F(\widetilde u),u-\widetilde u\rangle
={}&\langle\nabla f(x)-\nabla f(y),x-y\rangle\\
&-\langle A^T(z-s),x-y\rangle
+\langle A(x-y),z-s\rangle.
\end{aligned}
$$

The last two terms cancel by the defining property of the [matrix transpose](../../../vector-space.md#transpose), and the first is nonnegative by part a. Hence $F$ is a [monotone operator](../../../convex-optimization.md#monotone-operator).

<h3 id="2/d">d</h3>

↑ **Parent:** [2](#2)

<h4 id="2/d/solution">Solution</h4>

↑ **Parent:** [D](#2/d)

The assertion uses the positive parameters required for $M$ to be a preconditioner: assume $\alpha>0$ and $\beta>0$. For $x\in\mathbb R^n$ and $z\in\mathbb R^m$, complete the square:

$$
\begin{aligned}
\binom{x}{z}^{\!T}
M\binom{x}{z}
&=\alpha\|x\|_2^2+2\langle Ax,z\rangle+\beta\|z\|_2^2\\
&=\beta\left\|z+\frac{Ax}{\beta}\right\|_2^2
+x^T\left(\alpha I-\frac{A^TA}{\beta}\right)x.
\end{aligned}
$$

The [matrix 2-norm](../../../continuous-dual-space.md#matrix-2-norm) bound $\|Ax\|_2\leq\|A\|_2\|x\|_2$ shows that

$$
x^T\left(\alpha I-\frac{A^TA}{\beta}\right)x
\geq\left(\alpha-\frac{\|A\|_2^2}{\beta}\right)\|x\|_2^2>0
$$

for $x\ne0$ when $\alpha\beta>\|A\|_2^2$. If $x=0$ and $z\ne0$, the square contributes $\beta\|z\|_2^2>0$. Thus $\boxed{M\text{ is positive definite}}$. Equivalently, the [Schur complement](../../../linear-algebra.md#schur-complement) of the lower-right block is $\alpha I-A^TA/\beta\succ0$.

Taken literally without the positivity inherited from part b, the product condition alone is insufficient: $A=0$ and $\alpha=\beta=-1$ is a counterexample. Thus $\alpha,\beta>0$ is a necessary implicit hypothesis.

<h3 id="2/e">e</h3>

↑ **Parent:** [2](#2)

<h4 id="2/e/solution">Solution</h4>

↑ **Parent:** [E](#2/e)

Write $w_k=(x_k,z_k)$ and $w_{k+1}=(x_{k+1},z_{k+1})$. Expanding

$$
M w_{k+1}+F(w_{k+1})=Mw_k
$$

gives

$$
\begin{aligned}
\alpha x_{k+1}+A^Tz_{k+1}
+\nabla f(x_{k+1})-A^Tz_{k+1}
&=\alpha x_k+A^Tz_k,\\
Ax_{k+1}+\beta z_{k+1}
+Ax_{k+1}-b
&=Ax_k+\beta z_k.
\end{aligned}
$$

The off-diagonal terms in the first equation cancel. By the optimality condition for the [proximal operator](../../../convex-optimization.md#proximal-operator),

$$
\boxed{
x_{k+1}
=\operatorname{prox}_{\alpha^{-1}f}
\left(x_k+\alpha^{-1}A^Tz_k\right).}
$$

The second equation then becomes the explicit linear update

$$
\boxed{
z_{k+1}
=z_k+\beta^{-1}\bigl(Ax_k-2Ax_{k+1}+b\bigr).}
$$

**Thus each step of this [preconditioned proximal point algorithm](../../../convex-optimization.md#preconditioned-proximal-point-algorithm) uses only one evaluation of the [proximal operator](../../../convex-optimization.md#proximal-operator) of $\alpha^{-1}f$, together with applications of the [linear map](../../../vector-space.md#linear-map) $A$ and its [transpose](../../../vector-space.md#transpose) $A^T$.**

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2023](../../2023.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
