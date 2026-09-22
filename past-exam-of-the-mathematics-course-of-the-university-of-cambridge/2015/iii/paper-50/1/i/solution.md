<h1 id="1/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Only the empty binary configuration contributes to $f$, and only the occupied configuration contributes to $g$. Thus the [Hirota tau functions](../../../../../../hirota-tau-function.md) give

$$
f=1,\qquad g=e^X,\qquad \phi=4\arctan e^X,\qquad X=\kappa x-\beta_1t+\gamma.
$$

Here $\beta_1$ denotes the velocity parameter, while $\beta$ without a subscript remains the coupling of [Sine-Gordon theory](../../../../../../sine-gordon-theory.md). For $\kappa>0$, the field approaches the adjacent [scalar-field vacua](../../../../../../scalar-field-vacuum.md) $0$ and $2\pi$ at the two ends of space, so its [topological charge](../../../../../../topological-charge.md) is $1$. Its center is $X=0$, giving

$$
\boxed{v=\frac{\beta_1}{\kappa},\qquad x_{\rm center}(t)=vt-\frac\gamma\kappa,\qquad |v|<1.}
$$

The constraint $\kappa^2-\beta_1^2=1$ implies $\kappa=(1-v^2)^{-1/2}$. Hence this is precisely a [Lorentz boost](../../../../../../lorentz-boost.md) of the static [Sine-Gordon kink](../../../../../../sine-gordon-kink.md), with the expected [Lorentz contraction](../../../../../../length-contraction.md). As a direct check, if $F(X)=4\arctan e^X$, then $F'=2\operatorname{sech}X$ and $F''=\sin F$, so $(\partial_t^2-\partial_x^2)\phi+\sin\phi=(\beta_1^2-\kappa^2)F''+\sin F=0$.

The real-parameter condition also permits $\kappa<0$. That choice reverses the [topological charge](../../../../../../topological-charge.md) and describes an [antikink](../../../../../../antikink.md). The all-[kink](../../../../../../scalar-field-kink.md) scattering formulas below use $\kappa_i>0$; the orientation dependence is stated explicitly at the end of the two-body calculation.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [1](../../1.md)
3. [Paper 50](../../../paper-50-split.md)
4. [Iii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
