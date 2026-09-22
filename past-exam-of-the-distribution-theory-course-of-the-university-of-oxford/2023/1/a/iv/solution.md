<h1 id="1/a/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

The bound $0\leq d_n\leq2^{-n-1}$ proves [uniform convergence](../../../../../uniform-convergence.md) of the series by the [Weierstrass M-test](../../../../../weierstrass-m-test.md). Each summand is continuous and satisfies $d_n(x+1)=d_n(x)$, so its sum $t$, the [Takagi function](../../../../../blancmange-curve.md), is continuous and has period one.

For $n\geq m$, both $2^nu_m$ and $2^nv_m$ are integers, giving $d_n(u_m)=d_n(v_m)=0$. Therefore

$$
S_m:=\frac{t(v_m)-t(u_m)}{v_m-u_m}
=\sum_{n=0}^{m-1}\frac{d_n(v_m)-d_n(u_m)}{v_m-u_m}.
$$

The corners of $d_n$ occur on the grid $2^{-n-1}\mathbb Z$. When $n<m$, that grid is contained in $2^{-m}\mathbb Z$, so the interior of $[u_m,v_m]$ contains no corner of $d_n$. Its slope on this interval is consequently $+1$ or $-1$.

The interval $[u_{m+1},v_{m+1}]$ is a half of $[u_m,v_m]$. All the old slopes persist on this half, and the new summand contributes one more slope in $\{\pm1\}$. Thus

$$
\boxed{S_{m+1}-S_m\in\{\pm1\}.}
$$

If $t$ had a finite [derivative](../../../../../derivative.md) $L$ at $x_0$, write $t(y)=t(x_0)+L(y-x_0)+r(y)$ with $r(y)=o(|y-x_0|)$. Since $u_m\leq x_0<v_m$ and both endpoints tend to $x_0$,

$$
|S_m-L|\leq\frac{|r(v_m)|+|r(u_m)|}{v_m-u_m}\longrightarrow0.
$$

Indeed $|v_m-x_0|+|u_m-x_0|=v_m-u_m$; when $u_m=x_0$, its remainder is zero. This is the [secants straddling a differentiability point](../../../../../secants-straddling-a-differentiability-point.md) argument, including dyadic $x_0$. But the displayed increments prevent $S_m$ from converging. Hence $\boxed{t\text{ is nowhere differentiable}}$, using periodicity to cover all real $x_0$.

For the [distributional derivative](../../../../../distributional-derivative.md), set $r_n(x)=s(2^nx)$, using $s$ from part (iii). The change of variable in the [distributional derivative](../../../../../distributional-derivative.md) pairing gives $d_n'=r_n$; these are the [Rademacher functions](../../../../../rademacher-function.md). [Uniform convergence](../../../../../uniform-convergence.md) implies [weak convergence of distributions](../../../../../weak-convergence-of-distributions.md), and the [continuity of distributional differentiation](../../../../../continuity-of-distributional-differentiation.md) allows termwise differentiation in that topology. Explicitly,

$$
\boxed{t'=\sum_{n=0}^{\infty}r_n\quad\text{in }\mathcal D'(\mathbb R),\qquad
\langle t',\phi\rangle=-\int_{\mathbb R}t(x)\phi'(x)\,dx.}
$$

This series assertion is a [distributional convergence](../../../../../weak-convergence-of-distributions.md) statement. Its remainder satisfies the concrete estimate

$$
\left|\left\langle t'-\sum_{n=0}^{N}r_n,\phi\right\rangle\right|
\leq2^{-N-1}\|\phi'\|_{L^1}\longrightarrow0.
$$

It supplies a well-defined [distributional derivative](../../../../../distributional-derivative.md) even though the ordinary [derivative](../../../../../derivative.md) exists nowhere.

## ↑ Ancestors (13)

1. [Iv](../iv.md)
2. [A](../../a.md)
3. [1](../../../1.md)
4. [2023](../../../../2023-split.md)
5. [Past exam of the distribution theory course of the University of Oxford](../../../../split.md)
6. [Distribution theory course of the University of Oxford](../../../../../distribution-theory-course-of-the-university-of-oxford.md)
7. [Year 3 of the mathematics course of the University of Oxford](../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
