# Paper 326

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2022/paper_326.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2022/paper_326.pdf)

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
    - [iv](#1/b/iv)
      - [Solution](#1/b/iv/solution)
  - [c](#1/c)
    - [i](#1/c/i)
      - [Solution](#1/c/i/solution)
    - [ii](#1/c/ii)
      - [Solution](#1/c/ii/solution)
    - [iii](#1/c/iii)
      - [Solution](#1/c/iii/solution)
    - [iv](#1/c/iv)
      - [Solution](#1/c/iv/solution)
    - [v](#1/c/v)
      - [Solution](#1/c/v/solution)
- [2](#2)
  - [a](#2/a)
    - [i](#2/a/i)
      - [Solution](#2/a/i/solution)
    - [ii](#2/a/ii)
      - [Solution](#2/a/ii/solution)
    - [iii](#2/a/iii)
      - [Solution](#2/a/iii/solution)
  - [b](#2/b)
    - [i](#2/b/i)
      - [Solution](#2/b/i/solution)
    - [ii](#2/b/ii)
      - [Solution](#2/b/ii/solution)
    - [iii](#2/b/iii)
      - [Solution](#2/b/iii/solution)
    - [iv](#2/b/iv)
      - [Solution](#2/b/iv/solution)
  - [c](#2/c)
    - [i](#2/c/i)
      - [Solution](#2/c/i/solution)
    - [ii](#2/c/ii)
      - [Solution](#2/c/ii/solution)

## 1

↑ **Parent:** [Paper 326](paper-326.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

For a bounded operator $A:X\to Y$ between [Hilbert spaces](../../../hilbert-space.md), the [Moore--Penrose inverse of a Hilbert-space operator](../../../linear-algebra.md#moore-penrose-inverse-of-a-hilbert-space-operator) is defined on

$$
\mathcal D(A^\dagger)=\mathcal R(A)\oplus\mathcal R(A)^\perp
$$

and has range $\mathcal R(A^\dagger)=\mathcal N(A)^\perp$. Its [Penrose equations](../../../linear-algebra.md#penrose-equations) are

$$
AA^\dagger A=A,
\qquad
A^\dagger AA^\dagger=A^\dagger,
\qquad
(AA^\dagger)^*=AA^\dagger,
\qquad
(A^\dagger A)^*=A^\dagger A.
$$

Equivalently, $A^\dagger A=P_{\mathcal N(A)^\perp}$ and $AA^\dagger$ is the restriction of $P_{\overline{\mathcal R(A)}}$ to $\mathcal D(A^\dagger)$.

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/i">i</h4>

↑ **Parent:** [B](#1/b)

<h5 id="1/b/i/solution">Solution</h5>

↑ **Parent:** [I](#1/b/i)

**The statement is true without an additional [rank](../../../vector-space.md#matrix-rank) assumption.** If $A=U\Sigma V^H$ is a [singular value decomposition](../../../linear-algebra.md#singular-value-decomposition), then

$$
\boxed{(A^\dagger)^H=(V\Sigma^\dagger U^H)^H
=U\Sigma^\dagger V^H=(A^H)^\dagger.}
$$

<h4 id="1/b/ii">ii</h4>

↑ **Parent:** [B](#1/b)

<h5 id="1/b/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#1/b/ii)

This statement is also always true. The same [singular value decomposition](../../../linear-algebra.md#singular-value-decomposition) gives

$$
\boxed{(A^HA)^\dagger
=V(\Sigma^H\Sigma)^\dagger V^H
=V(\Sigma^\dagger)^2V^H
=A^\dagger(A^\dagger)^H.}
$$

<h4 id="1/b/iii">iii</h4>

↑ **Parent:** [B](#1/b)

<h5 id="1/b/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#1/b/iii)

**True.** The matrix $A^\dagger A$ is the [orthogonal projection](../../../hilbert-space.md#orthogonal-projection) onto the row space $\mathcal R(A^H)$, so its eigenvalues are zero and one. Consequently

$$
\boxed{\operatorname{rank}(A^\dagger A)
=\operatorname{rank}(A)
=\operatorname{rank}(A^\dagger)
=\operatorname{tr}(A^\dagger A).}
$$

<h4 id="1/b/iv">iv</h4>

↑ **Parent:** [B](#1/b)

<h5 id="1/b/iv/solution">Solution</h5>

↑ **Parent:** [Iv](#1/b/iv)

The [Reverse-order law for the Moore--Penrose inverse](../../../linear-algebra.md#reverse-order-law-for-the-moore-penrose-inverse) is false in general. Take

$$
A=\begin{pmatrix}1&0\\0&2\\0&0\end{pmatrix},
\qquad
B=\begin{pmatrix}1\\1\end{pmatrix}.
$$

Then

$$
(AB)^\dagger=\begin{pmatrix}1/5&2/5&0\end{pmatrix},
\qquad
B^\dagger A^\dagger=\begin{pmatrix}1/2&1/4&0\end{pmatrix}.
$$

A sufficient condition is

$$
\operatorname{rank}(A)=n,
\qquad
\operatorname{rank}(B)=n,
$$

so that $A$ has [full column rank](../../../vector-space.md#full-column-rank) and $B$ has [full row rank](../../../vector-space.md#full-row-rank). Indeed $A^\dagger A=I_n$ and $BB^\dagger=I_n$; these identities make $B^\dagger A^\dagger$ satisfy all four [Penrose equations](../../../linear-algebra.md#penrose-equations) for $AB$.

<h3 id="1/c">c</h3>

↑ **Parent:** [1](#1)

<h4 id="1/c/i">i</h4>

↑ **Parent:** [C](#1/c)

<h5 id="1/c/i/solution">Solution</h5>

↑ **Parent:** [I](#1/c/i)

If $B=\sup_j|d_j|<\infty$, then for every $f\in\ell^2$,

$$
\|Df\|_2^2=\sum_j|d_j|^2|f_j|^2
\leq B^2\|f\|_2^2,
$$

so the [diagonal operator on sequence space](../../../functional-analysis.md#diagonal-operator-on-sequence-space) is bounded. Conversely, for the standard unit vector $e_j$,

$$
|d_j|=\|De_j\|_2\leq\|D\|,
$$

so boundedness of $D$ implies $\sup_j|d_j|\leq\|D\|<\infty$.

<h4 id="1/c/ii">ii</h4>

↑ **Parent:** [C](#1/c)

<h5 id="1/c/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#1/c/ii)

Part i gives $\|D\|\leq B$. Conversely, choose indices $j_k$ with $|d_{j_k}|\to B$. Since $\|e_{j_k}\|_2=1$,

$$
\|D\|\geq\|De_{j_k}\|_2=|d_{j_k}|.
$$

Taking the [limit](../../../calculus.md#limit-of-a-function) proves $\boxed{\|D\|=B}$, whether or not the [supremum](../../../real-analysis.md#supremum) is attained.

<h4 id="1/c/iii">iii</h4>

↑ **Parent:** [C](#1/c)

<h5 id="1/c/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#1/c/iii)

The [Moore-Penrose inverse](../../../linear-algebra.md#moore-penrose-inverse) acts coordinatewise as

$$
[D^\dagger g]_j=
\begin{cases}
g_j/d_j,&d_j\ne0,\\
0,&d_j=0,
\end{cases}
$$

on the domain

$$
\mathcal D(D^\dagger)
=\left\{g\in\ell^2:
\sum_{d_j\ne0}\frac{|g_j|^2}{|d_j|^2}<\infty\right\}.
$$

The coordinates supported where $d_j=0$ form $\mathcal R(D)^\perp$ and are sent to zero. The inverse is continuous exactly when the nonzero diagonal entries are bounded away from zero,

$$
\inf_{d_j\ne0}|d_j|>0,
$$

apart from the trivial all-zero operator, whose inverse is zero. Otherwise unit vectors along entries tending to zero show that $D^\dagger$ is unbounded.

<h4 id="1/c/iv">iv</h4>

↑ **Parent:** [C](#1/c)

<h5 id="1/c/iv/solution">Solution</h5>

↑ **Parent:** [Iv](#1/c/iv)

For $d_j=1/j$, the equation $Du=f$ forces $u_j=jf_j$. It has a solution in $\ell^2$ exactly when

$$
\sum_{j=1}^\infty j^2|f_j|^2<\infty.
$$

For example, $f_j=1/j$ defines an element of $\ell^2$, but its forced preimage is the constant sequence $u_j=1$, which is not in $\ell^2$. Thus existence can fail. Since every $d_j$ is nonzero, $D$ has [trivial kernel](../../../linear-algebra.md#trivial-kernel) and any solution is unique.

<h4 id="1/c/v">v</h4>

↑ **Parent:** [C](#1/c)

<h5 id="1/c/v/solution">Solution</h5>

↑ **Parent:** [V](#1/c/v)

The proposed stability property is false. Set $u^*=0$, $f^*=0$, and take $u_n=e_n$. Then

$$
f_n=Du_n=\frac1n e_n,
\qquad
\|f_n-f^*\|_2=\frac1n\longrightarrow0,
$$

while $\|u_n-u^*\|_2=1$ for every $n$. Hence the inverse is not continuous on its range and the recovery problem is not [stable with respect to perturbations](../../../inverse-problem.md#well-posed-problem). This is the standard [unbounded inverse on a nonclosed operator range](../../../functional-analysis.md#unbounded-inverse-on-a-nonclosed-operator-range).

## 2

↑ **Parent:** [Paper 326](paper-326.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/i">i</h4>

↑ **Parent:** [A](#2/a)

<h5 id="2/a/i/solution">Solution</h5>

↑ **Parent:** [I](#2/a/i)

The extended-real functional $f:X\to\overline{\mathbb R}$ is [sequentially lower semicontinuous](../../../calculus.md#sequential-lower-semicontinuity) in the topology $\tau_X$ when every sequence $x_n\to x$ in $\tau_X$ satisfies

$$
\boxed{f(x)\leq\liminf_{n\to\infty}f(x_n).}
$$

<h4 id="2/a/ii">ii</h4>

↑ **Parent:** [A](#2/a)

<h5 id="2/a/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#2/a/ii)

The assertion is understood for every $\eta\in\mathbb R$ and for a topology in which sequentially closed sets are closed, in particular the norm topology of a [Banach space](../../../banach-space.md). Suppose first that $f$ is [sequentially lower semicontinuous](../../../calculus.md#sequential-lower-semicontinuity) and $x_n\in\Omega_\eta=\{x:f(x)\leq\eta\}$ converges to $x$. Then

$$
f(x)\leq\liminf_nf(x_n)\leq\eta,
$$

so $x\in\Omega_\eta$ and the sublevel set is closed. Conversely, if all sublevel sets are closed but lower semicontinuity fails, there are $x_n\to x$ and a real $\eta<f(x)$ with a subsequence satisfying $f(x_{n_k})\leq\eta$. Closedness of $\Omega_\eta$ would put $x$ in that set, a contradiction. This proves the [closed-sublevel-set characterization of lower semicontinuity](../../../calculus.md#closed-sublevel-set-characterization-of-lower-semicontinuity).

<h4 id="2/a/iii">iii</h4>

↑ **Parent:** [A](#2/a)

<h5 id="2/a/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#2/a/iii)

Use the extended-real characteristic functional

$$
\chi_{X'}(x)=
\begin{cases}
0,&x\in X',\\
+\infty,&x\notin X'.
\end{cases}
$$

For $\eta<0$ its sublevel set is empty, while for every finite $\eta\geq0$ its sublevel set is $X'$. Both are closed when $X'$ is closed, so part ii proves that this [indicator functional of a constraint set](../../../inverse-problem.md#indicator-functional-of-a-constraint-set) is lower semicontinuous.

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/i">i</h4>

↑ **Parent:** [B](#2/b)

<h5 id="2/b/i/solution">Solution</h5>

↑ **Parent:** [I](#2/b/i)

Let $T_\alpha=A^*A+\alpha I$. For every $f\in X$,

$$
\alpha\|f\|_X^2
\leq\langle f,T_\alpha f\rangle_X
=\|Af\|_Y^2+\alpha\|f\|_X^2
\leq(\|A\|^2+\alpha)\|f\|_X^2.
$$

Thus $T_\alpha$ is a [coercive operator](../../../functional-analysis.md#coercive-operator). If it is invertible and $T_\alpha f=g$, the lower bound and the [Cauchy-Schwarz inequality](../../../probability-and-statistics.md#cauchy-schwarz-inequality) give

$$
\alpha\|f\|^2\leq\langle f,g\rangle\leq\|f\|\|g\|,
$$

and therefore $\|T_\alpha^{-1}g\|\leq\alpha^{-1}\|g\|$. Hence

$$
\boxed{\|(A^*A+\alpha I)^{-1}\|\leq\frac1\alpha}.
$$

<h4 id="2/b/ii">ii</h4>

↑ **Parent:** [B](#2/b)

<h5 id="2/b/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#2/b/ii)

Subtracting $T_\alpha u_n=z_n$ and $T_\alpha u_m=z_m$ and applying the coercive estimate from part i yields

$$
\|u_n-u_m\|_X
\leq\frac1\alpha\|z_n-z_m\|_X.
$$

**Thus $(z_n)$ Cauchy implies $(u_n)$ Cauchy. Completeness of the [Hilbert space](../../../hilbert-space.md) $X$ gives $u_n\to u\in X$, and boundedness of $T_\alpha$ gives $z_n=T_\alpha u_n\to T_\alpha u$.**

<h4 id="2/b/iii">iii</h4>

↑ **Parent:** [B](#2/b)

<h5 id="2/b/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#2/b/iii)

The lower bound in part i shows that $T_\alpha u=0$ implies $u=0$, so $T_\alpha$ is injective. Since $T_\alpha$ is self-adjoint,

$$
\overline{\mathcal R(T_\alpha)}
=\mathcal N(T_\alpha^*)^\perp
=\mathcal N(T_\alpha)^\perp=X,
$$

so its range is dense. Part ii shows that its range is also closed: a convergent sequence $z_n=T_\alpha u_n$ has Cauchy preimages, whose limit $u$ satisfies $T_\alpha u=\lim z_n$. Hence $\mathcal R(T_\alpha)=X$. The operator is bijective, and the estimate in part i proves that its inverse is bounded. Therefore $A^*A+\alpha I$ is invertible for every $\alpha>0$.

<h4 id="2/b/iv">iv</h4>

↑ **Parent:** [B](#2/b)

<h5 id="2/b/iv/solution">Solution</h5>

↑ **Parent:** [Iv](#2/b/iv)

The equation $(A^*A+\alpha_*I)u_*=A^*f$ is the [Tikhonov normal equation](../../../inverse-problem.md#tikhonov-normal-equation). For $u=u_*+h$, expand the [Tikhonov regularization](../../../inverse-problem.md#tikhonov-regularization) functional:

$$
\begin{aligned}
\phi_{\alpha_*}(u)
&=\phi_{\alpha_*}(u_*)
+2\operatorname{Re}\langle A^*(Au_*-f)+\alpha_*u_*,h\rangle_X\\
&\quad+\|Ah\|_Y^2+\alpha_*\|h\|_X^2.
\end{aligned}
$$

The normal equation makes the linear term zero. The final two terms are nonnegative and are strictly positive for $h\ne0$ because $\alpha_*>0$. Thus $u_*$ is the unique global minimizer.

<h3 id="2/c">c</h3>

↑ **Parent:** [2](#2)

<h4 id="2/c/i">i</h4>

↑ **Parent:** [C](#2/c)

<h5 id="2/c/i/solution">Solution</h5>

↑ **Parent:** [I](#2/c/i)

The objective separates by coordinates, so minimize

$$
h_i(z)=\frac12(z-x_i)^2+\lambda|z|.
$$

The [subgradient optimality condition](../../../real-analysis.md#subgradient-optimality-condition) is

$$
0\in z-x_i+\lambda\,\partial|z|.
$$

For $z>0$ this gives $z=x_i-\lambda$, valid when $x_i>\lambda$; for $z<0$ it gives $z=x_i+\lambda$, valid when $x_i<-\lambda$. At $z=0$, the condition is $x_i\in[-\lambda,\lambda]$. Therefore the shrinkage operator is the [soft-thresholding operator](../../../probability-and-statistics.md#soft-thresholding)

$$
[\psi_\lambda(x)]_i
=\begin{cases}
x_i-\lambda,&x_i>\lambda,\\
0,&-\lambda\leq x_i\leq\lambda,\\
x_i+\lambda,&x_i<-\lambda.
\end{cases}
$$

<h4 id="2/c/ii">ii</h4>

↑ **Parent:** [C](#2/c)

<h5 id="2/c/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#2/c/ii)

The graph is continuous and piecewise linear: it is horizontal at zero on $[-\lambda,\lambda]$ and has slope one outside that interval, joining the axis at $(-\lambda,0)$ and $(\lambda,0)$.

```
 psi
  ^
  |                    /
  |                   /
--+---------==========--------> x
 /         -lambda  lambda
/
```

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2022](../../2022.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
