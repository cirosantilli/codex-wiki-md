<h1 id="4/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Define the signed [dimensionless](../../../../dimensionless-quantity.md) displacement

$$
\lambda=\sqrt{\frac{m\omega}{2\hbar}}x_0.
$$

The [spatial translation operator](../../../../spatial-translation-operator.md) is $T(x_0)=e^{-ipx_0/\hbar}$, and the phases of the new [energy eigenstates](../../../../energy-eigenstate.md) are fixed by $|n'\rangle=T(x_0)|n\rangle$. Their expansion coefficients are therefore

$$
\langle n'|0\rangle=\langle n|T(-x_0)|0\rangle.
$$

Since $p=i\sqrt{m\hbar\omega/2}(a^\dagger-a)$,

$$
T(-x_0)=e^{-\lambda(a^\dagger-a)}.
$$

Set $A=-\lambda a^\dagger$ and $B=\lambda a$. Their [commutator](../../../../commutator.md) is $[A,B]=\lambda^2I$, which commutes with both operators. Thus the stated special case of the [Baker--Campbell--Hausdorff formula](../../../../baker-campbell-hausdorff-formula.md) is applicable and gives

$$
e^{A+B}=e^{-\lambda^2/2}e^Ae^B.
$$

Because $a|0\rangle=0$,

$$
T(-x_0)|0\rangle=e^{-\lambda^2/2}e^{-\lambda a^\dagger}|0\rangle
=e^{-\lambda^2/2}\sum_{n=0}^\infty\frac{(-\lambda)^n}{\sqrt{n!}}|n\rangle.
$$

Taking the overlaps with $\langle n|$ therefore proves

$$
\boxed{|0\rangle=e^{-\lambda^2/2}\sum_{n=0}^\infty\frac{(-\lambda)^n}{\sqrt{n!}}|n'\rangle}.
$$

This is the [coherent state after shifting an oscillator equilibrium](../../../../coherent-state-after-shifting-an-oscillator-equilibrium.md). Its normalization follows from $e^{-\lambda^2}\sum_n\lambda^{2n}/n!=1$.

There is a sign qualification in the printed expansion: $(m\omega x_0^2/(2\hbar))^{n/2}=|\lambda|^n$ agrees with $(-\lambda)^n$ when $x_0\leq0$, equivalently $\gamma\geq0$. For a general signed displacement $x_0>0$, the odd coefficients have the opposite sign in the specified translated basis. The squared displacement alone fixes the occupation probabilities, not these coherent relative phases. The two-exponential identity also requires the central-commutator condition used above; it is not valid in that simple form for arbitrary operators.

## ↑ Ancestors (14)

1. [C](../c.md)
2. [4](../../4.md)
3. [2018](../../../2018-split.md)
4. [Past exam of the theoretical physics II course of the University of Cambridge](../../../split.md)
5. [Theoretical Physics II course of the University of Cambridge](../../../../theoretical-physics-ii-course-of-the-university-of-cambridge.md)
6. [Theoretical Physics course of the University of Cambridge](../../../../theoretical-physics-course-of-the-university-of-cambridge.md)
7. [Physics course of the year 3 of the natural sciences course of the University of Cambridge](../../../../physics-course-of-the-year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 3 of the natural sciences course of the University of Cambridge](../../../../year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../list-of-universities.md)
14. [Codex Wiki](../../../../split.md)
