<h1 id="3/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Away from forcing, set $F=0$. For a linear sinusoidal disturbance $A=\operatorname{Re}[\widehat A e^{i(kx-\omega t)}]$, the reduced equation gives

$$
-i\sigma k^3+i\beta\alpha_1\omega=0,\qquad\boxed{\omega=\frac{\sigma}{\beta\alpha_1}k^3}.
$$

Since $\sigma,\beta,\alpha_1>0$, the [phase velocity](../../../../../../phase-velocity.md) $c_p=\omega/k=\sigma k^2/(\beta\alpha_1)$ is positive for every nonzero wavenumber. The [group velocity](../../../../../../group-velocity.md) is

$$
\boxed{c_g=\frac{d\omega}{dk}=3\frac{\sigma k^2}{\beta\alpha_1}=3c_p>0}.
$$

Thus both the linear phase and wave packet travel downstream; the sign of $k$ does not introduce an upstream branch.

Now seek a permanent nonlinear wave with $\xi=x+ct$, for which the propagation [velocity](../../../../../../velocity.md) is $-c$. Substitution gives $\sigma A^{(3)}-\beta\alpha_1cA'-\alpha_2AA'=0$. Integration with vanishing far-field data gives

$$
\sigma A''-\beta\alpha_1cA-\frac{\alpha_2}{2}A^2=0.
$$

Multiplying by $A'$ and integrating again, with zero integration constant, gives

$$
\boxed{\sigma(A')^2=A^2\left(\beta\alpha_1c+\frac{\alpha_2}{3}A\right)}.
$$

Here $\alpha_2>0$, because $\gamma_0>\gamma_1>0$ and $R<R+1$. A smooth nonzero wave approaching zero requires $c>0$: for $c<0$ the right-hand side is negative at sufficiently small nonzero $A$. At $c=0$ the allowed positive branch has no nonzero turning point, so it cannot form a smooth localized pulse.

When $c>0$, the nonzero turning point is $A_m=-3\beta\alpha_1c/\alpha_2$. The energy curve is positive between $A_m$ and zero and negative below $A_m$, giving a homoclinic negative pulse. The positive branch has no turning point and cannot return to zero. Therefore

$$
\boxed{A<0,\qquad |A|_{\max}=\frac{3\beta\alpha_1c}{\alpha_2},\qquad\text{propagation velocity}=-c<0}.
$$

An explicit solution, also confirming smooth exponential tails, is

$$
A(\xi)=-\frac{3\beta\alpha_1c}{\alpha_2}\operatorname{sech}^2\!\left[\frac12\left(\frac{\beta\alpha_1c}{\sigma}\right)^{1/2}(\xi-\xi_0)\right].
$$

This establishes the [opposite propagation directions in the annular displacement equation](../../../../../../opposite-propagation-directions-in-the-annular-displacement-equation.md): linear waves move downstream while its localized nonlinear depression waves move upstream.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [3](../../3.md)
3. [Paper 75](../../../paper-75-split.md)
4. [Iii](../../../split.md)
5. [2003](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
