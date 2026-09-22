<h1 id="question-5/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Enforce the fixed-end [Dirichlet boundary condition](../../../../../../dirichlet-boundary-condition.md) by taking the [odd extension](../../../../../../odd-extension.md) of the initial [velocity](../../../../../../velocity.md) to the whole line:

$$
v_o(s)=\kappa s e^{-|s|/L}.
$$

This agrees with the specified [initial condition](../../../../../../initial-condition.md) for $s\geq0$. To derive the relevant form of [D'Alembert's formula](../../../../../../d-alembert-s-formula.md), the zero initial displacement in [b](../b.md) gives $G=-F$, up to a cancelling constant. The initial [velocity](../../../../../../velocity.md) then gives $-2cF'=v_o$. Hence

$$
y(x,t)=\frac1{2c}\int_{x-ct}^{x+ct}v_o(s)\,ds.
$$

An [antiderivative](../../../../../../antiderivative.md), valid across $s=0$, is

$$
\int s e^{-|s|/L}\,ds=-L(|s|+L)e^{-|s|/L}.
$$

Evaluation therefore gives the solution throughout $x>0,t>0$:

$$
\boxed{y(x,t)=\frac{\kappa L}{2c}
\left[(|x-ct|+L)e^{-|x-ct|/L}
-(x+ct+L)e^{-(x+ct)/L}\right].}
$$

For $ct\leq x$, replace $|x-ct|$ by $x-ct$; for $ct\geq x$, replace it by $ct-x$. Thus the same expression includes the reflected [wave](../../../../../../wave-split.md) after it reaches the fixed end.

At $x=0$ the two terms agree, so $y(0,t)=0$. At $t=0$ they again agree, so $y(x,0)=0$. Differentiating the [integral](../../../../../../integral-split.md) with respect to $t$ gives

$$
y_t(x,t)=\frac12\bigl[v_o(x+ct)+v_o(x-ct)\bigr],
$$

which recovers $y_t(x,0)=\kappa xe^{-x/L}$. Since $v_o$ is a [continuously differentiable function](../../../../../../continuously-differentiable-function.md), the formula is twice continuously differentiable even across $x=ct$, and satisfies the [wave equation](../../../../../../wave-equation-split.md) there as well.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [Question 5](../../question-5.md)
3. [Mathematics V resit](../../../mathematics-v-resit-split.md)
4. [Prelims](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Oxford](../../../../../split.md)
7. [Mathematics course of the University of Oxford](../../../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../split.md)
