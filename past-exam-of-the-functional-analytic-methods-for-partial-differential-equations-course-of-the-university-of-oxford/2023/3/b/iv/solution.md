<h1 id="3/b/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

The [zero extension of H01](../../../../../zero-extension-of-h01.md) makes $v_m$ an element of $H^1(\mathbb R^3)$. The [chain rule](../../../../../chain-rule.md) and [change of variables](../../../../../change-of-variables-formula.md) give the exact scaling identities

$$
\boxed{\|\nabla v_m\|_{L^2(\mathbb R^3)}^2=\|\nabla u_m\|_{L^2(B)}^2,\qquad
\|v_m\|_{L^2(\mathbb R^3)}^2=r_m^{-2}\|u_m\|_{L^2(B)}^2.}
$$

Indeed $\nabla v_m(x)=r_m^{3/2}\nabla u_m(r_mx)$ inside the expanded ball, and there is no boundary jump because the [Sobolev trace](../../../../../trace-operator.md) is zero.

First take the printed convergence assertion as an assumption, as the question requests. It would imply $\|\nabla v_m\|_2\to\|\nabla v\|_2>0$. The strict inequality follows because an $H^1(\mathbb R^3)$ function with zero [weak gradient](../../../../../weak-gradient.md) is constant [almost everywhere](../../../../../almost-everywhere.md), and the only constant in $L^2(\mathbb R^3)$ is zero; this contradicts the asserted positivity of $v$. If $u_m$ converged strongly in $H^1(B)$, its limit would have to be its [weak limit](../../../../../weak-limit.md) zero from (iii), forcing $\|\nabla u_m\|_2\to0$. The first scaling identity contradicts this. Thus the intended answer is

$$
\boxed{u_m\text{ does not converge strongly in }H^1(B).}
$$

There is nevertheless a substantive printing error: the asserted strong convergence of $v_m$ in the full $H^1(\mathbb R^3)$ is false for these positive sources. Here is a check that does not rely on any assertion about the limiting profile. Put $R_m=r_m^{-1}$ and $c=|E|^{-5/6}$. Rescaling the [weak formulation](../../../../../weak-formulation.md) gives

$$
-\Delta v_m=c\chi_E\quad\text{in }B_{R_m},\qquad v_m=0\quad\text{on }\partial B_{R_m}.
$$

The [spherical mean of a Poisson solution outside its source](../../../../../spherical-mean-of-a-poisson-solution-outside-its-source.md) provides an exact obstruction. The total source is $M=c|E|=|E|^{1/6}>0$. Let $a_m(s)=(4\pi)^{-1}\int_{S^2}v_m(s\omega)\,d\omega$ be its [spherical mean](../../../../../spherical-mean.md). On $1<s<R_m$ the function is a [harmonic function](../../../../../harmonic-function.md). The radial flux identity, obtained by testing against radial [test functions](../../../../../test-function.md) or by the [divergence theorem](../../../../../divergence-theorem.md), gives $-4\pi s^2a_m'(s)=M$, while the zero boundary value gives $a_m(R_m)=0$. Hence

$$
a_m(s)=\frac{M}{4\pi}\left(\frac1s-\frac1{R_m}\right)\qquad(1<s<R_m).
$$

[Cauchy-Schwarz inequality](../../../../../cauchy-schwarz-inequality.md) on each sphere, followed by [spherical coordinates](../../../../../spherical-coordinate-system.md), now yields

$$
\begin{aligned}
\|v_m\|_2^2
&\geq4\pi\int_1^{R_m}s^2a_m(s)^2\,ds\\
&=\frac{M^2}{4\pi}\left(\frac{R_m}{3}-1+\frac1{R_m}-\frac1{3R_m^2}\right)
\longrightarrow\infty.
\end{aligned}
$$

Thus the printed sequence is not even bounded in the full $H^1$ [norm](../../../../../norm.md). The result on [Poisson convergence on expanding balls in a homogeneous Sobolev space](../../../../../poisson-convergence-on-expanding-balls-in-a-homogeneous-sobolev-space.md) gives the appropriate corrected convergence in the [homogeneous Sobolev space](../../../../../homogeneous-sobolev-space.md) $\dot H^1(\mathbb R^3)$, which controls the [gradient](../../../../../gradient.md) in $L^2$ and the function in $L^6$, without requiring it to belong to $L^2$.

For completeness, the desired nonconvergence of $u_m$ has a direct proof that needs neither the incorrect claim nor its correction. Choose a nonnegative nonzero [test function](../../../../../test-function.md) $\eta\in C_c^\infty(E)$, which exists since $E$ is a domain containing the origin. The rescaled [weak formulation](../../../../../weak-formulation.md) and [Cauchy-Schwarz inequality](../../../../../cauchy-schwarz-inequality.md) give

$$
0<c\int_E\eta\,dx
=\int_{\mathbb R^3}\nabla v_m\cdot\nabla\eta\,dx
\leq\|\nabla v_m\|_2\|\nabla\eta\|_2.
$$

Consequently, for every $m$,

$$
\boxed{\|\nabla u_m\|_2=\|\nabla v_m\|_2
\geq\frac{|E|^{-5/6}\int_E\eta\,dx}{\|\nabla\eta\|_2}>0.}
$$

Together with (iii), this rigorously proves failure of [strong convergence](../../../../../norm-convergence.md) for the actual sequence defined in the paper.

## ↑ Ancestors (13)

1. [Iv](../iv.md)
2. [B](../../b.md)
3. [3](../../../3.md)
4. [2023](../../../../2023-split.md)
5. [Past exam of the functional analytic methods for partial differential equations course of the University of Oxford](../../../../split.md)
6. [Functional analytic methods for partial differential equations course of the University of Oxford](../../../../../functional-analytic-methods-for-partial-differential-equations-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
