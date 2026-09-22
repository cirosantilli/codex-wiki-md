# Paper 339

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2022/paper_339.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2022/paper_339.pdf)

**Table of contents**

- [1](#1)
  - [a](#1/a)
    - [Solution](#1/a/solution)
  - [b](#1/b)
    - [i](#1/b/i)
      - [Solution](#1/b/i/solution)
    - [ii](#1/b/ii)
      - [Solution](#1/b/ii/solution)
    - [iii](#1/b/iii)
      - [Solution](#1/b/iii/solution)
  - [c](#1/c)
    - [i](#1/c/i)
      - [Solution](#1/c/i/solution)
    - [ii](#1/c/ii)
      - [Solution](#1/c/ii/solution)
    - [iii](#1/c/iii)
      - [Solution](#1/c/iii/solution)
- [2](#2)
  - [a](#2/a)
    - [Solution](#2/a/solution)
  - [b](#2/b)
    - [Solution](#2/b/solution)
  - [c](#2/c)
    - [i](#2/c/i)
      - [Solution](#2/c/i/solution)
    - [ii](#2/c/ii)
      - [Solution](#2/c/ii/solution)
    - [iii](#2/c/iii)
      - [Solution](#2/c/iii/solution)
    - [iv](#2/c/iv)
      - [Solution](#2/c/iv/solution)
- [3](#3)
  - [a](#3/a)
    - [Solution](#3/a/solution)
  - [b](#3/b)
    - [Solution](#3/b/solution)
  - [c](#3/c)
    - [i](#3/c/i)
      - [Solution](#3/c/i/solution)
    - [ii](#3/c/ii)
      - [Solution](#3/c/ii/solution)
    - [iii](#3/c/iii)
      - [Solution](#3/c/iii/solution)
    - [iv](#3/c/iv)
      - [Solution](#3/c/iv/solution)
  - [d](#3/d)
    - [Solution](#3/d/solution)

## 1

↑ **Parent:** [Paper 339](paper-339.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

A vector $g$ is a [subgradient](../../../real-analysis.md#subgradient) of the [convex function](../../../real-analysis.md#convex-function) $f$ at $x$ when

$$
f(y)\geq f(x)+g^T(y-x)
$$

for every $y$. The set of all such vectors is the [subdifferential](../../../convex-optimization.md#subdifferential) $\partial f(x)$. The [proximal operator](../../../convex-optimization.md#proximal-operator) satisfies

$$
\boxed{u=\operatorname{prox}_f(x)
\quad\Longleftrightarrow\quad x-u\in\partial f(u).}
$$

More generally, $u=\operatorname{prox}_{tf}(x)$ exactly when $(x-u)/t\in\partial f(u)$.

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/i">i</h4>

↑ **Parent:** [B](#1/b)

<h5 id="1/b/i/solution">Solution</h5>

↑ **Parent:** [I](#1/b/i)

The proximal optimality condition gives

$$
\frac{x_k-x_{k+1}}t\in\partial f(x_{k+1}).
$$

The [subgradient inequality](../../../real-analysis.md#subgradient-inequality) therefore yields, for every $u$,

$$
\boxed{f(u)\geq f(x_{k+1})+\frac1t(x_k-x_{k+1})^T(u-x_{k+1}).}
$$

<h4 id="1/b/ii">ii</h4>

↑ **Parent:** [B](#1/b)

<h5 id="1/b/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#1/b/ii)

Rearranging part i and using the polarization identity gives

$$
\begin{aligned}
t[f(x_{k+1})-f(u)]
&\leq(x_k-x_{k+1})^T(x_{k+1}-u)\\
&=\frac12\left(\|u-x_k\|^2-\|u-x_{k+1}\|^2-\|x_k-x_{k+1}\|^2\right).
\end{aligned}
$$

Dropping the final nonpositive term proves

$$
\boxed{t[f(x_{k+1})-f(u)]
\leq\frac12(\|u-x_k\|^2-\|u-x_{k+1}\|^2).}
$$

<h4 id="1/b/iii">iii</h4>

↑ **Parent:** [B](#1/b)

<h5 id="1/b/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#1/b/iii)

The defining minimization, compared with the candidate $x_k$, shows that $f(x_{k+1})\leq f(x_k)$. Put $u=x^*$ in part ii and sum from $j=0$ to $k-1$. The squared distances telescope, while monotonicity gives

$$
kt[f(x_k)-f^*]
\leq t\sum_{j=0}^{k-1}[f(x_{j+1})-f^*]
\leq\frac12\|x_0-x^*\|^2.
$$

Hence

$$
\boxed{f(x_k)-f^*\leq\frac{\|x_0-x^*\|^2}{2kt}.}
$$

<h3 id="1/c">c</h3>

↑ **Parent:** [1](#1)

<h4 id="1/c/i">i</h4>

↑ **Parent:** [C](#1/c)

<h5 id="1/c/i/solution">Solution</h5>

↑ **Parent:** [I](#1/c/i)

The [Fenchel conjugate](../../../convex-optimization.md#convex-conjugate) of $h$ is

$$
\boxed{h^*(y)=\sup_x\{y^Tx-h(x)\}.}
$$

<h4 id="1/c/ii">ii</h4>

↑ **Parent:** [C](#1/c)

<h5 id="1/c/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#1/c/ii)

Set $g(u)=tf(u)+\|u\|^2/2$. Expanding the square gives

$$
\boxed{M_tf(x)=\frac1{2t}\|x\|^2-\frac1t g^*(x).}
$$

The function $g$ is one-[strongly convex](../../../real-analysis.md#strongly-convex-function), so its [Fenchel conjugate](../../../convex-optimization.md#convex-conjugate) is differentiable with one-Lipschitz gradient. The displayed identity therefore proves that the [Moreau envelope](../../../convex-optimization.md#moreau-envelope) $M_tf$ is differentiable even when $f$ is nonsmooth.

<h4 id="1/c/iii">iii</h4>

↑ **Parent:** [C](#1/c)

<h5 id="1/c/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#1/c/iii)

The maximizer defining $g^*(x)$ is $\operatorname{prox}_{tf}(x)$, so

$$
\boxed{\nabla M_tf(x)=\frac1t[x-\operatorname{prox}_{tf}(x)].}
$$

Consequently

$$
x_{k+1}=\operatorname{prox}_{tf}(x_k)
=x_k-t\nabla M_tf(x_k).
$$

**Thus the [proximal point algorithm](../../../convex-optimization.md#proximal-point-algorithm) for $f$ is ordinary [gradient descent](../../../numerical-analysis.md#gradient-descent) with step $t$ on its smooth Moreau envelope.**

## 2

↑ **Parent:** [Paper 339](paper-339.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

For the equality constraint, the [Lagrangian](../../../calculus-of-variations.md#lagrangian) and dual function are

$$
L(x,z)=f(x)+z^T(Ax-b),
\qquad q(z)=\inf_xL(x,z),
$$

and the [Lagrangian dual problem](../../../mathematical-optimization.md#lagrangian-dual-problem) is $\sup_{z\in\mathbb R^m}q(z)$. [Weak duality](../../../mathematical-optimization.md#weak-duality) says $q(z)\leq p^*$ for every $z$. [Strong duality](../../../mathematical-optimization.md#strong-duality) means the dual supremum equals the primal infimum, usually with a dual maximizer. A sufficient convex constraint qualification is that $f$ be proper, closed and convex and that some $x\in\operatorname{ri}(\operatorname{dom}f)$ satisfy $Ax=b$.

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/solution">Solution</h4>

↑ **Parent:** [B](#2/b)

Use multiplier $-z$ for $Ax-b-s=0$. The Lagrangian is

$$
L(x,s,z)=\frac12x^TQx+I_{\mathbb R_+^m}(s)-z^T(Ax-b-s).
$$

The infimum over $s$ is finite exactly when $z\geq0$. The infimum over $x$ occurs at $x=Q^{-1}A^Tz$, and hence

$$
\boxed{h(z)=b^Tz-\frac12z^TAQ^{-1}A^Tz.}
$$

The dual is $\max_{z\geq0}h(z)$. Since the primal objective is coercive, the explicit [Slater condition](../../../mathematical-optimization.md#slater-s-condition)

$$
\boxed{\text{there exists }\bar x\text{ such that }A\bar x>b}
$$

is sufficient for feasibility, attainment, and equality of primal and dual values.

<h3 id="2/c">c</h3>

↑ **Parent:** [2](#2)

<h4 id="2/c/i">i</h4>

↑ **Parent:** [C](#2/c)

<h5 id="2/c/i/solution">Solution</h5>

↑ **Parent:** [I](#2/c/i)

Let $M=AQ^{-1}A^T$. Since $\nabla h(z)=b-Mz$, [projected gradient ascent](../../../convex-optimization.md#projected-gradient-descent) on the nonnegative orthant is

$$
\boxed{z_{k+1}=\bigl[z_k+\eta(b-Mz_k)\bigr]_+,}
$$

where the positive part is componentwise and one may take $0<\eta\leq1/L$.

<h4 id="2/c/ii">ii</h4>

↑ **Parent:** [C](#2/c)

<h5 id="2/c/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#2/c/ii)

The Hessian of $-h$ is $M=AQ^{-1}A^T$. Thus $-h$ is strongly convex exactly when $A$ has [full row rank](../../../vector-space.md#full-row-rank). In that case one may use

$$
\boxed{\mu\geq\frac{\lambda_{\min}(AA^T)}{\lambda_{\max}(Q)}.}
$$

In all cases, the gradient has Lipschitz constant bounded by

$$
\boxed{L=\lambda_{\max}(M)
\leq\frac{\|A\|_2^2}{\lambda_{\min}(Q)}.}
$$

<h4 id="2/c/iii">iii</h4>

↑ **Parent:** [C](#2/c)

<h5 id="2/c/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#2/c/iii)

When $A$ has full row rank, projected gradient ascent with step $1/L$ has linear convergence and requires

$$
\boxed{k=O\left(\frac L\mu\log\frac1\epsilon\right)}
$$

iterations, up to the initial-error constant. The accelerated projected method of [Nesterov](../../../convex-optimization.md#nesterov-accelerated-gradient-method) requires

$$
\boxed{k=O\left(\sqrt{\frac L\mu}\log\frac1\epsilon\right).}
$$

Without full row rank, the general smooth-convex bounds are $O(LR^2/\epsilon)$ and $O(\sqrt{LR^2/\epsilon})$, respectively, when a dual optimum lies within distance $R$ of the initial point.

<h4 id="2/c/iv">iv</h4>

↑ **Parent:** [C](#2/c)

<h5 id="2/c/iv/solution">Solution</h5>

↑ **Parent:** [Iv](#2/c/iv)

For $C=\{x:Ax\geq b\}$, primal [projected gradient descent](../../../convex-optimization.md#projected-gradient-descent) is

$$
\boxed{x_{k+1}=P_C[(I-\eta Q)x_k],
\qquad 0<\eta\leq\lambda_{\max}(Q)^{-1}.}
$$

Projection onto $C$ is itself a constrained quadratic program. The dual method only projects componentwise onto $\mathbb R_+^m$ and uses the fixed matrix $AQ^{-1}A^T$, so its iterations can be substantially cheaper, especially when $Q^{-1}$ can be prefactored and the number of constraints is moderate.

## 3

↑ **Parent:** [Paper 339](paper-339.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

A map $T$ is a [firmly nonexpansive mapping](../../../convex-optimization.md#firmly-nonexpansive-mapping) when

$$
\|Tx-Ty\|^2\leq(Tx-Ty)^T(x-y)
$$

for all $x,y$. Put $p=\operatorname{prox}_f(x)$ and $q=\operatorname{prox}_f(y)$. Then $x-p\in\partial f(p)$ and $y-q\in\partial f(q)$. Monotonicity of the [subdifferential](../../../convex-optimization.md#subdifferential) gives

$$
[(x-p)-(y-q)]^T(p-q)\geq0,
$$

which rearranges to

$$
\boxed{\|p-q\|^2\leq(p-q)^T(x-y).}
$$

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

Write $P_f=\operatorname{prox}_f$ and $P_h=\operatorname{prox}_h$. Since $w_k=x_k+z_{k-1}$,

$$
y_k=P_h(w_k),
\qquad z_k=w_k-P_h(w_k),
$$

and therefore

$$
\boxed{w_{k+1}=T(w_k),
\qquad T=I-P_h+P_f(2P_h-I).}
$$

With reflected proximal maps $R_f=2P_f-I$ and $R_h=2P_h-I$,

$$
T=\frac12(I+R_fR_h).
$$

Firm nonexpansiveness of each proximal map is equivalent to nonexpansiveness of its reflection. Thus $R_fR_h$ is nonexpansive, and its average with the identity is firmly nonexpansive. This is the [Douglas–Rachford method](../../../convex-optimization.md#douglas-rachford-method).

<h3 id="3/c">c</h3>

↑ **Parent:** [3](#3)

<h4 id="3/c/i">i</h4>

↑ **Parent:** [C](#3/c)

<h5 id="3/c/i/solution">Solution</h5>

↑ **Parent:** [I](#3/c/i)

Take $f=I_C$ and $h=I_D$. Their proximal maps are the [projections](../../../mathematical-optimization.md#euclidean-projection-onto-a-convex-set) $P_C,P_D$, so

$$
w_{k+1}=w_k-P_Dw_k+P_C(2P_Dw_k-w_k).
$$

The Douglas--Rachford shadow sequence $P_Dw_k$ converges in finite dimensions to a point of $C\cap D$ when the intersection is nonempty.

<h4 id="3/c/ii">ii</h4>

↑ **Parent:** [C](#3/c)

<h5 id="3/c/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#3/c/ii)

The function

$$
d_D(x)=\min_{y\in D}\frac12\|y-x\|^2
$$

is the [Moreau envelope](../../../convex-optimization.md#moreau-envelope) of the convex indicator $I_D$, and is therefore convex. It is nonnegative and vanishes exactly on $D$. Since $C\cap D\ne\varnothing$, the minimum of $d_D$ over $C$ is zero, and every minimizer belongs to both $C$ and $D$.

<h4 id="3/c/iii">iii</h4>

↑ **Parent:** [C](#3/c)

<h5 id="3/c/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#3/c/iii)

The [squared distance to a convex set](../../../convex-optimization.md#squared-distance-to-a-convex-set) satisfies

$$
\boxed{\nabla d_D(x)=x-P_Dx.}
$$

The map $I-P_D$ is firmly nonexpansive because $P_D$ is firmly nonexpansive, so

$$
\|\nabla d_D(x)-\nabla d_D(y)\|\leq\|x-y\|.
$$

**Thus $d_D$ is one-smooth in the Euclidean norm.**

<h4 id="3/c/iv">iv</h4>

↑ **Parent:** [C](#3/c)

<h5 id="3/c/iv/solution">Solution</h5>

↑ **Parent:** [Iv](#3/c/iv)

Projected gradient descent with unit step is

$$
\boxed{x_{k+1}=P_C[x_k-(x_k-P_Dx_k)]=P_C(P_Dx_k).}
$$

**Thus this instance reduces to alternating Euclidean projections.**

<h3 id="3/d">d</h3>

↑ **Parent:** [3](#3)

<h4 id="3/d/solution">Solution</h4>

↑ **Parent:** [D](#3/d)

Work in the product space $(\mathbb R^n)^\ell$ and define

$$
\mathcal C=C_1\times\cdots\times C_\ell,
\qquad
\mathcal D=\{(x,\ldots,x):x\in\mathbb R^n\}.
$$

Then $\mathcal C\cap\mathcal D$ is nonempty exactly when $\bigcap_jC_j$ is nonempty. For $X=(x_1,\ldots,x_\ell)$,

$$
\boxed{P_{\mathcal C}X=(P_{C_1}x_1,\ldots,P_{C_\ell}x_\ell),}
$$

while, with $\bar x=\ell^{-1}\sum_jx_j$,

$$
\boxed{P_{\mathcal D}X=(\bar x,\ldots,\bar x).}
$$

This is the [product-space reformulation of convex feasibility](../../../convex-optimization.md#product-space-reformulation-of-convex-feasibility).

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2022](../../2022.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
