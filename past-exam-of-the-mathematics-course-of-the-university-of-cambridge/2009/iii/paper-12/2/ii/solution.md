<h1 id="2/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

There is a qualification in the printed hypotheses: [quadratic ellipticity does not bound a nonsymmetric coefficient matrix](../../../../../../quadratic-ellipticity-does-not-bound-a-nonsymmetric-coefficient-matrix.md). The intended standard existence proof needs $a_{ij}\in L^\infty(\Omega)$, or more generally a bounded principal [bilinear form](../../../../../../bilinear-form.md). To see why this does not follow from the displayed inequalities, take $\Omega=(-1,1)^2$ and

$$
A(x)=\begin{pmatrix}1&k(x_1)\\-k(x_1)&1\end{pmatrix},\qquad k(t)=\begin{cases}|t|^{-1}&t\ne0,\\0&t=0.\end{cases}
$$

Then $\zeta^TA(x)\zeta=|\zeta|^2$ for every $x,\zeta$. However, choose $u_0,\varphi_0\in C_c^\infty(\Omega)$ equal to $x_2,x_1$, respectively, on a small rectangle about the origin. There $(A Du_0)\cdot D\varphi_0=k(x_1)$, whose positive part has infinite integral. Thus the standard principal pairing is not a finite Lebesgue integral even for these smooth [test functions](../../../../../../test-function.md). This demonstrates the missing form hypothesis, rather than assuming that all unbounded skew coefficients prevent solvability.

Under the intended bounded-coefficient hypothesis the proof is as follows. On $H=H_0^1(\Omega)$ use the [Hilbert space](../../../../../../hilbert-space-split.md) [norm](../../../../../../norm.md) $\|Dw\|_2$, equivalent to the $H^1$ [norm](../../../../../../norm.md) by the [Poincaré inequality](../../../../../../poincare-inequality.md) on a bounded domain. The form from part (i) is bounded, since

$$
|B(w,v)|\leq\|A\|_{\infty,\mathrm{op}}\|Dw\|_2\|Dv\|_2+\|q\|_\infty\|w\|_2\|v\|_2\leq C\|Dw\|_2\|Dv\|_2.
$$

It is a [coercive bilinear form](../../../../../../coercive-bilinear-form.md) even without symmetry:

$$
B(w,w)=\int_\Omega a_{ij}D_jwD_iw-\int_\Omega qw^2\geq\lambda\|Dw\|_2^2.
$$

Here the nonpositive sign of $q$ is essential. With $u=\psi+w$, the required equation becomes

$$
B(w,v)=\ell(v),\qquad\ell(v)=-\int_\Omega fv-B(\psi,v).
$$

The [Cauchy-Schwarz inequality](../../../../../../cauchy-schwarz-inequality.md), bounded coefficients and the [Poincaré inequality](../../../../../../poincare-inequality.md) show that $\ell$ is a bounded [linear functional](../../../../../../linear-functional.md) on $H$. The [Lax-Milgram theorem](../../../../../../lax-milgram-theorem.md) states that a bounded coercive [bilinear form](../../../../../../bilinear-form.md) on a real Hilbert space represents each bounded [linear functional](../../../../../../linear-functional.md) in this way with a unique $w\in H$. It therefore yields $u=\psi+w$ with the required boundary condition and weak equation. For completeness, if $u_1,u_2$ are solutions, $z=u_1-u_2\in H_0^1$ satisfies $B(z,z)=0$; [coercivity](../../../../../../coercive-function.md) and the [Poincaré inequality](../../../../../../poincare-inequality.md) imply $z=0$.

**With the missing bounded-form hypothesis, the weak solution exists and is unique.** For nonsymmetric matrices the printed quadratic inequalities omit the hypothesis needed for this standard formulation and proof. No maximum principle is used. In part (iii), symmetry makes the quadratic upper bound a bound on the whole matrix, so no such qualification is needed there.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [2](../../2.md)
3. [Paper 12](../../../paper-12-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
